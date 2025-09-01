# ใช้ Python 3.12 รุ่น slim
FROM python:3.12-slim

# กำหนดโฟลเดอร์ทำงาน
WORKDIR /app

# คัดลอก requirements.txt มาก่อนเพื่อลดการ build ใหม่เมื่อโค้ดเปลี่ยน
COPY requirements.txt .

# ติดตั้ง dependency
RUN pip install -r requirements.txt

# คัดลอกโค้ดทั้งหมดในโฟลเดอร์ scheduler ไปยัง /app
COPY . .

# คำสั่งรัน scheduler เมื่อ container เริ่ม
CMD ["python3", "scheduler.py"]
