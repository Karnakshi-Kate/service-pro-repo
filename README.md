# Microservices Deployment Using Auto Scaling Group and Load Balancer

## Project Introduction
This project demonstrates how to deploy a microservices-based application on AWS using EC2 instances, an Auto Scaling Group (ASG), and an Application Load Balancer (ALB). The main objective of this project is to achieve scalability, high availability, and efficient traffic distribution for cloud-based applications.

The infrastructure is designed to automatically launch or terminate EC2 instances based on traffic demand. The Application Load Balancer distributes incoming traffic evenly across multiple EC2 instances, ensuring better performance and reliability.

This project helps in understanding:
- AWS EC2 instance deployment
- Auto Scaling Group configuration
- Application Load Balancer setup
- High availability architecture
- Scalable cloud infrastructure
- Basic DevOps deployment concepts

---

## Technologies Used
- AWS EC2
- Auto Scaling Group (ASG)
- Application Load Balancer (ALB)
- Security Groups
- Target Groups
- Linux / Ubuntu
- Git & GitHub

---

## Architecture Diagram

![Architecture Diagram](./img/ChatGPT%20Image%20May%2024,%202026,%2002_37_13%20PM.png)

---

## Project Setup Steps

### 1. Launch Template
- Create launch template on AWS
- Configure Security Group rules
- Install required packages and application dependencies

---

### Home-LT

![](./img/Screenshot-1.png)

![](./img/Screenshot-2.png)

![](./img/Screenshot-3.png)

![](./img/Screenshot-4.png)

---

### Mobile-LT

![](./img/Screenshot-5.png)

![](./img/Screenshot-6.png)

---

### Laptop-LT

![](./img/Screenshot-7.png)

![](./img/Screenshot-8.png)

---

### 2. Create Auto Scaling Group
- Create launch template
- Configure minimum, desired, and maximum capacity
- Attach ALB target group
- Configure scaling policies

---

### Home-ASG

![](./img/Screenshot-10.png)

![](./img/Screenshot-11.png)

![](./img/Screenshot-12.png)

![](./img/Screenshot-13.png)

![](./img/Screenshot-14.png)

![](./img/Screenshot-15.png)

![](./img/Screenshot-16.png)

![](./img/Screenshot-17.png)

![](./img/Screenshot-18.png)

![](./img/Screenshot-19.png)

![](./img/Screenshot-20.png)

![](./img/Screenshot-21.png)

---

### Mobile-ASG

![](./img/Screenshot-22.png)

![](./img/Screenshot-23.png)

![](./img/Screenshot-24.png)

![](./img/Screenshot-25.png)

![](./img/Screenshot-26.png)

![](./img/Screenshot-27.png)

![](./img/Screenshot-28.png)

---

### Laptop-ASG

![](./img/Screenshot-29.png)

![](./img/Screenshot-30.png)

![](./img/Screenshot-31.png)

![](./img/Screenshot-32.png)

![](./img/Screenshot-33.png)

![](./img/Screenshot-34.png)

![](./img/Screenshot-35.png)

![](./img/Screenshot-36.png)

![](./img/Screenshot-37.png)

![](./img/Screenshot-38.png)

![](./img/Screenshot-39.png)

---

### 3. Create Target Group

- Configure target group for EC2 instances
- Set health check path and protocol

---

### Home-TG

![](./img/Screenshot-41.png)

![](./img/Screenshot-42.png)

![](./img/Screenshot-43.png)

![](./img/Screenshot-44.png)

![](./img/Screenshot-45.png)

---

### Mobile-TG

![](./img/Screenshot-46.png)

![](./img/Screenshot-47.png)

![](./img/Screenshot-48.png)

![](./img/Screenshot-49.png)

![](./img/Screenshot-50.png)

![](./img/Screenshot-51.png)

---

### Laptop-TG

![](./img/Screenshot-52.png)

![](./img/Screenshot-53.png)

![](./img/Screenshot-54.png)

![](./img/Screenshot-55.png)

![](./img/Screenshot-56.png)

![](./img/Screenshot-57.png)

![](./img/Screenshot-58.png)

---

### 4. Target group attach to Auto Scaling group

---

### attach Home-TG to ASG

![](./img/Screenshot-59.png )

![](./img/Screenshot-60.png)

![](./img/Screenshot-61.png)

![](./img/Screenshot-62.png)

---

### attach Mobile-TG to ASG

![](./img/Screenshot-63.png)

![](./img/Screenshot-64.png)

![](./img/Screenshot-65.png)

---

### attach Laptop-TG to ASG

![](./img/Screenshot-66.png)

![](./img/Screenshot-67.png)

![](./img/Screenshot-68.png)

---

### 5. Create Scheduile Action

![](./img/Screenshot-69.png)

![](./img/Screenshot-70.png)

![](./img/Screenshot-71.png)

![](./img/Screenshot-72.png)

---

### 6. Configure Load Balancer

- Create Application Load Balancer
- Attach target group
- Configure listener rules

![](./img/Screenshot-73.png)

![](./img/Screenshot-74.png)

![](./img/Screenshot-75.png)

![](./img/Screenshot-76.png)

![](./img/Screenshot-77.png)

![](./img/Screenshot-78.png)

![](./img/Screenshot-79.png)

![](./img/Screenshot-80.png)

![](./img/Screenshot-81.png)

![](./img/Screenshot-82.png)

![](./img/Screenshot-83.png)

![](./img/Screenshot-84.png)

![](./img/Screenshot-85.png)

![](./img/Screenshot-86.png)

---

### 6. Testing
- Access application using Load Balancer DNS
- Test automatic scaling during high traffic
- Verify health checks and failover

![](./img/Screenshot-87.png)

![](./img/Screenshot%202026-05-08%20133944.png)

![](./img/Screenshot%202026-05-08%20134018.png)

![](./img/Screenshot%202026-05-08%20134048.png)

![](./img/Screenshot%202026-05-08%20134103.png)

---

## Features
- Automatic scaling of EC2 instances
- High availability architecture
- Traffic distribution using Load Balancer
- Fault tolerance
- Scalable cloud deployment
- Easy infrastructure management

---

## Project Summary
In this project, a microservices application was successfully deployed on AWS cloud infrastructure using EC2 instances. An Auto Scaling Group was configured to dynamically manage the number of instances according to traffic load, while the Application Load Balancer ensured efficient traffic distribution across healthy instances.

This setup improves application reliability, scalability, and performance while reducing manual infrastructure management efforts.

---

## Conclusion
This project provided practical experience with AWS cloud services and modern deployment architecture. By implementing Auto Scaling Groups and Load Balancers, the application became more scalable, reliable, and capable of handling varying traffic loads efficiently.

The project also helped in understanding important cloud computing concepts such as high availability, fault tolerance, traffic management, and automated infrastructure scaling. These skills are essential for DevOps and cloud engineering roles.

---
