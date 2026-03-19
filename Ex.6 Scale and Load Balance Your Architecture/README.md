# Lab 6 – Scale and Load Balance Your Architecture

## Title

Scale and Load Balance Your Architecture
Author : your name   Reg no : yours   Date :

---

## Objective

The objective of this lab is to understand how to design a scalable and highly available architecture on AWS using Auto Scaling and Elastic Load Balancing. This experiment focuses on distributing incoming traffic across multiple EC2 instances, automatically scaling resources based on demand, and validating fault tolerance.

---

## Prerequisites

* Basic knowledge of Amazon EC2 and VPC
* Completion of previous labs (IAM, EC2, EBS, Database Server)
* AWS Academy Lab access
* Stable internet connection

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Elastic Load Balancer (ELB / ALB)
* Auto Scaling Groups (ASG)
* Amazon CloudWatch

---

## Tasks Performed

### Task 1: Review Existing Architecture

Students review the existing EC2-based application architecture created in previous experiments.

### Task 2: Create a Launch Template

Students create a launch template that defines the EC2 instance configuration including AMI, instance type, security group, and user data.

### Task 3: Create an Auto Scaling Group

Students create an Auto Scaling Group using the launch template and configure minimum, maximum, and desired instance capacity.

### Task 4: Configure an Application Load Balancer

Students create an Application Load Balancer and configure target groups for routing traffic to EC2 instances.

### Task 5: Register Auto Scaling Group with Load Balancer

Students attach the Auto Scaling Group to the target group of the load balancer.

### Task 6: Configure Scaling Policies

Students configure scaling policies based on CPU utilization using Amazon CloudWatch alarms.

### Task 7: Test Load Balancing and Scaling

Students test the setup by generating traffic and observing automatic scaling and load distribution.

---

## Workflow (To be filled by Student)

1. Describe step-by-step how you performed this experiment in your own words.

2. Logged into AWS and reviewed existing EC2 setup.

3. Created a launch template with AMI, instance type, security group, and user data.

4. Created an Auto Scaling Group with min, max, and desired capacity.

5. Set up an Application Load Balancer and target group.

6. Attached the Auto Scaling Group to the load balancer.

7. Configured scaling policies using CloudWatch (CPU-based).

8. Tested by generating traffic and observed load balancing and auto scaling.

9. Verified fault tolerance by stopping an instance and checking automatic replacement.
    
---

## Output Screenshots 

<img width="1920" height="1200" alt="Screenshot (263)" src="https://github.com/user-attachments/assets/cfbbd37f-0f5a-46bf-9447-d6775bdba0e1" />

<img width="1920" height="1200" alt="Screenshot (265)" src="https://github.com/user-attachments/assets/50012f05-875c-45f7-a225-0a993f5fc903" />

<img width="1920" height="1200" alt="Screenshot (266)" src="https://github.com/user-attachments/assets/0ee52a85-f32a-466d-8548-77e196b73d37" />

<img width="1920" height="1200" alt="Screenshot (267)" src="https://github.com/user-attachments/assets/16c97545-aac4-43e1-a923-b52df99973b3" />

<img width="1920" height="1200" alt="Screenshot (268)" src="https://github.com/user-attachments/assets/7b043671-c491-49fc-885d-1bbd1294fc56" />


<img width="1920" height="1200" alt="Screenshot (270)" src="https://github.com/user-attachments/assets/9ead375b-4026-4979-8a45-f74b860fc92a" />

<img width="1920" height="1200" alt="Screenshot (272)" src="https://github.com/user-attachments/assets/dfbd67ec-ebd8-462c-82c8-edb805492d61" />

<img width="1920" height="1200" alt="Screenshot (274)" src="https://github.com/user-attachments/assets/c99218fb-0d9e-45ec-b68b-752e0c2a0327" />

<img width="1920" height="1200" alt="Screenshot (275)" src="https://github.com/user-attachments/assets/0678275d-d7ed-4b33-85d3-a93d78a8474f" />


---


## Result

This experiment demonstrated how to build a scalable and fault-tolerant cloud architecture using Auto Scaling Groups and Elastic Load Balancing. The system automatically adjusted resources based on workload and ensured continuous service availability by distributing traffic across multiple instances.
