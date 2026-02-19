# EC2 Instance Setup

# Steps to Create an EC2 Instance on AWS

## 1. Login
- Go to **AWS Management Console**
- Sign in with your AWS account.

---

## 2. Open EC2 Dashboard
- Navigate to: **Services → Compute → EC2**
- Click **Launch Instance**

---

## 3. Configure Instance

### Name
Enter any instance name  
Example: `MyServer`

### AMI (Operating System)
Choose an OS template:
- Amazon Linux
- Ubuntu
- Windows

### Instance Type
Select hardware configuration  
**Free tier:** `t2.micro` or `t3.micro`

### Key Pair
- Create or select key pair
- Download `.pem` file (used for SSH login)

### Network Settings
Allow:
- SSH (Port 22)
- HTTP (Port 80)
- HTTPS (Port 443)

### Storage
- Default: **8 GB**
- Increase if needed

---

## 4. Launch Instance
Click **Launch Instance**  
Wait until **Instance State = Running**

---

## 5. Connect to Instance
Select instance → Click **Connect**

Connection options:
- EC2 Instance Connect (browser)
- SSH client (using key pair)

---

## ✅ Done!
Your cloud server is now live 

---

## Objective
The objective of this step was to deploy a basic compute resource using Amazon EC2 to host a simple web application and understand core cloud infrastructure concepts.

## Instance Configuration
- AMI: Amazon Linux 2
- Instance Type: t2.micro (Free Tier eligible)
- Network: Default VPC
- Public IP: Enabled
- Storage: Default root volume

## Security Group Configuration
The following inbound rules were configured:
- SSH (Port 22): Allowed only from my local IP address
- HTTP (Port 80): Allowed from anywhere to access the web application

This ensured secure administrative access while allowing public access to the application.

## Application Deployment
- Connected to the EC2 instance using SSH
- Installed Apache HTTP server
- Started and enabled the web service
- Deployed a simple HTML page to verify successful setup

## Verification
The application was verified by accessing the EC2 public IP address through a web browser and confirming the page loaded successfully.

## Outcome
A running EC2 instance was successfully deployed with a basic web application, forming the foundation for monitoring and operational tasks in the next steps.

