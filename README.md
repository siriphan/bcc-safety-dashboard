# BCC Safety Web Application v7

ปรับปรุงตามคำขอล่าสุด:
- เพิ่ม Logo BCC ด้านซ้ายบนตามเอกสารแนบ โดยฝังภาพไว้ใน Worker แล้ว
- ลบเมนู/Title Bar ข้อความ `BCC Safety Record Web Application / Blue City / Energy Theme`
- สถิติความปลอดภัยประจำเดือนสามารถเลือกเดือน/ปีที่จะแสดงได้ แยกจากวันที่คำนวณ Safety Record
- Auto Update สีเขียว `วันทำงานที่ไม่เกิดอุบัติเหตุ` ตั้งแต่ 1/1/2566 ถึงวันที่ปัจจุบัน ถ้ายังไม่ได้กำหนดสีอื่น
- เดือนภาษาไทยแสดงเต็มขึ้น โดยขยายช่องแสดงเดือน
- Export PNG แนวตั้งยังเรียงลำดับ: ข้อมูลฝ่าย > สถิติความปลอดภัย > สถิติความปลอดภัยประจำเดือน

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
