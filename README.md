# BCC Safety Interactive Dashboard — GitHub + Cloudflare Workers

Dashboard สำหรับ Safety Record / Accident Record พร้อมแก้ไขข้อมูลแบบ Real-time ข้ามหลายเครื่อง ผ่าน Cloudflare Workers + Durable Objects + WebSocket

## Deploy ผ่าน GitHub Actions

1. สร้าง GitHub repository ใหม่ เช่น `bcc-safety-dashboard`
2. Upload ไฟล์ทั้งหมดใน ZIP นี้ขึ้น repository
3. ไปที่ Cloudflare Dashboard > My Profile > API Tokens > Create Token
4. เลือก Template: **Edit Cloudflare Workers** หรือสร้าง Custom Token ที่มีสิทธิ์ Workers Scripts Edit สำหรับ Account
5. ไปที่ GitHub Repository > Settings > Secrets and variables > Actions > New repository secret
6. ตั้งชื่อ secret เป็น `CLOUDFLARE_API_TOKEN` แล้ววางค่า Token
7. ไปที่แท็บ Actions แล้ว Run workflow หรือ push เข้า branch `main`

## ไฟล์สำคัญ

```text
.github/workflows/deploy-cloudflare.yml
package.json
wrangler.toml
src/worker.js
```

## ทดสอบ Local

```bash
npm install
npm run dev
```

## Deploy Manual

```bash
npm install
npx wrangler login
npm run deploy
```
