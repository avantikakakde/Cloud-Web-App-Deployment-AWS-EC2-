

# ☁️ My Cloud Web App — Deployed on AWS EC2

This project demonstrates how to **host a modern static web app** on the **Amazon Web Services (AWS) EC2** platform using **Apache Web Server**.  
The app features an attractive design with multiple tabs, smooth animations, and a dark/light mode toggle — perfect for learning **cloud deployment** basics.

---

## 🖥️ Project Overview

| Attribute | Details |
| :--- | :--- |
| **Platform** | Amazon Web Services (AWS) |
| **Service Used** | EC2 (Elastic Compute Cloud) |
| **Server OS** | Ubuntu |
| **Web Server** | Apache |
| **Frontend Stack** | HTML, CSS, JavaScript |
| **Deployment Type** | Static website (Manual Deployment) |

---

## 🌐 Live Demo

🔗 **Deployed URL:**  
👉 [http://13.233.45.182/index2.html]


![](./images/Screenshot%202025-10-28%20130240.png)
---



### ☁️ **2️⃣ AWS EC2 Instance Console**  

![AWS EC2 Console Screenshot](./images/Screenshot%202025-10-28%20124453.png)

---


---

## ⚙️ Deployment Steps (AWS EC2)

### **Step 1️⃣ — Launch EC2 Instance**
1. Go to **AWS Console → EC2 → Launch Instance**
2. Choose **Ubuntu Server 22.04 LTS (Free Tier Eligible)**
3. Instance type → `t2.micro`
4. Create or use an existing **key pair (.pem file)**
5. In **Security Group**, enable:
   - SSH (Port 22)
   - HTTP (Port 80)
6. Launch the instance

---

### **Step 2️⃣ — Connect to Your Instance**
Use SSH from your terminal:

 - ssh -i "your-key.pem" ubuntu@your-ec2-public-ip

 ---


### Step 3️⃣ — Install Apache Web Server

- sudo apt update -y

- sudo apt install apache2 -y



✅ Test it:

Open http://your-ec2-public-ip in a browser.

You should see the Apache default page.

---

 ### Step 4️⃣ — Deploy Your HTML App

Replace the default page with your custom web app:

- cd /var/www/html

- sudo nano index2.html

---

### Step 5️⃣ — Verify Deployment

Open:

http://http://13.233.45.182/index2.html


You should see your beautiful Cloud App live on the web 🌐

---




### 🧠 Short Note on Deployment

“This project demonstrates deploying a static web app on AWS EC2 using Apache Web Server.
I launched an Ubuntu instance, installed Apache, and uploaded an HTML app that features modern UI elements — like tab navigation and dark/light mode.
The deployment helped me understand key cloud concepts such as instance management, networking, and web hosting on AWS.”
