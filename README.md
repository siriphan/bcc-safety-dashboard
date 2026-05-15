# BCC Safety Web Application v11 — Manual Number Edit

ปรับปรุงตามคำขอ:
- รวม Header + Logo + ชื่อบริษัท/ฝ่าย + Safety First + Title Bar Image ให้เป็น Layout เดียวกันตามภาพตัวอย่าง
- Logo ซ้ายบนใช้พื้นที่เดียวกับ Header
- ชื่อบริษัทและชื่อฝ่ายอยู่กึ่งกลางแบบเดียวกับภาพตัวอย่าง
- Safety First อยู่ขวาบนแบบวงกลม
- Title Bar ใช้รูปภาพเอกสารแนบ และจัดเต็มความกว้างด้านล่าง Header
- คง Logic v8/v9: วันอนาคต = ว่าง, Auto Green เฉพาะ 1/1/2566 ถึงปัจจุบัน
- Export PNG แนวตั้งยังมี Logo และ Title Bar Image

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


## เพิ่มใน v11

- แก้ไขช่องตัวเลขแบบ Manual ได้
- ช่อง `OPERATED WITHOUT A LOST TIME ACCIDENT (DAYS)` สามารถพิมพ์เลขเองได้
- ช่อง `THE BEST RECORD (DAYS)` สามารถพิมพ์เลขเองได้
- ค่าที่พิมพ์เองจะถูกบันทึกแยกตามฝ่ายและ Sync แบบ Real-time
- เมื่อ Reset ฝ่ายนี้ ระบบจะล้างค่า Manual Override ของฝ่ายนั้นด้วย
