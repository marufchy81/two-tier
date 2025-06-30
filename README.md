
# Two-Tier Docker Project

## Author
**Maruf Chowdhury**

## Project Overview
This project demonstrates a two-tier architecture using Docker, Docker Compose, Docker Swarm, NGINX, and custom application containers. The frontend interacts with backend logic to perform number operations such as reversing and summing digits. Everything is containerized and orchestrated for portability and scalability.

---

## Tools & Technologies Used
- **Docker** â€“ Containerization of frontend and backend services
- **Docker Compose** â€“ Local multi-container setup
- **Docker Hub** â€“ Hosting custom images
- **NGINX** â€“ Web server and reverse proxy
- **Docker Swarm** â€“ (Optional) for clustering and service management
- **EC2 Instances** â€“ Hosting the project on AWS

---

## Features
- Number reverse and summation web app
- Containerized frontend served via NGINX
- Custom backend logic in separate container
- Responsive communication between tiers

---

## Screenshots

### 1. EC2 Instances
![EC2 Instances](1.png)

### 2. Application Working (Frontend)
![Frontend React App](2.png)

### 3. Docker Containers Running (Terminal)
![Docker ps](3.png)

### 4. Docker Hub Image Repo
![Docker Hub](4.png)

### 5. NGINX Welcome Page (Port 8080)
![NGINX](welcomenginx.png)

---

## How to Run This Project
### Step 1: Clone the Repository
```bash
git clone https://github.com/yourusername/two-tier-project.git
cd two-tier-project
```

### Step 2: Build & Run with Docker Compose
```bash
docker-compose up --build
```

### Step 3: Access the App
- Navigate to: `http://<your-ec2-public-ip>:8080`

### Step 4: Push Images to DockerHub
```bash
docker tag your-image marufchy/your-image-name:tag
docker push marufchy/your-image-name:tag
```

### Step 5 (Optional): Deploy on Docker Swarm
```bash
docker swarm init
docker stack deploy -c docker-compose.yml yourstackname
```

---

## Conclusion
This project showcases end-to-end deployment of a basic two-tier app using Docker tools and AWS. It reflects an understanding of container networking, image publishing, orchestration, and real-world deployment.

---

Feel free to fork, star, and contribute!
