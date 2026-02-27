# Lab 3 – Introduction to Amazon Elastic Compute Cloud (EC2)

## Author

* **Name**: EZHILARASI N
* **Register Number**: 212224040088
* **Date of Submission**: 27.02.2026

---

## Objective

The objective of this experiment is to understand the fundamentals of Amazon Elastic Compute Cloud (EC2). This lab focuses on launching and managing a virtual server, understanding instance types and AMIs, connecting to an EC2 instance, monitoring its status, and performing basic instance operations such as start, stop, and terminate.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* Web browser with internet connectivity
* Basic knowledge of Linux commands (optional)

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Key Pair
* Security Group
* SSH Client (PuTTY / Terminal)

---

## Tasks Performed

### Task 1: Explore Amazon EC2 Dashboard

Explore the EC2 service dashboard in the AWS Management Console. Observe the different sections such as Instances, AMIs, Instance Types, Key Pairs, Security Groups, and Elastic IPs.

---

### Task 2: Launch an EC2 Instance

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type (t2.micro) under the free tier. Configure basic settings such as instance name, key pair, and security group.

---

### Task 3: Configure Security Group

Configure a security group to allow inbound access:

* SSH (Port 22) from your IP address
* HTTP (Port 80) from anywhere (0.0.0.0/0)

This security group acts as a firewall for the instance.

---

### Task 4: Connect to EC2 Instance

Connect to the running EC2 instance using SSH. Use the downloaded key pair and connect via terminal or PuTTY.

For Amazon Linux:

```
ssh -i "keyname.pem" ec2-user@<Public-IP>
```

---

### Task 5: Perform Basic Instance Operations

Perform the following operations from the EC2 console:

* Stop the instance
* Start the instance
* Reboot the instance

Observe the state changes of the instance.

---

### Task 6: Monitor EC2 Instance

Monitor the EC2 instance using the Monitoring tab. Observe metrics such as CPU utilization, network in/out, and instance status checks.

---

### Task 7: Terminate EC2 Instance

Terminate the EC2 instance after completing the experiment to avoid unnecessary AWS charges.

---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)

First, I opened the AWS Management Console and selected the EC2 service in the N. Virginia (us-east-1) region. I launched a new instance and named it Web Server.

I selected the default Amazon Linux 2023 AMI and kept the instance type as t2.micro. I chose the existing key pair vockey.

In the network settings, I selected Lab VPC and kept PublicSubnet1. I created a new security group named Web Server security group and removed the default inbound rule.

In Advanced details, I enabled termination protection and added the User Data script to install and start the Apache web server and create a simple HTML page.

After launching the instance, I waited until it showed Running and 2/2 status checks passed.

Next, I monitored the instance using the Status checks, Monitoring tab, System log, and Instance screenshot options.

When I tried accessing the web server using the public IP address, it did not load because HTTP traffic was not allowed. So, I edited the security group and added an HTTP (port 80) inbound rule with source Anywhere-IPv4. After refreshing the browser, the message “Hello From Your Web Server!” appeared.

Then, I stopped the instance and changed the instance type from t2.micro to t2.small. I also enabled stop protection and increased the EBS volume size from 8 GiB to 10 GiB. After that, I started the instance again.

I explored EC2 Service Quotas to check instance limits.

Finally, I tested stop protection by trying to stop the instance. It failed because stop protection was enabled. I disabled stop protection and successfully stopped the instance.

## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Dashboard / Instance List

<img width="863" height="473" alt="image" src="https://github.com/user-attachments/assets/7eb2b7f7-8a1a-4462-870a-b4ac11ee0356" />


### Screenshot 2: SSH Connection to Instance

<img width="857" height="478" alt="image" src="https://github.com/user-attachments/assets/8fb83436-0948-4abd-b4c8-b72cc961fa16" />


### Screenshot 3: Instance Monitoring / Status

<img width="867" height="471" alt="image" src="https://github.com/user-attachments/assets/78d61a08-5e98-40c0-9d0b-d63dabd0bb33" />

## Result 

This experiment provided hands-on experience with Amazon EC2 by demonstrating how to launch, connect, manage, and monitor a virtual server in AWS. It helped in understanding the concept of Infrastructure as a Service (IaaS) and how compute resources can be provisioned and controlled on demand in the cloud.
