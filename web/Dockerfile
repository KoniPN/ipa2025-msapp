# ใช้ Python 3.12 รุ่น slim เพื่อลดขนาด image
FROM python:3.12-slim

# กำหนดโฟลเดอร์ทำงานใน container
WORKDIR /app

# คัดลอกไฟล์ทั้งหมดในโฟลเดอร์ web ไปยัง /app
COPY . /app

# ติดตั้ง dependency ตาม requirements.txt
RUN pip install -r requirements.txt

# เปิดพอร์ต 8080 ให้บริการ Flask
EXPOSE 8080

# คำสั่งเริ่มต้นเมื่อ container ทำงาน
CMD ["python3", "app.py"]
