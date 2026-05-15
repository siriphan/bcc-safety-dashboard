# BCC Safety Web Application v2 — แยกตามฝ่าย

เวอร์ชันนี้ปรับเป็น Web Application พร้อมฟีเจอร์:

- Font หลัก: `TH Sarabun New` และ fallback เป็น Google Font `Sarabun`
- เพิ่ม / ลบ / เลือกดูข้อมูลแยกตามฝ่าย
- แต่ละฝ่ายมี Safety Record และ Accident Record แยกกัน
- Real-time Sync ผ่าน Cloudflare Workers + Durable Objects + WebSocket
- โครงสร้างไฟล์ถูกต้อง มี `src/worker.js` เพื่อแก้ปัญหา entry-point not found

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

## ทดสอบบนเครื่อง

```bash
npm install
npm run dev
```

## Manual deploy

```bash
npm install
npx wrangler deploy
```
