# HOSxP เวอร์ชัน 3.66.11.00

SQL scripts สำหรับการดึงข้อมูลจาก **HOSxP version 3.66.11.00**  
ใช้เพื่อการศึกษา/งานวิจัย (Non-commercial use only) เช่น การ export ข้อมูลผู้ป่วย, OPD, Telemedicine, Drug allergy และอื่น ๆ

---
 
## รายการสคริปต์ที่พร้อมใช้งาน

- export_buddycare.sql → ดึงข้อมูลไปใช้กับระบบ BuddyCare

- masked_patient.sql → สร้าง JSON ข้อมูลผู้ป่วยแบบ masked

- export_allergy.sql → รายงานประวัติการแพ้ยา

- export_dtx.sql → ข้อมูล DTX records

- export_service_cost.sql → ค่าใช้จ่ายการรักษา

- export_daily_visit.sql → รายงานการเข้ารับบริการรายวัน

- export_telemedicine.sql → รายชื่อผู้ป่วย telemedicine

- export_village.sql → รายชื่อหมู่บ้าน

---
# โครงสร้างตารางฐานข้อมูล HOSxP

## ตารางเกี่ยวกับสิทธิการรักษาและข้อมูลพื้นฐาน

| ตาราง | รายละเอียด |
|-------|-------------|
| pttype | ข้อมูลสิทธิการรักษาของผู้ป่วย |
| occupation | ข้อมูลอาชีพของผู้ป่วย |
| religion | ข้อมูลศาสนาของผู้ป่วย |

---

## ตารางเกี่ยวกับ OPD (ผู้ป่วยนอก)

| ตาราง | รายละเอียด |
|-------|-------------|
| patient | ข้อมูลทั่วไปของผู้ป่วย |
| ovst | ข้อมูลการเข้ารับบริการ (Visit) |
| vn_stat | ข้อมูล Visit และค่าใช้จ่ายที่เกี่ยวข้อง |
| opdscreen | ข้อมูลการคัดกรองผู้ป่วย |
| ovstdiag | ข้อมูลผลการตรวจรักษาและการวินิจฉัย |
| ptcardno | ข้อมูลเลขบัตรประชาชนผู้ป่วย |
| pttypeno | ข้อมูลเลขที่สิทธิการรักษาและรายละเอียดสิทธิ |
| occupation | ข้อมูลอาชีพ |
| pttype | ข้อมูลประเภทสิทธิการรักษา |
| spclty | ข้อมูลแผนก/สาขาการรักษา |
| kskdepartment | ข้อมูลจุดส่งตรวจ ห้องตรวจ และหน่วยบริการ |
| thaiaddress | ข้อมูลที่อยู่ผู้ป่วย (ตำบล อำเภอ จังหวัด) |

---

## วิธีใช้งาน

1. เปิด **เปิดเมนู SQL Editor (ไอคอนรูปสายฟ้า)** หรือเครื่องมือที่ใช้เชื่อมต่อฐานข้อมูล HOSxP  
3. เปิดไฟล์ SQL ที่ต้องการ เช่น:
   - `export_village.sql`
   - `export_allergy.sql`
3. กด **Run** เพื่อรัน script  
4. ผลลัพธ์จะได้เป็นตารางข้อมูล สามารถ export ออกเป็น **CSV / Excel / JSON** ได้ตามต้องการ  

> แนะนำให้ใช้สิทธิ์ **read-only account** ในการเชื่อมต่อฐานข้อมูล เพื่อความปลอดภัยของข้อมูลผู้ป่วย

---

## ผู้พัฒนา (Author)

- **ชื่อ:** รัชชานนท์ นกน้อย  
- **ตำแหน่ง:** นักวิชาการคอมพิวเตอร์  
- **GitHub:** [ratchanon-noknoy2318](https://github.com/ratchanon-noknoy2318)  
- **LinkedIn:** [linkedin.com/in/ratchanon-noknoy](https://linkedin.com/in/ratchanon-noknoy)



