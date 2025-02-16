# Project Title:
Create EC2 Instance Resource Webpage (source code provided in GitHub link " https://github.com/tassdaq/webserver.git " publish on Public IP


## Description:
This project involves setting up an AWS EC2 instance to host a webpage accessible via its public IP. 
The instance will be launched in a customized VPC and configured with the necessary security rules to allow SSH, ICMP, and HTTP traffic.

![up-running](https://github.com/user-attachments/assets/9da71caa-e96a-42f1-b45f-1a71c8b4e82f)


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

Set up a Subnet within the VPC (12.0.0.0/24).

Create a Security Group with rules to allow SSH (port 22), ICMP (ping), and HTTP (port 80) access.

Launch an EC2 Instance using the Ubuntu AMI, selecting the T2.micro instance type.

Attach the Security Group to the instance.

Generate a Key Pair (.pem file) for SSH access.

Allocate and Assign a Public IP to the instance.

Configure the Instance to host a basic webpage.

Test Connectivity using SSH, ICMP, and HTTP.



Expected Outcome:

A publicly accessible webpage hosted on the EC2 instance, accessible via its public IP address, with proper security configurations.
		

 
 ![vpc-11](https://github.com/user-attachments/assets/b376565f-9d41-443f-9ad2-b505264abeb3)
![US-Region-1](https://github.com/user-attachments/assets/75aba4c1-ab5d-416d-8f61-80c7b675dac8)
![up-running](https://github.com/user-attachments/assets/b1821154-a5c9-45aa-8a13-249c53f48dc2)
![subnet](https://github.com/user-attachments/assets/2d411e4d-0437-4b58-beb7-fca8cbc4a9a8)
![SG-2](https://github.com/user-attachments/assets/41efc00d-3d5b-488c-ae9e-b7cf88783aa6)
![SG-1](https://github.com/user-attachments/assets/f0649a34-cda4-47c6-8d68-24367d715c13)
![Route-Table](https://github.com/user-attachments/assets/3c2d4a2d-8fe5-4945-b452-84168eb24312)
![Internet-Gateway](https://github.com/user-attachments/assets/0de804a8-2b62-405d-8613-cd11d43808a6)
![image2](https://github.com/user-attachments/assets/68354ea2-4d82-43f5-ae1a-18e9bbbb05b3)
![image](https://github.com/user-attachments/assets/a0020603-1d3d-49b5-b42b-ee918a80e931)
