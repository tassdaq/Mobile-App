# Mobile Webapp Deployment on ubuntu nginx webserver:
Create EC2 Instance Resource Webpage (source code provided in GitHub link " https://github.com/tassdaq/Mobile-App.git " publish on Public IP

## Description:
This project involves setting up an AWS EC2 instance to host a webpage accessible via its public IP. 
The instance will be launched in a customized VPC and configured with the necessary security rules to allow SSH, ICMP, and HTTP traffic.


### Project Specifications:
Region: US-East-1
VPC: Customized (Webpage)
IP Pool: 12.0.0.0/16
Subnet: 12.0.0.0/24
Security Group: Webpage (Allow SSH, ICMP, and HTTP only)
Instance Type: T2.micro (Free Tier Eligible)
Image: Ubuntu
Key Pair: .pem
Storage: Default



Implementation Steps:

Create a VPC with the specified IP range (12.0.0.0/16).
![VPC](https://github.com/user-attachments/assets/0a9fe519-69af-40fd-9448-bf3efd53ec84)

Set up a Subnet within the VPC (12.0.0.0/24).
![Subnet](https://github.com/user-attachments/assets/d2e87ea8-1af0-4adb-bfc1-fffcc363e4c9)

Create a Security Group with rules to allow SSH (port 22), ICMP (ping), and HTTP (port 80) access.
![SG-1](https://github.com/user-attachments/assets/28c9e0ed-88ac-4126-8847-ac7e0f206b2d)
![SG](https://github.com/user-attachments/assets/16afebe0-1c73-4086-a1bc-9cf31d58d1c1)

Launch an EC2 Instance using the Ubuntu AMI, selecting the T2.micro instance type.
![Instance-Type](https://github.com/user-attachments/assets/c87d8e1e-a2e9-4188-891c-17890db8ed7e)
![Image](https://github.com/user-attachments/assets/29c42a6d-7c83-4b27-8de8-f1a74b20e8c2)

Attach the Security Group to the instance.
Generate a Key Pair (.pem file) for SSH access.
Allocate and Assign a Public IP to the instance.
Configure the Instance to host a basic webpage.
Test Connectivity using SSH, ICMP, and HTTP.



Expected Outcome:
A publicly accessible webpage hosted on the EC2 instance, accessible via its public IP address, with proper security configurations.
![Web](https://github.com/user-attachments/assets/c5f95c74-e24d-4af9-b51d-373b4e06d5ca)
	

 

