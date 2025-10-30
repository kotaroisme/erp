## 1. Sales & Customer Management

**CRM** - Lead dan opportunity management, pipeline tracking **Sales** - Quotation, sales order, pricelists, customer portal **Point of Sale (POS)** - Retail operations, kasir, inventory real-time **Subscriptions** - Recurring billing, contract management (Enterprise) **Rental** - Asset rental dengan pricing per periode (Enterprise)

| Technical Name              | Display Name         | Deskripsi                                                 |
| --------------------------- | -------------------- | --------------------------------------------------------- |
| `crm`                       | CRM                  | Lead management, pipeline tracking, activities scheduling |
| `sale_management`           | Sales                | Quotation, sales order, pricelists, delivery management   |
| `sale_crm`                  | CRM Integration      | Link CRM opportunities ke sales quotations                |
| `point_of_sale`             | Point of Sale        | Retail POS operations, offline mode, receipt printing     |
| `sale_subscription`         | Subscriptions        | Recurring billing, MRR tracking, automatic invoicing      |
| `sale_renting`              | Rental               | Asset rental dengan pricing per hour/day/week             |
| `sale_amazon`               | Amazon Connector     | Sync orders dan inventory dengan Amazon marketplace       |
| `sale_ebay`                 | eBay Connector       | Integration dengan eBay untuk listing dan orders          |
| `sale_loyalty`              | Loyalty & Gift Cards | Loyalty programs, points, gift cards, promotions          |
| `sale_product_configurator` | Product Configurator | Configure produk complex dengan variants dan options      |
| `sale_margin`               | Sales Margin         | Display margin di quotation dan sales order               |
| `sale_quotation_builder`    | Quotation Builder    | Drag-drop quotation builder dengan templates              |

## 2. Marketing & Website

**Website** - Website builder dengan drag-drop **eCommerce** - Online store, product catalog, checkout **Email Marketing** - Campaign builder, segmentation, analytics **Marketing Automation** - Lead nurturing workflows (Enterprise) **Social Marketing** - Posting scheduler multi-platform **SMS Marketing** - Bulk SMS campaigns **Events** - Event management, registrations, ticketing **Surveys** - Form dan survey builder

| Technical Name            | Display Name         | Deskripsi                                          |
| ------------------------- | -------------------- | -------------------------------------------------- |
| `website`                 | Website              | Website builder dengan drag-drop editor            |
| `website_sale`            | eCommerce            | Online store, shopping cart, product catalog       |
| `website_blog`            | Blog                 | Blog management dengan comments dan SEO            |
| `website_forum`           | Forum                | Community forum dengan gamification                |
| `website_slides`          | eLearning            | Course management, slides, quizzes, certifications |
| `website_event`           | Events               | Event website dengan registrations dan ticketing   |
| `website_crm`             | Contact Form         | Lead generation forms di website                   |
| `website_livechat`        | Live Chat            | Real-time chat widget di website                   |
| `mass_mailing`            | Email Marketing      | Mass email campaigns dengan templates              |
| `mass_mailing_sms`        | SMS Marketing        | Bulk SMS campaigns dan triggers                    |
| `marketing_automation`    | Marketing Automation | Lead nurturing workflows berbasis triggers         |
| `social_marketing`        | Social Marketing     | Schedule posts ke Facebook, LinkedIn, Twitter      |
| `surveys`                 | Surveys              | Survey builder dengan conditional questions        |
| `website_sale_wishlist`   | Wishlist             | Customer wishlist di eCommerce                     |
| `website_sale_comparison` | Product Comparison   | Compare products side-by-side                      |
## 3. Inventory & Supply Chain

**Inventory** - Stock management, warehousing, traceability **Purchase** - Purchase order, vendor management, RFQ **Manufacturing (MRP)** - Production planning, work orders, BoM **PLM** - Product lifecycle management, engineering change orders (Enterprise) **Maintenance** - Equipment maintenance scheduling **Quality** - Quality control checkpoints, alerts

| Technical Name         | Display Name            | Deskripsi                                                   |
| ---------------------- | ----------------------- | ----------------------------------------------------------- |
| `stock`                | Inventory               | Warehouse management, stock moves, traceability             |
| `purchase`             | Purchase                | Purchase orders, RFQ, vendor management                     |
| `mrp`                  | Manufacturing           | Production orders, work orders, Bill of Materials           |
| `mrp_subcontracting`   | Subcontracting          | Manage subcontracted manufacturing                          |
| `mrp_workorder`        | Work Orders             | Detailed work order management dengan tablet view           |
| `mrp_plm`              | PLM                     | Engineering change orders, version control                  |
| `quality_control`      | Quality                 | Quality checks, alerts, control points                      |
| `quality_mrp`          | Quality - Manufacturing | Quality checks di manufacturing process                     |
| `maintenance`          | Maintenance             | Equipment maintenance requests dan scheduling               |
| `stock_barcode`        | Barcode                 | Barcode scanning untuk inventory operations                 |
| `stock_dropshipping`   | Dropshipping            | Dropship workflows tanpa hold inventory                     |
| `stock_landed_costs`   | Landed Costs            | Distribute additional costs (shipping, customs) ke products |
| `stock_picking_batch`  | Batch Picking           | Group pickings untuk efficient warehouse operations         |
| `purchase_requisition` | Purchase Agreements     | Blanket orders, calls for tenders                           |
## 4. Accounting & Finance

**Accounting** - General ledger, journal entries, reconciliation **Invoicing** - Customer invoices, vendor bills **Expenses** - Employee expense claims, reimbursement **Documents** - AI document parsing untuk bills dan expenses (Enterprise) **Sign** - Digital signature untuk documents (Enterprise)

| Technical Name                      | Display Name           | Deskripsi                                          |
| ----------------------------------- | ---------------------- | -------------------------------------------------- |
| `account`                           | Accounting             | General ledger, journal entries, chart of accounts |
| `account_invoicing`                 | Invoicing              | Standalone invoicing tanpa full accounting         |
| `account_payment`                   | Payments               | Payment registration dan reconciliation            |
| `account_bank_statement_import`     | Bank Import            | Import bank statements dari CSV/OFX/CAMT           |
| `account_bank_statement_import_qif` | QIF Import             | Import Quicken Interchange Format                  |
| `account_reconcile_model`           | Reconciliation Models  | Automated reconciliation rules                     |
| `account_asset`                     | Assets Management      | Fixed assets, depreciation schedules               |
| `account_budget`                    | Budgets                | Budget management dan variance analysis            |
| `account_batch_payment`             | Batch Payments         | Batch payment processing untuk multiple invoices   |
| `account_sepa`                      | SEPA Credit Transfer   | Generate SEPA payment files                        |
| `account_sepa_direct_debit`         | SEPA Direct Debit      | SEPA direct debit mandates                         |
| `account_check_printing`            | Check Printing         | Print checks dari Odoo                             |
| `account_reports`                   | Accounting Reports     | Financial reports: P&L, balance sheet, cash flow   |
| `account_consolidation`             | Consolidation          | Multi-company consolidation                        |
| `account_intrastat`                 | Intrastat              | EU intrastat reporting                             |
| `account_tax_python`                | Python Taxes           | Define tax computation dengan Python code          |
| `hr_expense`                        | Expenses               | Employee expense management                        |
| `documents_account`                 | Documents - Accounting | AI parsing untuk vendor bills                      |
| `sign`                              | Sign                   | Digital signature untuk documents                  |
## 5. Human Resources

**Employees** - Employee database, contracts, org chart **Recruitment** - Applicant tracking, job postings **Time Off** - Leave management, accruals, approvals **Timesheets** - Time tracking per project/task **Attendances** - Check-in/out, kiosk mode **Payroll** - Salary computation, payslips (Enterprise) **Appraisal** - Performance reviews (Enterprise) **Fleet** - Vehicle management, fuel logs, maintenance **Referrals** - Employee referral programs (Enterprise)

| Technical Name       | Display Name         | Deskripsi                                            |
| -------------------- | -------------------- | ---------------------------------------------------- |
| `hr`                 | Employees            | Employee database, contracts, departments            |
| `hr_recruitment`     | Recruitment          | Job postings, applicant tracking                     |
| `hr_holidays`        | Time Off             | Leave requests, accruals, approvals                  |
| `hr_timesheet`       | Timesheets           | Time tracking per project dan task                   |
| `hr_attendance`      | Attendances          | Check-in/out, kiosk mode, overtime                   |
| `hr_payroll`         | Payroll              | Salary computation, payslips, accounting integration |
| `hr_payroll_account` | Payroll - Accounting | Link payroll ke accounting journals                  |
| `hr_contract`        | Contracts            | Employee contract management                         |
| `hr_appraisal`       | Appraisals           | Performance reviews dan 360 feedback                 |
| `hr_skills`          | Skills               | Skills tracking dan competency matrix                |
| `fleet`              | Fleet                | Vehicle management, fuel logs, maintenance           |
| `hr_referral`        | Referrals            | Employee referral programs dengan rewards            |
| `hr_work_entry`      | Work Entries         | Work entry validation untuk payroll                  |
| `hr_expense_extract` | Expense Digitization | OCR untuk expense receipts                           |
## 6. Project & Services

**Project** - Project management, tasks, milestones **Timesheets** - Time logging billable/non-billable **Planning** - Resource planning, shift scheduling (Enterprise) **Field Service** - Work orders, technician dispatch (Enterprise) **Helpdesk** - Ticket management, SLA tracking (Enterprise) **Appointments** - Online appointment booking

| Technical Name       | Display Name        | Deskripsi                                      |
| -------------------- | ------------------- | ---------------------------------------------- |
| `project`            | Project             | Project management, tasks, kanban, Gantt       |
| `hr_timesheet`       | Timesheets          | Time tracking (shared dengan HR)               |
| `timesheet_grid`     | Timesheet Grid      | Grid view untuk timesheet entry                |
| `project_forecast`   | Planning            | Resource planning dengan drag-drop             |
| `helpdesk`           | Helpdesk            | Ticket management, SLA tracking                |
| `helpdesk_timesheet` | Helpdesk Timesheets | Log time on support tickets                    |
| `industry_fsm`       | Field Service       | Work orders, technician scheduling, mobile app |
| `appointment`        | Appointments        | Online booking calendar                        |
| `sale_timesheet`     | Sales Timesheets    | Bill time dari timesheets                      |
| `project_purchase`   | Project Purchase    | Link purchase orders ke projects               |
## 7. Productivity & Collaboration

**Discuss** - Internal chat, channels, direct messages **Calendar** - Shared calendars, meeting scheduler **Contacts** - Contact database, shared across modules **VoIP** - Integrated calling (Enterprise) **Approvals** - Custom approval workflows (Enterprise) **Knowledge** - Internal wiki, documentation (Enterprise)

| Technical Name | Display Name | Deskripsi                                   |
| -------------- | ------------ | ------------------------------------------- |
| `mail`         | Discuss      | Internal chat, channels, notifications      |
| `calendar`     | Calendar     | Shared calendar, meeting scheduling         |
| `contacts`     | Contacts     | Contact database shared across apps         |
| `voip`         | VoIP         | Integrated calling dengan PBX integration   |
| `approvals`    | Approvals    | Custom approval workflows untuk any request |
| `knowledge`    | Knowledge    | Internal wiki, collaborative documentation  |
| `documents`    | Documents    | Document management system dengan tagging   |
| `web_mobile`   | Mobile       | Mobile-responsive views                     |

## 8. Reporting & Analytics

**Dashboards** - Custom dashboard builder **Spreadsheet** - Spreadsheet view untuk data analysis (Enterprise) **Studio** - No-code customization tool (Enterprise)

| Technical Name          | Display Name      | Deskripsi                                |
| ----------------------- | ----------------- | ---------------------------------------- |
| `board`                 | Dashboards        | Custom dashboard builder                 |
| `spreadsheet_dashboard` | Spreadsheet       | Spreadsheet-based reports dan dashboards |
| `web_studio`            | Studio            | No-code customization tool               |
| `base_automation`       | Automated Actions | Trigger automated actions pada events    |
| `web_gantt`             | Gantt View        | Gantt chart view untuk planning          |
| `web_cohort`            | Cohort View       | Cohort analysis view                     |
| `web_map`               | Map View          | Geo-localized map view                   |

## 9. Integration & Technical

**IoT Box** - Hardware integration untuk devices **Barcode** - Barcode scanning operations **Studio** - Custom app builder tanpa coding (Enterprise)

| Technical Name       | Display Name         | Deskripsi                                   |
| -------------------- | -------------------- | ------------------------------------------- |
| `iot`                | IoT Box              | Connect hardware devices (printers, scales) |
| `hw_posbox_homepage` | POS IoT Box          | IoT Box untuk POS peripherals               |
| `barcodes`           | Barcode Nomenclature | Define barcode parsing rules                |

---


## MODUL WAJIB (Must-Have)

Modul ini foundational, hampir semua bisnis butuh:

**Kolaborasi Dasar:**

- `contacts` - Database customer/vendor/karyawan
- `mail` (Discuss) - Chat internal
- `calendar` - Kalender bersama

**Pilih Salah Satu untuk Penjualan:**

- `sale_management` - Untuk bisnis B2B (quotation, sales order)
- `website_sale` - Untuk toko online
- `point_of_sale` - Untuk retail/kasir

**Keuangan Dasar (Pilih Salah Satu):**

- `account_invoicing` - Invoice sederhana
- `account` - Accounting lengkap (kalau butuh laporan keuangan detail)

---

## MODUL OPTIONAL - Tergantung Jenis Bisnis

### A. Kalau Jual Barang Fisik

**Perlu Tambahan:**

- `stock` - Gudang dan inventory
- `purchase` - Beli barang dari supplier

**Dependencies:**

- `stock` butuh ada kalau pakai `point_of_sale`
- `purchase` sebaiknya pakai kalau sudah ada `stock`

---

### B. Kalau Ada Produksi/Manufaktur

**Perlu Tambahan:**

- `mrp` - Manufacturing (bikin produk dari bahan baku)

**Dependencies:**

- `mrp` butuh `stock` dan `purchase` sudah jalan dulu

**Optional Tambahan untuk Manufacturing:**

- `mrp_workorder` - Detail proses kerja (butuh `mrp`)
- `quality_control` - Quality check
- `maintenance` - Maintenance alat produksi

---

### C. Kalau Fokus ke Marketing

**Optional:**

- `website` - Website company
- `website_blog` - Blog (butuh `website`)
- `mass_mailing` - Email marketing
- `social_marketing` - Post ke social media

**Dependencies:**

- `website_blog` butuh `website` dulu
- `website_sale` butuh `website` + `sale_management`

---

### D. Kalau Bisnis Jasa/Project

**Optional:**

- `project` - Project management
- `hr_timesheet` - Catat jam kerja
- `sale_timesheet` - Invoice berdasarkan jam kerja (butuh `hr_timesheet` + `sale_management`)

---

### E. Untuk Sales & Customer Relationship

**Optional:**

- `crm` - Lead management (tracking calon customer)
- `sale_crm` - Link CRM ke Sales (butuh `crm` + `sale_management`)
- `sale_subscription` - Langganan bulanan/tahunan (butuh `sale_management`)

---

### F. Human Resources

**Optional:**

- `hr` - Database karyawan
- `hr_recruitment` - Rekrutmen
- `hr_holidays` - Cuti karyawan
- `hr_attendance` - Absensi
- `hr_payroll` - Gaji (ENTERPRISE, butuh `hr`)
- `hr_expense` - Reimburse karyawan

---

### G. Support & Helpdesk

**Optional:**

- `helpdesk` - Ticketing support (ENTERPRISE)
- `helpdesk_timesheet` - Catat waktu per ticket (butuh `helpdesk` + `hr_timesheet`)

---

### H. Fitur Advanced (ENTERPRISE)

**Optional - Untuk Bisnis Besar:**

- `marketing_automation` - Email otomatis (butuh `mass_mailing` + `crm`)
- `approvals` - Approval workflow
- `knowledge` - Wiki internal
- `documents` - Document management
- `sign` - Tanda tangan digital (butuh `documents`)
- `industry_fsm` - Field service (teknisi lapangan)
- `project_forecast` - Planning resource

## SUMMARY DEPENDENCIES

**Rantai Dependencies Umum:**

```
1. Bisnis Jual Barang:
   sale_management → stock → purchase → mrp (kalau produksi)

2. Bisnis Online:
   website → website_sale (perlu sale_management juga)

3. Marketing Full:
   website → mass_mailing → marketing_automation (perlu crm)

4. Sales Complete:
   crm → sale_management → sale_crm (link keduanya)

5. Project Billing:
   project → hr_timesheet → sale_timesheet (perlu sale_management)

6. HR Complete:
   hr → hr_payroll → hr_payroll_account (perlu account)
```



---
## 1. MASTER DATA TABLES

### `res_partner`

**Kegunaan:** Menyimpan semua "pihak" dalam sistem (customer, vendor, karyawan contact, company contact)

**Hubungan:**

- Dipakai oleh `sale_order` untuk mencatat siapa customernya
- Dipakai oleh `purchase_order` untuk mencatat siapa vendornya
- Dipakai oleh `account_move` untuk invoice/bill ke siapa
- Dipakai oleh `stock_picking` untuk delivery ke siapa
- Bisa self-reference: `parent_id` untuk struktur (company → contact person di bawahnya)

**Contoh Real:**
PT ABC (res_partner)
  ├─ Budi (contact person) → parent_id = PT ABC
  └─ Siti (contact person) → parent_id = PT ABC

---

### `res_users`
**Kegunaan:** User yang bisa login ke sistem

**Hubungan:**
- Link ke `res_partner` via `partner_id` (setiap user punya data contact)
- Dipakai oleh `sale_order.user_id` untuk track salesperson mana yang handle
- Dipakai oleh `purchase_order.user_id` untuk track purchaser
- Dipakai untuk permission dan access control

**Contoh Real:**
User "andi@company.com" 
  → punya partner_id = Andi (res_partner)
  → bisa bikin sales order sebagai salesperson

---

### `res_company`
**Kegunaan:** Data perusahaan (untuk multi-company setup)

**Hubungan:**
- Semua tabel transaksi punya `company_id`
- Link ke `res_partner` untuk alamat company
- Satu database bisa punya banyak company (group)

**Contoh Real:**
Company A di Jakarta
Company B di Surabaya
→ bisa pakai 1 Odoo database, data terpisah per company

---

### `product_template`
**Kegunaan:** Master produk (template/induk)

**Hubungan:**
- Parent dari `product_product` (1 template bisa punya banyak variant)
- Menyimpan info umum: nama, harga, kategori
- Link ke `product_category` untuk grouping

**Contoh Real:**
Template: "T-Shirt"
  ├─ Variant: T-Shirt Merah Size M
  ├─ Variant: T-Shirt Merah Size L
  └─ Variant: T-Shirt Biru Size M

---

### `product_product`
**Kegunaan:** Produk actual (variant dari template)

**Hubungan:**
- Child dari `product_template` via `product_tmpl_id`
- Dipakai di `sale_order_line` untuk item yang dijual
- Dipakai di `purchase_order_line` untuk item yang dibeli
- Dipakai di `stock_move` untuk track pergerakan barang

**Contoh Real:**
product_product.id = 123
  → product_tmpl_id = "T-Shirt"
  → SKU = "TSH-RED-M"
  → Barcode = "123456789"

---

## 2. SALES MODULE

### `sale_order`
**Kegunaan:** Header sales order/quotation

**Hubungan:**
- `partner_id` → siapa customer (res_partner)
- `user_id` → salesperson (res_users)
- Parent dari `sale_order_line` (1 SO punya banyak item)
- Generate `stock_picking` untuk delivery
- Generate `account_move` untuk invoice

**Flow:**
Customer pesan
  → Bikin sale_order (status: draft)
  → Confirm → jadi sales order (status: sale)
  → Trigger stock_picking untuk kirim barang
  → Trigger account_move untuk invoice

---

### `sale_order_line`
**Kegunaan:** Detail item per sales order

**Hubungan:**
- `order_id` → belongs to sale_order mana
- `product_id` → produk apa yang dijual
- Generate `stock_move` untuk item ini
- Generate `account_move_line` untuk invoice line

**Contoh Real:**
sale_order.name = "SO001"
  ├─ sale_order_line: Product A, qty 10, price 100rb
  └─ sale_order_line: Product B, qty 5, price 50rb
Total: 1.25 juta

---

## 3. PURCHASE MODULE

### `purchase_order`
**Kegunaan:** Header purchase order ke vendor

**Hubungan:**
- `partner_id` → vendor (res_partner)
- `user_id` → purchaser (res_users)
- Parent dari `purchase_order_line`
- Generate `stock_picking` untuk receive barang
- Generate `account_move` untuk vendor bill

**Flow:**
Butuh stock
  → Bikin purchase_order (status: draft)
  → Send ke vendor (status: sent)
  → Vendor confirm → jadi PO (status: purchase)
  → Terima barang → stock_picking
  → Terima bill → account_move

---

### `purchase_order_line`
**Kegunaan:** Detail item per purchase order

**Hubungan:**
- `order_id` → belongs to purchase_order mana
- `product_id` → produk apa yang dibeli
- Generate `stock_move` untuk receive item ini
- Generate `account_move_line` untuk vendor bill line

---

## 4. INVENTORY MODULE

### `stock_location`
**Kegunaan:** Lokasi gudang (warehouse, customer, vendor, transit)

**Hubungan:**
- Self-reference: `location_id` untuk hierarchy (Warehouse → Zone → Rack)
- Dipakai di `stock_move` untuk from/to location
- Ada tipe: internal (gudang), customer (keluar), supplier (masuk), transit

**Contoh Real:**
Warehouse Jakarta (parent)
  ├─ Zone A (location_id = Warehouse Jakarta)
  │   ├─ Rack 1
  │   └─ Rack 2
  └─ Zone B
      └─ Rack 3

Customer Location (virtual, untuk track barang keluar)
Vendor Location (virtual, untuk track barang masuk)

---

### `stock_picking`
**Kegunaan:** Dokumen perpindahan barang (delivery order, receipt)

**Hubungan:**
- `partner_id` → kirim ke/dari siapa (res_partner)
- `location_id` → dari lokasi mana
- `location_dest_id` → ke lokasi mana
- `sale_id` → kalau dari sales order
- `purchase_id` → kalau dari purchase order
- Parent dari `stock_move` (1 picking punya banyak item)

**Contoh Real:**
Delivery Order: DO001
  → sale_id = SO001
  → location_id = Warehouse Jakarta
  → location_dest_id = Customer Location
  → partner_id = PT ABC (customer)

---

### `stock_move`
**Kegunaan:** Pergerakan actual per produk

**Hubungan:**
- `picking_id` → belongs to stock_picking mana
- `product_id` → produk apa yang pindah
- `location_id` → dari lokasi mana
- `location_dest_id` → ke lokasi mana
- `sale_line_id` → kalau dari sales order line
- `purchase_line_id` → kalau dari purchase order line

**Contoh Real:**
stock_picking = DO001
  ├─ stock_move: Product A, 10 pcs, WH Jakarta → Customer
  └─ stock_move: Product B, 5 pcs, WH Jakarta → Customer

**Update inventory:**
- Ketika stock_move done, qty di lokasi berkurang/bertambah

---

## 5. ACCOUNTING MODULE

### `account_account`
**Kegunaan:** Chart of accounts (daftar rekening/akun)

**Hubungan:**
- Dipakai di `account_move_line` untuk debit/credit ke akun mana
- Link ke `account_account_type` untuk kategori (asset, liability, income, expense)

**Contoh Real:**
Code: 1110 - Cash in Bank
Code: 1120 - Account Receivable
Code: 4010 - Sales Revenue
Code: 5010 - Cost of Goods Sold

---

### `account_journal`
**Kegunaan:** Journal untuk grouping transaksi

**Hubungan:**
- Dipakai di `account_move` untuk categorize transaksi
- Ada tipe: sales (invoice), purchase (bill), cash, bank

**Contoh Real:**
Sales Journal → untuk customer invoice
Purchase Journal → untuk vendor bill
Bank Journal BCA → untuk transaksi bank BCA
Cash Journal → untuk petty cash

---

### `account_move`
**Kegunaan:** Header dokumen akuntansi (invoice, bill, payment, journal entry)

**Hubungan:**
- `partner_id` → invoice/bill ke siapa (res_partner)
- `journal_id` → masuk journal mana (account_journal)
- Parent dari `account_move_line` (1 invoice punya banyak line)
- Auto-generate dari `sale_order` (untuk invoice) atau `purchase_order` (untuk bill)

**Tipe:**
out_invoice → Customer Invoice
in_invoice → Vendor Bill
out_refund → Customer Credit Note
in_refund → Vendor Refund
entry → Manual Journal Entry

**Flow dari Sales:**
sale_order (SO001) confirmed
  → generate account_move (INV/2024/001)
    → move_type = out_invoice
    → partner_id = Customer

---

### `account_move_line`
**Kegunaan:** Detail per line di journal entry (debit/credit per account)

**Hubungan:**
- `move_id` → belongs to account_move mana
- `account_id` → debit/credit ke account mana
- `partner_id` → related to partner (untuk receivable/payable)
- `product_id` → kalau dari penjualan/pembelian produk

**Contoh Real:**
Invoice INV001 total 1 juta
account_move_line:
  ├─ Account Receivable (1110) → Debit 1,000,000
  └─ Sales Revenue (4010) → Credit 1,000,000

**Double Entry:**
- Setiap transaksi, total debit = total credit
- Account receivable naik (debit) = revenue naik (credit)

---

## 6. HR MODULE

### `hr_department`
**Kegunaan:** Departemen dalam organisasi

**Hubungan:**
- Self-reference: `parent_id` untuk hierarchy (HQ → Regional → Branch)
- `manager_id` → siapa head of department (hr_employee)
- Dipakai di `hr_employee` untuk assign ke department

**Contoh Real:**
IT Department (parent)
  ├─ Development Team
  └─ Infrastructure Team

Sales Department (parent)
  ├─ Direct Sales
  └─ Online Sales

---

### `hr_employee`
**Kegunaan:** Data karyawan

**Hubungan:**
- `user_id` → kalau karyawan ini punya akses login (res_users)
- `department_id` → di department mana (hr_department)
- `parent_id` → siapa managernya (hr_employee)
- Self-reference untuk organization chart

**Contoh Real:**
Budi (Director)
  ├─ Andi (Manager) → parent_id = Budi
  │   ├─ Deni (Staff) → parent_id = Andi
  │   └─ Eka (Staff) → parent_id = Andi
  └─ Citra (Manager) → parent_id = Budi

---

## RELATIONSHIP SUMMARY

### Customer Order Flow (End-to-End)
1. Customer (res_partner)
     ↓
2. Bikin Sales Order (sale_order)
     ├─ sale_order_line (item A, B, C)
     ↓
3. Confirm → Generate Delivery (stock_picking)
     ├─ stock_move (pindah Product A dari WH → Customer)
     ├─ stock_move (pindah Product B dari WH → Customer)
     ↓
4. Validate Delivery → Generate Invoice (account_move)
     ├─ account_move_line (Debit: Receivable)
     └─ account_move_line (Credit: Revenue)
     ↓
5. Customer bayar → Payment (account_move)
     ├─ account_move_line (Debit: Bank)
     └─ account_move_line (Credit: Receivable)

### Purchase Flow (End-to-End)
1. Vendor (res_partner)
     ↓
2. Bikin Purchase Order (purchase_order)
     ├─ purchase_order_line (item X, Y)
     ↓
3. Confirm → Generate Receipt (stock_picking)
     ├─ stock_move (pindah Product X dari Vendor → WH)
     ├─ stock_move (pindah Product Y dari Vendor → WH)
     ↓
4. Validate Receipt → Generate Bill (account_move)
     ├─ account_move_line (Debit: Expense/COGS)
     └─ account_move_line (Credit: Payable)
     ↓
5. Bayar vendor → Payment (account_move)
     ├─ account_move_line (Debit: Payable)
     └─ account_move_line (Credit: Bank)