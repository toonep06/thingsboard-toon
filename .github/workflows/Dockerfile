# ใช้ base image ของ OpenJDK
FROM openjdk:17-jdk-slim

# ตั้งค่าตัวแปรสภาพแวดล้อม
ENV JAVA_HOME /usr/lib/jvm/java-17-openjdk-amd64
ENV PATH $JAVA_HOME/bin:$PATH

# สร้าง directory สำหรับแอปพลิเคชัน
WORKDIR /app

# คัดลอกไฟล์ที่ดาวน์โหลดมาที่ container
COPY thingsboard.jar /app/thingsboard.jar

# กำหนด command เพื่อรันแอปพลิเคชัน
ENTRYPOINT ["java", "-jar", "/app/thingsboard.jar"]
