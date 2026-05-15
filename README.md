# BCC Safety Web Application v9

ปรับปรุงตามคำขอ:
- แก้ไข Title Bar ให้ใช้รูปภาพจากเอกสารแนบ `KV New Slogan LinkedIn.jpg`
- ฝัง Title Bar Image ใน Worker เป็น Base64 ไม่ต้องอัปโหลดไฟล์รูปแยก
- คง Logic v8: วันอนาคต = ว่าง, Auto Green เฉพาะ 1/1/2566 ถึงปัจจุบัน
- Logo BCC ด้านซ้ายบนยังอยู่
- Export PNG แนวตั้งใส่ Title Bar Image ในหัวรายงานด้วย

## Login
User: `BCC`
Password: `Siriphan.m`

## โครงสร้างไฟล์ที่ต้องอยู่ที่ root ของ GitHub repo
```text
.github/workflows/deploy-cloudflare.yml
package.json
wrangler.toml
src/worker.js
README.md
```
