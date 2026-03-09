# Lab 5 – Build a Database Server (AWS)

## Author

* **Name**: EZHILARASI N
* **Register Number**: 212224040088
* **Date of Submission**: 09.03.2026

---

## Objective

The objective of this experiment is to understand how to deploy and configure a database server in AWS. This lab focuses on launching an EC2 instance, installing a database management system (DBMS), configuring basic database settings, creating a sample database, and validating connectivity to the database server.

---

## Prerequisites

* Basic understanding of cloud computing concepts
* AWS account or AWS Academy Lab access
* An existing VPC and EC2 knowledge (from previous labs)
* Basic knowledge of Linux commands and SQL

---

## Tools Used

* AWS Management Console
* Amazon EC2
* Security Groups
* SSH Client (Terminal / PuTTY)
* MySQL / MariaDB / PostgreSQL (any one)

---

## Tasks Performed

### Task 1: Launch EC2 Instance for Database Server

Launch a new EC2 instance using Amazon Linux 2 AMI. Select an appropriate instance type and configure key pair and security group.

---

### Task 2: Configure Security Group for Database Access

Modify the security group to allow:

* SSH (Port 22) for remote access
* Database port (e.g., MySQL – 3306 or PostgreSQL – 5432)

---

### Task 3: Connect to EC2 Instance

Connect to the EC2 instance using SSH from your local machine.

---

### Task 4: Install Database Server

Install a database server software such as MySQL, MariaDB, or PostgreSQL on the EC2 instance using package manager commands.

---

### Task 5: Start and Configure Database Service

Start the database service and configure basic settings such as root password and user privileges.

---

### Task 6: Create a Sample Database

Create a sample database and a table inside it. Insert a few records into the table.

---

### Task 7: Test Database Connectivity

Test the database server by connecting to it locally or remotely and performing basic SQL queries.

---

## Workflow (Student Explanation)

(Write the steps you followed in your own words)

1. Logged in to AWS Management Console and opened Amazon EC2.

2. Launched a new EC2 instance using Amazon Linux 2 AMI and selected an appropriate instance type.

3. Created/selected a key pair and configured a security group for the instance.

4. Modified the security group to allow SSH (Port 22) and database access (3306 for MySQL or 5432 for PostgreSQL).

5. Connected to the EC2 instance using an SSH client such as PuTTY or terminal.

6.Installed the database server (e.g., MySQL, MariaDB, or PostgreSQL) using Linux package manager commands.

7. Started the database service and configured basic settings such as the root password and user privileges.

8. Created a sample database and table and inserted a few records.

9. Tested database connectivity by running basic SQL queries.
 


## Output Screenshots (Attach 3)

### Screenshot 1: EC2 Instance for Database Server

<img width="1919" height="1069" alt="Screenshot 2026-03-08 150312" src="https://github.com/user-attachments/assets/e433954b-0362-4d1b-b650-bd7aff1bdd34" />

<img width="1919" height="1068" alt="Screenshot 2026-03-08 150723" src="https://github.com/user-attachments/assets/93b2d716-5aa7-4746-b02d-eba40562f4f5" />

---

### Screenshot 2: Database Service Running

<img width="1919" height="1070" alt="Screenshot 2026-03-08 152649" src="https://github.com/user-attachments/assets/c6b28a0d-8181-4d54-9fef-6a077a9ec673" />


<img width="1920" height="1200" alt="Screenshot (255)" src="https://github.com/user-attachments/assets/2deddce9-5f36-4693-a445-13b13d57c99c" />


### Screenshot 3: Sample Database and Table

<img width="1920" height="1200" alt="Screenshot (259)" src="https://github.com/user-attachments/assets/23a47c8c-17e7-46c6-9201-ba43df096b07" />


## Result

This experiment demonstrated how to build a database server in AWS using an EC2 instance. By installing and configuring a DBMS, creating a sample database, and testing connectivity, the fundamentals of hosting and managing a cloud-based database server were underst
