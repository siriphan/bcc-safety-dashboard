# BCC Safety Web Application v6

ปรับปรุงตามคำขอล่าสุด:
- แก้ปัญหา Show เดือนภาษาไทยไม่เต็ม โดยขยายช่องเดือนและปรับ layout ฝั่ง Accident Record
- Export รูป PNG เป็นแนวตั้ง Portrait โดยจัดลำดับข้อมูลเป็น:
  1. ข้อมูลฝ่าย
  2. สถิติความปลอดภัย
  3. สถิติความปลอดภัยประจำเดือน
- Export Portrait ไม่จับทั้งหน้าจอแนวนอนแล้ว แต่สร้างหน้า Export เฉพาะสำหรับรายงานแนวตั้ง
- ยังมี Login, เพิ่มฝ่าย, ลบฝ่าย, Real-time Sync, Export JSON, Footer ผู้จัดทำ Siriphan

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

## GitHub Secrets
```text
CLOUDFLARE_API_TOKEN
CLOUDFLARE_ACCOUNT_ID
```
