# BCC Safety Web Application v4 — Footer Enhanced

ฟีเจอร์หลัก:
- Font หลัก: `TH Sarabun New` และ fallback เป็น Google Font `Sarabun`
- เพิ่ม / ลบ / เลือกดูข้อมูลแยกตามฝ่าย
- Real-time Sync ผ่าน Cloudflare Workers + Durable Objects + WebSocket
- Export JSON และ Export รูป PNG
- Footer แบบใหม่ แสดงผู้จัดทำ Siriphan พร้อมรายละเอียดระบบ เวอร์ชัน และเทคโนโลยี

## Footer v4

Footer ใหม่ประกอบด้วย:
- ชื่อระบบ: BCC Safety Web Application
- คำอธิบาย: Interactive Safety Record Dashboard
- ผู้จัดทำ: Siriphan
- บทบาท: IT Officer / Web Application Developer
- Version 4.0
- Cloudflare Workers + Real-time Sync
- Export PNG / JSON
- © 2026 Bangkok Cable

## โครงสร้างไฟล์ที่ต้องอยู่ที่ Root ของ GitHub repo

```text
.github/workflows/deploy-cloudflare.yml
package.json
wrangler.toml
src/worker.js
README.md
```

## GitHub Secrets ที่ต้องมี

```text
CLOUDFLARE_API_TOKEN
CLOUDFLARE_ACCOUNT_ID
```

## Deploy

Push เข้า branch `main` หรือกด Run workflow ใน GitHub Actions
