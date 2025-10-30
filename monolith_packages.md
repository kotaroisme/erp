# Problem dengan Microservices

**Produk baru belum punya clarity tentang bounded context.** Saat kamu baru mulai, understanding tentang domain masih evolving. Apa yang kamu pikir sebagai "payments service" terpisah, ternyata coupled tight dengan "orders" dan "inventory" setelah beberapa sprint. Kalau sudah extract jadi service terpisah, refactor boundary jadi expensive: deploy coordination, API contract breaking, data migration cross-database.

**Operational complexity tidak proporsional dengan team size dan traffic.** Microservices membawa: service discovery, distributed logging, tracing, circuit breaker, retry logic, eventual consistency handling, deployment orchestration. Untuk produk dengan <10 engineer dan traffic <1000 req/s, ini adalah overhead yang consume energy lebih banyak daripada deliver value ke customer.

**Debugging dan development velocity turun significant.** Stack trace yang tadinya straightforward jadi distributed tracing cross multiple service. Local development butuh orchestrate beberapa service atau extensive mocking. Onboarding engineer baru dari "clone, run, debug" jadi "setup service A, B, C, configure connection, understand communication flow".

Ada kasus Team startup extract ke 8 microservices di month ke-3, lalu spend 6 bulan berikutnya berjuang dengan distributed transaction dan eventual consistency bug. Velocity turun 40% dan mereka akhirnya merge kembali beberapa service.

Microservices adalah solution untuk specific problem: independent scaling, independent deployment, organizational autonomy. Produk baru belum punya problem ini. Yang produk baru punya adalah uncertainty tentang domain model dan pressure untuk deliver value cepat.

Monolith dengan package adalah investment untuk future optionality tanpa premature commitment. Kita  pay small upfront cost (package discipline, static analysis) untuk avoid large future cost (distributed system complexity atau costly merge-back dari premature extraction).

Saat metrics show clear signal—scaling bottleneck yang tidak solve dengan vertical scaling, deployment conflict antar team, atau regulatory isolation requirement—extraction decision jadi obvious dengan data. Dan karena boundary sudah ada, extraction adalah engineering project dengan timeline predictable, bukan exploration dengan risk tinggi.

# Kenapa Monolith + Package
**Package boundaries sebagai rehearsal**

Package structure dalam monolith adalah prediksi awal microservice boundaries. Kalau package masih sering saling bergantung erat atau boundaries-nya blur, itu signal bahwa split akan sulit. Saya biasa mengukur coupling dengan dependency graph: kalau cyclic dependencies masih ada atau depth of call chain antar package >3 level, itu perlu diselesaikan dulu dalam monolith.

# Target Microservices
**Monitoring yang perlu ada sejak hari pertama**

Jangan tunggu sampai "mau split" baru pasang monitoring. Saya mulai dari tiga metrik dasar:

- Latency per package (bukan hanya endpoint-level, tapi logical boundary)
- Error rate per package
- Resource usage pattern (CPU, memory, I/O) di level package kalau bisa di-instrument

Kalau tooling belum support package-level metrics, gunakan structured logging dengan package identifier di setiap log entry. Ini bisa di-aggregate nanti.

**Kriteria "stabil" yang terukur**

Stabil bukan berarti "tidak ada bug", tapi business logic tidak lagi berubah drastis setiap sprint. Saya menggunakan dua indikator:

1. Change frequency: berapa banyak PR yang touch package tertentu dalam 3 bulan terakhir
2. Change scope: apakah perubahan itu bugfix minor atau redesign logic

Kalau change frequency tinggi tapi scope-nya kecil, itu acceptable. Kalau sering ada redesign, tunggu sampai domain understanding settle.

**Migration trigger yang jelas**

"Nanti bertahap diubah" perlu trigger konkret, bukan just feeling. Beberapa trigger yang reasonable:

- Scalability bottleneck: satu package butuh scale independent (misal: payment processing vs catalog browsing)
- Team structure: kalau team sudah grow dan ada ownership natural per domain
- Deployment friction: kalau deploy monolith jadi risky karena satu perubahan kecil bisa affect everything

Kalau trigger ini belum muncul setelah 1-2 tahun, tetap monolith adalah keputusan yang valid. Microservices bukan tujuan akhir, tapi respons terhadap constraint.
# Monolith Structure
erp/
├── package.yml  
└── packages/
    ├── accounting/
    │   ├── package.yml
    │   ├── README.mg
    ├── sales/
    │   ├── package.yml
    │   ├── README.md
    ├── integration/
    │   ├── package.yml
    │   └── README.md
    ├── hr/
    │   └── package.yml
    ├── inventory/
    │   └── package.yml
    ├── marketing/
    │   └── package.yml
    ├── projects/
    │   └── package.yml
    ├── productivity/
    │   └── package.yml
    └── reporting/
        └── package.yml
        
# Deployment
Target deployment ada dua Aplikasi dan Worker. Aplikasi akan bisa di akses secara public(customer). Worker adalah aplikasi yang jalan di background misal untuk async atau meneria webhook.

**Aplikasi sebagai public-facing process:** Handle HTTP request dari customer, serve API atau web interface, enforce authentication dan authorization, coordinate operation cross-package.

**Worker sebagai background process:** Consume job dari queue, handle webhook dari external service (payment gateway, email provider), execute scheduled task, process heavy computation yang tidak boleh block request-response cycle.

**Benefit dari separation ini:**

Resource allocation independent: Aplikasi butuh low latency response, Worker bisa toleran higher latency tapi butuh throughput tinggi. Aplikasi scale berdasarkan request per second, Worker scale berdasarkan queue depth.

Failure isolation: Worker crash tidak affect Aplikasi availability. Customer masih bisa browse dan submit order meskipun background email belum terkirim. Ini memberi graceful degradation natural.

Deployment risk lower: Deploy Worker tidak butuh zero-downtime strategy yang strict. Job yang in-progress bisa di-drain atau di-retry. Aplikasi deployment butuh careful rolling update untuk avoid request drop.