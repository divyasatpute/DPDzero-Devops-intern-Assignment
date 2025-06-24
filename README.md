# 🚀 DPDzero DevOps Intern Assignment: Nginx Reverse Proxy with Docker Compose

👩‍💻 **Author:** Divya V. Satpute  
🎯 **Role:** DevOps Intern at DPDzero

---

## 📌 Project Overview

This assignment demonstrates:

- 🐳 Containerizing Go and Python microservices
- 🔁 Exposing them via Nginx reverse proxy
- 📦 Running everything using Docker Compose
- ☁️ Optionally deploying to AWS EC2

---

## 📁 Project Folder Structure
├── docker-compose.yml

├── nginx/

│ └── nginx.conf

├── service_1/

│ ├── Dockerfile

│ └── main.go

├── service_2/

│ ├── Dockerfile

│ ├── app.py

│ └── requirements.txt



## 🧪 Build & Run
🔹 Build and run containers
### docker-compose up --build -d
This command builds and launches all services in detached mode.

## ✅ Testing the Services
### 🔹 Direct service check:
curl http://localhost:8001/hello
curl http://localhost:8002/hello
### 🔹 Via Nginx reverse proxy:

curl http://localhost:8080/service1/hello
curl http://localhost:8080/service2/hello
## ✅ You should get:

{"message": "Hello from Service 1"}
{"message": "Hello from Service 2"}


### docker-compose up --build -d
## In your browser, visit:


http://<your-ec2-ip>:8080/service1/hello
http://<your-ec2-ip>:8080/service2/hello
### 📊 Health Check (Optional Debugging)
### To verify if containers are healthy:

docker inspect --format='{{json .State.Health}}' service1-container
docker inspect --format='{{json .State.Health}}' service2-container
## 📚 Key Learnings
✅ Dockerizing Go and Flask apps
✅ Docker Compose orchestration
✅ Nginx reverse proxy configuration
✅ Health checks for better reliability
✅ Optional EC2 deployment and cloud networking

## 🙏 Thank You
Big thanks to DPDzero for this hands-on and practical assignment.

🧠 It strengthened my skills in DevOps fundamentals, containerization, orchestration, and cloud testing.

## 🔗 Connect With Me
### 👩‍💼 LinkedIn: Divya Satpute


## Solutions


![image](https://github.com/user-attachments/assets/89693513-225d-4da5-b556-0ffad6489ff5)
![image](https://github.com/user-attachments/assets/dade1f76-29c5-40da-8ff3-e1a589183a98)
![image](https://github.com/user-attachments/assets/32a9ab9e-34e4-4330-ae40-c414e9065d58)
![image](https://github.com/user-attachments/assets/0c613c06-2a0f-49ef-929f-374505bcfd51)
![image](https://github.com/user-attachments/assets/b3bc220b-9470-4802-aa16-338393f4208a)


## Video demontration link 
### https://drive.google.com/file/d/1XykCtWmVA2q0M4d8B4ARMbSbPKgdnWqi/view?usp=sharing

