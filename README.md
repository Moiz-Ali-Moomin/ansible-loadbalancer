# ⚖️ Load Balancer & Web Server Setup on AWS using Ansible

## 📌 Overview
This project demonstrates how to **automate the setup of a load-balanced web architecture on AWS using Ansible**.  
It provisions and configures:
- Multiple **web servers**
- A **load balancer** (e.g., HAProxy / Nginx)
- Required AWS infrastructure

The goal is to show **infrastructure automation, configuration management, and scalable system design** using Ansible.

---

## 🧠 Problem Statement
Manually configuring load balancers and backend web servers is:
- Error-prone
- Time-consuming
- Difficult to scale and reproduce

This project solves the problem by using **Ansible playbooks** to automate the deployment and configuration of all components in a repeatable way.

---

## 🏗️ Architecture & Workflow
User Request
↓
Load Balancer (AWS EC2)
↓
Web Server 1 Web Server 2
↓ ↓
-------- Application --------

yaml
Copy code

---

## 🛠️ Tech Stack
- **Cloud Provider:** AWS
- **Automation / Config Management:** Ansible
- **Load Balancer:** Nginx / HAProxy
- **Web Server:** Apache / Nginx
- **OS:** Linux
- **Configuration:** YAML

---

## ⚙️ Key Features
- Automated AWS infrastructure configuration
- Load balancer setup using Ansible
- Backend web server provisioning
- Modular Ansible playbooks
- Scalable and reusable architecture
- Infrastructure-as-Code approach

---

## 📂 Project Structure

```text
ansible-loadbalancer/
├── ec2.yml.yml             # AWS EC2 provisioning playbook
├── loadbalancer.yml.yml    # Load balancer configuration playbook
├── webserver.yml.yml       # Web server configuration playbook
└── README.md

🚀 How to Run the Project

1️⃣ Prerequisites

AWS account

IAM user with EC2 permissions

Ansible installed

Python installed

SSH key configured for EC2

Inventory file with target hosts

2️⃣ Clone the repository

bash
Copy code
git clone https://github.com/Moiz-Ali-Moomin/ansible-loadbalancer.git
cd ansible-loadbalancer

3️⃣ Provision EC2 instances

bash
Copy code
ansible-playbook ec2.yml.yml

4️⃣ Configure web servers

bash
Copy code
ansible-playbook webserver.yml.yml

5️⃣ Configure load balancer

bash
Copy code
ansible-playbook loadbalancer.yml.yml

📊 Outcome / Results

Load balancer successfully distributes traffic

Web servers configured automatically

Reduced manual configuration effort

Scalable web architecture on AWS

🧪 What I Learned

Automating infrastructure using Ansible

Configuring load balancers programmatically

Managing multiple hosts with Ansible

Writing reusable playbooks

Applying DevOps best practices

🔮 Future Enhancements

Add auto-scaling groups

Integrate with AWS ELB / ALB

Add HTTPS with SSL/TLS

Use dynamic EC2 inventory

Add monitoring and logging

