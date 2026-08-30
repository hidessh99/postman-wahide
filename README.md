# 🌐 Wahide REST API Collection (OpenCollection / Bruno / Postman)

Official API collection for **Wahide (Enterprise SaaS WhatsApp Multi-Tenant Gateway)**.

---

## 📂 Struktur Modul API

```text
.
├── opencollection.yml
├── 00-health/                 # Liveness, Readiness, Health Checks
├── 01-iam/                    # Auth, Users, Address, Agents, Admin RBAC
├── 02-subscription/           # Plans, Tenant Subscription, Webhook
├── 03-whatsapp/               # Device Slot CRUD, QR Pairing, Instant Messages, Meta Cloud API
├── 04-campaign/               # Broadcast Campaigns, Start, Message Audit Logs
├── 05-contact/                # Phonebook Contacts, Bulk Import, Audience Tags
├── 06-finance/                # Billing Orders, Invoices, Vouchers, Reports, Payment Webhooks
├── 07-content/                # CMS Posts, Settings, S3/R2 Presigned Uploads
├── 08-support/                # Helpdesk Tickets, Attachments, Resolution Replies
├── 09-notification/           # Async Notification Queue, System Broadcasts
└── 10-cronjob/                # 15 Enterprise Cronjob Endpoints (X-Cron-Secret)
```

---

## 🚀 Cara Penggunaan

### 1. Menggunakan Bruno / Yaak (OpenCollection)
1. Buka aplikasi **Bruno** atau **Yaak**.
2. Pilih **Open Collection** dan arahkan ke folder ini.
3. Atur environment variables:
   - `baseUrl`: `http://localhost:3030` (atau URL server Anda)
   - `token`: `<JWT_TOKEN_OR_API_KEY>`
   - `cronSecret`: `wahide_cron_secret_2026`

### 2. Menggunakan Postman
1. Import folder atau konversi `opencollection.yml` ke Postman Collection format.
