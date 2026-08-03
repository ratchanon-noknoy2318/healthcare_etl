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

## วิธีใช้งาน

1. เปิด **เปิดเมนู SQL Editor หรือคลิกไอคอนรูปสายฟ้า** หรือเครื่องมือที่ใช้เชื่อมต่อฐานข้อมูล HOSxP  
3. เปิดไฟล์ SQL ที่ต้องการ เช่น:
   - `export_village.sql`
   - `export_allergy.sql`
3. กด **Run** เพื่อรัน script  
4. ผลลัพธ์จะได้เป็นตารางข้อมูล สามารถ export ออกเป็น **CSV / Excel / JSON** ได้ตามต้องการ  

> 💡 แนะนำให้ใช้สิทธิ์ **read-only account** ในการเชื่อมต่อฐานข้อมูล เพื่อความปลอดภัยของข้อมูลผู้ป่วย
