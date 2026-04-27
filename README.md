

# 🚀 AWS 3-Tier Architecture Project

### Java Web Application Deployment using AWS Cloud

![AWS](https://img.shields.io/badge/AWS-Cloud-orange?style=for-the-badge)
![Java](https://img.shields.io/badge/Java-WebApp-red?style=for-the-badge)
![Nginx](https://img.shields.io/badge/Nginx-ReverseProxy-green?style=for-the-badge)
![Tomcat](https://img.shields.io/badge/Tomcat-AppServer-yellow?style=for-the-badge)
![RDS](https://img.shields.io/badge/RDS-MariaDB-blue?style=for-the-badge)

### ☁️ Real Industry Based Cloud Deployment Project

</div>

---

# 📌 Project Overview

This project demonstrates how companies deploy applications securely using **3-Tier Architecture** on AWS.

A Java web application is hosted using separate layers:

### 🔹 1. Presentation Layer
Handles user requests from browser using **Nginx**.

### 🔹 2. Application Layer
Runs business logic and Java application using **Apache Tomcat**.

### 🔹 3. Database Layer
Stores data securely using **Amazon RDS MariaDB**.

---

# 🏗️ Architecture Flow

```text id="y4hnpz"
User Browser
     ↓
Public IP
     ↓
Nginx Server
     ↓
Tomcat Server
     ↓
Java WAR Application
     ↓
Amazon RDS Database
☁️ AWS Services Used
AWS Service	Purpose
EC2	Virtual Servers
VPC	Private Network
Public Subnet	Internet Access
Private Subnet	Secure Internal Servers
Security Group	Firewall Rules
Internet Gateway	Public Internet
NAT Gateway	Internet for Private Server
RDS	Managed Database
🖥️ Servers Created
Server Name	Purpose
Jump Server	Nginx Reverse Proxy
App Server	Tomcat Hosting
Database	Secure Storage
⚙️ What I Did in This Project
✅ Step 1: Networking Setup
Created custom VPC
Created public and private subnets
Attached Internet Gateway
Created NAT Gateway
Configured Route Tables
✅ Step 2: Security Setup

Allowed ports:

22 → SSH
80 → HTTP
443 → HTTPS
8080 → Tomcat
3306 → MySQL
✅ Step 3: Application Deployment

Installed:

Java
Apache Tomcat

Started Tomcat server and deployed Java WAR file.

✅ Step 4: Reverse Proxy Setup

Installed Nginx and configured:

location / {
proxy_pass http://Private-IP:8080/student/;
}
✅ Step 5: Database Setup

Created Amazon RDS MariaDB and connected application database.

🎯 Final Result
User → Nginx → Tomcat → Database

Application runs successfully and stores data securely.

📚 Skills Learned

✅ AWS Networking
✅ Linux Commands
✅ EC2 Management
✅ Nginx Reverse Proxy
✅ Apache Tomcat
✅ Java Deployment
✅ RDS Database
✅ Cloud Security

💼 Best For
AWS Resume Project
DevOps Fresher Project
Cloud Engineer Interview
Linux Admin Interview
👩‍💻 Author
Akshada Kiran Doke

Cloud & DevOps Learner ☁️
Linux | AWS | GitHub

⭐ Support

If you like this project, give it a ⭐ on GitHub.
