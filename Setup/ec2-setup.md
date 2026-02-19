# EC2 Setup
# EC2 Instance Setup

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

