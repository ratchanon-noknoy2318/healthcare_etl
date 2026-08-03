# HOSxP เวอร์ชัน 3.66.11.00

SQL scripts สำหรับการดึงข้อมูลจาก **HOSxP version 3.66.11.00**  
ใช้เพื่อการศึกษา/งานวิจัย (Non-commercial use only) เช่น การ export ข้อมูลผู้ป่วย, OPD, Telemedicine, Drug allergy และอื่น ๆ

---
 
## Available Scripts

- Export_hosxp_to_buddycare.sql → ดึงข้อมูลไปใช้กับระบบ BuddyCare

- Export_masked_patient_json.sql → สร้าง JSON ข้อมูลผู้ป่วยแบบ masked

- Export_patient_drug_allergy.sql → รายงานประวัติการแพ้ยา

- Export_patient_dtx_records.sql → ข้อมูล DTX records

- Export_patient_service_cost.sql → ค่าใช้จ่ายการรักษา

- Export_patient_visit_daily.sql → รายงานการเข้ารับบริการรายวัน

- Export_telemedicine_patients.sql → รายชื่อผู้ป่วย telemedicine

- Export_village_list.sql → รายชื่อหมู่บ้าน

---

## How to Use

1. เปิด **เปิดเมนู SQL Editor หรือคลิกไอคอนรูปสายฟ้า** หรือเครื่องมือที่ใช้เชื่อมต่อฐานข้อมูล HOSxP  
3. เปิดไฟล์ SQL ที่ต้องการ เช่น:
   - `Export_patient_visit_daily.sql`
   - `Export_patient_drug_allergy.sql`
3. กด **Run** เพื่อรัน script  
4. ผลลัพธ์จะได้เป็นตารางข้อมูล สามารถ export ออกเป็น **CSV / Excel / JSON** ได้ตามต้องการ  

> 💡 แนะนำให้ใช้สิทธิ์ **read-only account** ในการเชื่อมต่อฐานข้อมูล เพื่อความปลอดภัยของข้อมูลผู้ป่วย
