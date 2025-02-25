# Docker_JavaApp
## 📌 Project Overview
This project focuses on **containerizing** a multi-tier Java web application using **Docker and Docker Compose**. Each service runs in its own container, ensuring portability, scalability, and efficient management.

 

## 🛠 Tech Stack
- **Docker & Docker Compose** – Container orchestration  
- **Tomcat** – Java application server  
- **Nginx** – Reverse proxy & load balancing  
- **RabbitMQ** – Message broker  
- **Memcached** – Caching layer  
- **MySQL** – Relational database  

## 📂 Project Structure
```
📂 multi-tier-app-dockerized/
 ├── docker-compose.yml
 ├── .env
 ├── tomcat/
 │   ├── Dockerfile
 ├── nginx/
 │   ├── Dockerfile
 ├── mysql/
 │   ├── Dockerfile
 ├── memcached/
 │   ├── Dockerfile
 ├── rabbitmq/
 │   ├── Dockerfile
```

## 🔧 Setup Instructions
1️⃣ **Clone the Repository**  
```bash
git clone <repo-link>
cd multi-tier-app-dockerized
```

2️⃣ **Configure Environment Variables**  
Modify the `.env` file with your configurations.

3️⃣ **Build and Run the Containers**  
```bash
docker-compose up -d --build
```

4️⃣ **Verify Running Containers**  
```bash
docker ps
```

5️⃣ **Access the Application**  
- **Frontend (Nginx):** `http://localhost:80`
- **Tomcat Application:** `http://localhost:8080`
- **Database (MySQL):** `localhost:3306`
- **RabbitMQ Management UI:** `http://localhost:15672`

## 🚀 Next Steps
- **Deploy on Kubernetes** (Coming Soon!)  
- **CI/CD Integration**  

## 📌 Contributing
Feel free to fork, open issues, or submit pull requests!  

---
📌 **Authors:** [Nader Ashour] & [Mohamed Elweza]  
