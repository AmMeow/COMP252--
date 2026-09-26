# Laundry Delivery System (ระบบบริหารจัดการและจัดส่งซักรีด)

วิชา: COMP342 วิศวกรรมซอฟต์แวร์เบื้องต้น (Software Engineering)
ใบงานที่ 4: Implementation + Git

## เกี่ยวกับโปรเจกต์ (Project Overview)
Laundry Delivery System เป็นเว็บแอปพลิเคชันสำหรับการบริหารจัดการบริการซักรีดแบบครบวงจร ช่วยอำนวยความสะดวกให้ลูกค้าสามารถสั่งซักผ้า ระบุตำแหน่งที่อยู่ ชำระเงิน และติดตามสถานะการรับ-ส่งผ้าแบบเรียลไทม์ พร้อมระบบจัดการงานสำหรับพนักงานและผู้ดูแลระบบ

## เทคโนโลยีที่ใช้ (Tech Stack)
- **Language & Framework:** Python 3 (Flask Framework)
- **Front-end:** HTML5, CSS3, JavaScript, Bootstrap 5
- **Database:** SQLite
- **Version Control:** Git & GitHub

## โครงสร้างโฟลเดอร์โปรเจกต์ (Directory Structure)
```text
laundry-delivery-system/
├── docs/                   # เอกสารรายงานการวิเคราะห์และออกแบบระบบ (Lab 1 - Lab 3)
│   ├── srs.md
│   └── design.md
├── src/                    # ซอร์สโค้ดหลักของระบบ
│   ├── app.py              # ไฟล์หลักสำหรับรัน Flask Application
│   ├── models.py           # Data Models (Customer, Order, Payment, Delivery)
│   ├── routes/             # Controller / Route Handlers
│   │   ├── auth.py         # โมดูลระบบสมาชิกและการยืนยันตัวตน
│   │   ├── order.py        # โมดูลรายการสั่งซื้อและการชำระเงิน
│   │   └── delivery.py     # โมดูลติดตามและอัปเดตการจัดส่ง
│   ├── static/             # ไฟล์ CSS, JS และ รูปภาพ
│   └── templates/          # หน้าจอ HTML (Views)
├── tests/                  # สคริปต์สำหรับการทดสอบระบบ (Lab 5)
│   └── test_order.py
├── .gitignore
├── README.md
└── requirements.txt

## สมาชิกในทีมและการแบ่งงาน (Team Members & Roles)
1. **นายมาร์ค (Project Manager / Full-stack Developer)**
   - ดูแลภาพรวม Git Repository และตั้งโครงสร้างโปรเจกต์
   - พัฒนาโมดูลระบบสมัครสมาชิกและล็อกอิน (`Customer` / Auth Module)
   - พัฒนาหน้าจอ Dashboard ฝั่งลูกค้า
2. **นายเบสท์ (Backend Developer / Database Admin)**
   - ออกแบบ schema ฐานข้อมูล SQLite
   - พัฒนาระบบสั่งซื้อ ค้นหา/เลือกบริการ และคำนวณราคา (`Order` & `Service` Module)
   - พัฒนาระบบจัดการการชำระเงิน (`Payment` Module)
3. **นายอัน (System Analyst / QA & Developer)**
   - พัฒนาระบบติดตามและอัปเดตสถานะการรับ-ส่งผ้า (`Delivery` Module)
   - พัฒนาหน้าจอสำหรับพนักงานซักรีดและพนักงานจัดส่ง
   - พัฒนาหน้าจัดการสำหรับผู้ดูแลระบบ (Admin Panel)

## ขั้นตอนการติดตั้งและรันโปรเจกต์ (Getting Started)
1. Clone Repository นี้ลงเครื่อง local:
   ```bash
git clone https://github.com/AmMeow/COMP252--.git
