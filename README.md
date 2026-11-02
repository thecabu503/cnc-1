# ระบบประเมินผลบุคลากร CNC ประจำปี 2026 (เฉพาะพนักงานประจำ ครบทั้ง 4 ระดับ ➔ อัตราส่วน 20% + QR Code รายบุคคล 57 คน)

ชุดโค้ดสำหรับอัปโหลดขึ้น **GitHub Pages** (`https://thecabu503.github.io/cnc-1/`) เชื่อมต่อกับ **Google Sheets** และซิงก์ 24 ชม. ลงไฟล์ **Master บน Server ไดรฟ์ `L:\`** (`\\ehdata4.eandh.co.th\data\Lpd-data\LPD-Document-(NOT Sharing)\5.GROUP-SUPERVISOR\12.Takuya\CNC_Evaluation_Master_2026`)

## ผังสายการประเมินผลครบทั้ง 4 ระดับ (เฉพาะพนักงานประจำ รวม 57 คน)
1. **Technician พนักงานประจำ (38 คน: CNC-1 = 20, CNC-2 = 18)** ➔ ประเมินโดย **Leader / Ass. / Sup.** (แบบฟอร์ม `T-xxxxx` 34 ข้อ / เต็ม 80 คะแนน ➔ อัตราส่วน 20%)
2. **Leader พนักงานประจำ (13 คน: CNC-1 = 7, CNC-2 = 6)** ➔ ประเมินโดย **Ass. / Sup.** (แบบฟอร์ม `L-xxxxx` 15 ข้อ / เต็ม 80 คะแนน ➔ อัตราส่วน 20%)
3. **Ass. / Asst. Supervisor พนักงานประจำ (4 คน: CNC-1 = 2, CNC-2 = 2)** ➔ ประเมินโดย **Sup. (Supervisor: Anurak, Takuya, Varitthon)** (แบบฟอร์ม `As-xxxxx` 15 ข้อ / เต็ม 80 คะแนน ➔ อัตราส่วน 20%)
4. **Engineer พนักงานประจำ (2 คน: CNC-1 = Sakkarin `01896`, CNC-2 = Weerapat `01939`)** ➔ ประเมินโดย **Sup. (Supervisor: Anurak, Takuya, Varitthon)** (แบบฟอร์ม `E-xxxxx` 15 ข้อ / เต็ม 80 คะแนน ➔ อัตราส่วน 20%)

## โครงสร้างไฟล์ในโฟลเดอร์ GitHub นี้
1. **`index.html`** — หน้าเว็บให้คะแนนประเมินออนไลน์ครบทั้ง 4 ระดับ (เต็ม 80 คะแนน ➔ คำนวณอัตราส่วน 20% อัตโนมัติ) เชื่อมต่อ Google Sheet อัตโนมัติเบื้องหลัง รองรับการสแกน QR Code รายบุคคล (`?role=...&zone=...&emp=...`)
2. **`qr_table.html`** — ตารางรวม QR Code รายบุคคลครบทั้ง **57 คน** (กรองแยกตามระดับตำแหน่งและโซน `CNC-1` / `CNC-2` ได้ทันที พร้อมพิมพ์กระดาษ A4)
3. **`google_apps_script/Code.gs`** — โค้ดหลังบ้านสำหรับวางใน Google Sheets เพื่อรับข้อมูลคะแนนครบทั้ง 4 ระดับแบบ Real-time
