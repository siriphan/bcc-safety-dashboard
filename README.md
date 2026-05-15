# BCC Safety Web Application v5

เพิ่มตามคำขอ:
- หน้า Login: User `BCC`, Password `Siriphan.m`
- Safety Record คำนวณจากข้อมูล Accident Record รายเดือน
- เลือกวันที่แสดงผลได้ โดยเริ่มปี พ.ศ. 2565
- ปรับสีสันเข้มขึ้น โทน Navy Blue / Electric Blue
- Title bar สไตล์ตามเอกสารแนบ: แถบสีน้ำเงินเข้ม พร้อมลายเมือง/พลังงาน/เส้นแสง
- ยังมี Export PNG, Export JSON, เพิ่มฝ่าย, ลบฝ่าย, Real-time Sync และ Footer ผู้จัดทำ Siriphan

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
