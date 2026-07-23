
# 🚀 AWS Serverless Event Announcement System

A **fully serverless event announcement application** built using **AWS** and **Terraform**. This project enables users to create events, subscribe to notifications, and view announcements through a responsive static web application.

---

## 📖 Project Overview

This project demonstrates how to build a scalable serverless application using **Infrastructure as Code (IaC)** with **Terraform**.

###  Key Features

- ✅ Create and publish event announcements
- ✅ Subscribe to event notifications via email
- ✅ View upcoming events through a web interface
- ✅ Fully serverless architecture
- ✅ Infrastructure managed with Terraform
- ✅ Static website hosted on Amazon S3
- ✅ Fast content delivery using CloudFront

---

# 🏗️ Architecture


<img width="1672" height="941" alt="ChatGPT Image Jul 23, 2026, 10_25_12 PM" src="https://github.com/user-attachments/assets/7ea864bd-11c7-495c-aae5-263ceaaf38c9" />


```text
                    👤 User
                       │
                       ▼
              ☁️ CloudFront CDN
                       │
                       ▼
                 🪣 Amazon S3
               (Static Website)
                       │
        ┌──────────────┴──────────────┐
        │                             │
        ▼                             ▼
  🌐 API Gateway                📄 events.json
        │
   ┌────┴────┐
   ▼         ▼
⚡ Lambda   ⚡ Lambda
(Create)   (Subscribe)
   │         │
   ▼         ▼
🪣 S3 Bucket 📧 Amazon SNS
```

---

# 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| ☁️ AWS Lambda | Backend Functions |
| 🌐 API Gateway | REST APIs |
| 🪣 Amazon S3 | Static Website Hosting |
| 📧 Amazon SNS | Email Notifications |
| 🚀 CloudFront | Content Delivery |
| 🔐 IAM | Security & Permissions |
| 🏗️ Terraform | Infrastructure as Code |
| 🐍 Python (boto3) | Lambda Development |
| 🌐 HTML | Frontend |
| 🎨 CSS | Styling |
| ⚡ JavaScript | Client-side Logic |
| 🐙 Git & GitHub | Version Control |

---

# 📂 Project Structure

```text
Event-Announcement-System/
│
├── 📁 frontend/
│   ├── index.html
│   ├── styles.css
│   └── events.json
│
├── 📁 lambda/
│   ├── create_event.py
│   ├── subscribe.py
│   ├── create_event.zip
│   └── subscribe.zip
│
├── 📁 terraform/
│   ├── main.tf
│   ├── variables.tf
│   ├── outputs.tf
│   ├── terraform.tfvars
│   └── .terraform.lock.hcl
│
├── 📁 scripts/
│   └── update-frontend.sh
│
├── 📄 deploy.sh
├── 📄 .gitignore
└── 📄 README.md
```

---

# ✨ Features

✅ Fully Serverless Application

✅ Infrastructure as Code (Terraform)

✅ Static Website Hosting (Amazon S3)

✅ Global Content Delivery (CloudFront)

✅ REST APIs with API Gateway

✅ Event Creation using AWS Lambda

✅ Email Notifications with Amazon SNS

✅ Automated Deployment Script

---

# 🚀 Deployment

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/dilli-prathap/Event-Announcement-System.git
cd Event-Announcement-System
```

---

## 2️⃣ Initialize Terraform

```bash
cd terraform

terraform init
terraform plan
terraform apply
```

Or simply run:

```bash
./deploy.sh
```

---

# 🧹 Destroy Infrastructure

```bash
./deploy.sh destroy
```

or

```bash
terraform destroy
```

---

# ⚙️ Configuration

Update the values in:

```text
terraform/terraform.tfvars
```

Example:

```hcl
aws_region         = "us-east-1"
bucket_name        = "your-bucket-name"
notification_email = "your-email@example.com"
```

---

# ☁️ AWS Services Used

| Service | Description |
|----------|-------------|
| ⚡ Lambda | Backend Compute |
| 🌐 API Gateway | API Management |
| 🪣 Amazon S3 | Static Website Hosting |
| 📧 Amazon SNS | Email Notifications |
| 🚀 CloudFront | CDN |
| 🔐 IAM | Access Management |
| 🏗️ Terraform | Infrastructure Automation |


<img width="1667" height="657" alt="Screenshot 2026-07-23 210648" src="https://github.com/user-attachments/assets/69c6ed47-77c0-4ab4-b4c7-1b55c788befb" />
<img width="1637" height="648" alt="Screenshot 2026-07-23 210709" src="https://github.com/user-attachments/assets/bd8a2ac8-5cd7-4fd2-b73c-6762278a5a3e" />
<img width="1277" height="437" alt="Screenshot 2026-07-23 210744" src="https://github.com/user-attachments/assets/ec40411c-3a15-4126-ad8d-d24e748fef5a" />
<img width="1602" height="787" alt="Screenshot 2026-07-23 210922" src="https://github.com/user-attachments/assets/bc81a111-8a9d-4a6a-8f68-1e152968a373" />
<img width="1571" height="763" alt="Screenshot 2026-07-23 211216" src="https://github.com/user-attachments/assets/372425c3-3992-448e-8a21-5cb76b11769e" />
<img width="582" height="202" alt="Screenshot 2026-07-23 211240" src="https://github.com/user-attachments/assets/8e09d8ce-4cd3-410b-81df-3d21ecf9a179" />
<img width="1557" height="633" alt="Screenshot 2026-07-23 211256" src="https://github.com/user-attachments/assets/c6d013c1-613b-45ce-989c-a19227d0ba65" />

---

# 📸 Project Highlights

✅ Fully Automated Deployment

✅ Scalable Serverless Architecture

✅ Event Notification System

✅ Static Website Hosting

✅ Infrastructure as Code

✅ Cloud-Based Solution

---


# 🎯 Learning Outcomes

This project helped me gain practical experience in:

-  AWS Serverless Architecture
-  Infrastructure as Code (Terraform)
-  AWS Lambda Development
-  API Gateway Integration
-  Amazon SNS Notifications
-  Amazon S3 Static Website Hosting
-  CloudFront Distribution
-  Python (boto3)
-  Git & GitHub
-  Cloud Deployment

---

# 🔮 Future Enhancements

- 🔐 User Authentication (Amazon Cognito)
- ✏️ Edit & Delete Events
- 🗄️ DynamoDB Integration
- 🖼️ Image Upload Support
- 🏷️ Event Categories
- 🔍 Search & Filter Events
- ⚙️ GitHub Actions CI/CD Pipeline
- 📱 Responsive UI Improvements

---

# 👨‍💻 Author

**Dilli Prathap**

💼 Aspiring Cloud & DevOps Engineer

🐙 GitHub: **https://github.com/dilli-prathap**

---

# ⭐ If you found this project useful...

Give this repository a ⭐ on GitHub!

Happy Coding! 🚀
