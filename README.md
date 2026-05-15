# BCC Safety Web Application v3 — Export รูป PNG + แยกตามฝ่าย

ฟีเจอร์หลัก:
- Font หลัก: `TH Sarabun New` และ fallback เป็น Google Font `Sarabun`
- เพิ่ม / ลบ / เลือกดูข้อมูลแยกตามฝ่าย
- แต่ละฝ่ายมี Safety Record และ Accident Record แยกกัน
- Real-time Sync ผ่าน Cloudflare Workers + Durable Objects + WebSocket
- Export ข้อมูล JSON
- Export หน้าจอเป็นรูปภาพ PNG
- Footer ด้านล่าง: `Web Application ผู้จัดทำ: Siriphan`

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

## ทดสอบ Local

```bash
npm install
npm run dev
```
