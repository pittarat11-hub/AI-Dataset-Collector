# AI Dataset Collector — GitHub Only

เว็บเก็บภาพชิ้นงาน 3 มุม Front / Middle / Back โดยไม่ใช้ฐานข้อมูลภายนอก

## วิธีใช้งาน

1. Upload ไฟล์ทั้งหมดขึ้น GitHub Repository
2. เปิด GitHub Pages
3. เปิดเว็บไซต์บน iPad
4. กรอกชื่อพนักงานและชื่อ Part
5. ถ่าย Front / Middle / Back
6. กด "บันทึก Dataset"
7. เข้า Gallery
8. กด "ดาวน์โหลดทั้งหมด ZIP"

## สำคัญ

เวอร์ชันนี้ใช้ Browser Local Storage:
- ข้อมูลอยู่ใน Browser ของเครื่องที่บันทึก
- ไม่ส่งข้อมูลไป Server
- ไม่ต้องใช้ Supabase
- ไม่ต้องมี PHP
- GitHub Pages ใช้เป็นที่โฮสต์เว็บเท่านั้น

หากล้างข้อมูลเว็บไซต์/Browser ข้อมูลอาจหาย จึงควรดาวน์โหลด ZIP สำรองเป็นระยะ

## ZIP Dataset

โครงสร้าง:

Part_Name/
  front/
  middle/
  back/
metadata.csv

เหมาะสำหรับนำภาพไปจัด Dataset ต่อใน Roboflow หรือใช้กับ Python/PyTorch

## GitHub Pages

Repository > Settings > Pages > Deploy from branch > main > / (root) > Save

## Camera

บน iPad/iPhone/Android ปุ่มถ่ายภาพใช้ HTML file input + camera capture ของอุปกรณ์
ควรเปิดเว็บผ่าน HTTPS ซึ่ง GitHub Pages รองรับ

## หมายเหตุเรื่องพื้นที่

รูปจะถูกเก็บเป็นข้อมูลใน Browser และใช้พื้นที่ของเครื่อง หากมีภาพจำนวนมาก ควรดาวน์โหลด ZIP ออกมาเป็นระยะ และลบข้อมูลเก่าจาก Gallery หลังจากสำรองแล้ว
