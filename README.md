<div align="center">

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
Handles user requests from browser.

➡️ Used **Nginx Server** on Public EC2 Instance.

### 🔹 2. Application Layer
Runs business logic and Java application.

➡️ Used **Apache Tomcat** on Private EC2 Instance.

### 🔹 3. Database Layer
Stores application data securely.

➡️ Used **Amazon RDS MariaDB**

---



# 🔄 Project Flow

```text
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
Server Name	Location	Purpose
Jump Server	Public Subnet	Nginx Reverse Proxy
App Server	Private Subnet	Tomcat Hosting
Database	Private Subnet	Secure Storage
⚙️ What I Did in This Project
✅ Step 1: Networking Setup
Created custom VPC
Created 3 subnets
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

Started Tomcat server.

Deployed Java WAR file.

✅ Step 4: Reverse Proxy Setup

Installed Nginx on Jump Server.

Configured:

location / {
proxy_pass http://Private-IP:8080/student/;
}
✅ Step 5: Database Setup

Created Amazon RDS MariaDB.

Connected Java app with database using JDBC connector.

📸 Project Output
🔹 AWS Architecture
<p align="center"> <img src="images/output1.png" width="80%"> </p>
🔹 Tomcat Running
<p align="center"> <img src="images/output2.png" width="80%"> </p>
🔹 Java Application Form
<p align="center"> <img src="images/output3.png" width="80%"> </p>
🔹 Database Connected
<p align="center"> <img src="images/output4.png" width="80%"> </p>
🎯 Final Result

When user opens Public IP:

User → Nginx → Tomcat → Database

Application runs successfully and stores user data in database.

📚 Skills Learned

✅ AWS Networking
✅ Linux Commands
✅ EC2 Management
✅ Nginx Reverse Proxy
✅ Apache Tomcat
✅ Java Deployment
✅ RDS Database
✅ Cloud Security
✅ Real Production Architecture

💼 Best For
AWS Resume Project
DevOps Fresher Project
Cloud Engineer Interview
Linux Admin Interview
👩‍💻 Author
Akshada Kiran Doke

Cloud & DevOps Learner ☁️
Linux | AWS | GitHub | Automation

⭐ Support

If you like this project, give it a ⭐ on GitHub.
