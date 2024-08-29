# # Select Image openjdk:17-jdk-slim
# FROM openjdk:17-jdk-slim
# FROM maven:3.8.4-openjdk-17-slim
# # FROM maven:3.9.6-eclipse-temurin-17
# # FROM maven:3.9.6-eclipse-temurin-17-slim
# # RUN apt-get update && apt-get install -y maven

# # config directory
# WORKDIR /SpringAPI/app

# # Coppy all flie
# COPY . .

# # Build Code
# RUN mvn clean package -DskipTests
# # RUN mvn package

# # Config Port
# EXPOSE 8080

# # Command run Application Spring
# # ENTRYPOINT [ "java", "-jar", "/SpringAPI/app/target/spring-store-api-0.0.1-SNAPSHOT.jar"]
# ENTRYPOINT ["java","-jar","./SpringAPI/app/target/springboot-store-api-0.0.1-SNAPSHOT.jar"]

# เลือก Image ที่จะใช้ ในที่นี้เลือกใช้ openjdk:17-jdk-slim , 3maven:3.8.4-openjdk-17-slim
# FROM openjdk:17-jdk-slim
# FROM maven:3.8.4-openjdk-17-slim

# # กำหนด directory ที่เราจะใช้เก็บโค้ดของเรา
# WORKDIR /SpringAPI/app

# # คัดลอกไฟล์ทั้งหมดไปยัง container
# COPY . .

# # Build โค้ดของเรา
# RUN mvn clean package -DskipTests

# # กำหนด port ที่เราจะใช้
# EXPOSE 8080


# เลือก Image ที่จะใช้ ในที่นี้เลือกใช้ openjdk:17-jdk-slim , 3maven:3.8.4-openjdk-17-slim
FROM openjdk:17-jdk-slim
FROM maven:3.8.4-openjdk-17-slim

# กำหนด directory ที่เราจะใช้เก็บโค้ดของเรา
WORKDIR /SpringAPI/app

# คัดลอกไฟล์ทั้งหมดไปยัง container
COPY . .

# Build โค้ดของเรา
RUN mvn clean package -DskipTests
# RUN mvn clean package

# กำหนด port ที่เราจะใช้
EXPOSE 8080

# คำสั่งรัน Application Spring
ENTRYPOINT ["java","-jar","/SpringAPI/app/target/spring-store-api-0.0.1-SNAPSHOT.jar"]