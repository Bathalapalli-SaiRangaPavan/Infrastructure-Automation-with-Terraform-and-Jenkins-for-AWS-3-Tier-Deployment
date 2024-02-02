## Project Purpose
- This project focuses on deploying a 3-tier architecture on AWS using Terraform for infrastructure as code (IaC) automation.
- The deployment is orchestrated through a Jenkins pipeline, integrating Terraform, Ansible, and Terragrunt to ensure environment-specific deployments.
- The goal is to achieve a scalable and automated deployment process for a monolithic application.

## Infrastructure and Environment

- **Operating System:** Linux
- **Cloud Provider:** AWS
- **DNS Management:** Route53
- **SSL Certificates:** Certificate Manager
- **Notification Service:** SNS
- **Identity and Access Management:** IAM Roles
- **Instance Management:** Systems Manager (Session Manager)
- **Load Balancing:** Elastic Load Balancer (ELB)
- **Networking:** Virtual Private Cloud (VPC)
- **Internet Connectivity:** NAT Gateway
- **Monitoring:** CloudWatch Alarms
- **Artifact Storage:** S3 Bucket

## Application Stack

- **Application Deployment:** Spring Boot
- **Database:** MySQL
- **Build Tool:** Maven
- **Version Control:** Git
- **Web Server:** NGINX

## Automation Tools

- **Infrastructure as Code:** Terraform
- **Configuration Management:** Ansible
- **Deployment Orchestration:** Jenkins
- **Terragrunt:** for managing Terraform configurations

## Jenkins Pipeline

The Jenkins pipeline is the heart of the automated deployment process. It integrates Terraform, Ansible, and Terragrunt to ensure a smooth and environment-specific deployment.

1. **Checkout:** Jenkins pipeline starts by checking out the Terraform and Ansible scripts from BitBucket.

2. **Terraform Deployment:**
    - Terraform is used for provisioning AWS resources.
    - Different environments (dev, staging, prod) are managed using Terraform modules.
    - Jenkins triggers Terraform deployments based on environment parameters.

3. **Ansible Configuration:**
    - Ansible is employed for configuration management.
    - Plays are triggered as part of Terraform deployments, using user data sections.
    - Ensures consistent configuration across different instances.

4. **Terragrunt Integration:**
    - Terragrunt is utilized for managing Terraform configurations.
    - Enables code reusability and maintains modular structures for environments.

5. **Artifact Deployment:**
    - Jenkins pipeline deploys artifacts (Spring Boot application, configuration files) to EC2 instances.

6. **Database Setup:**
    - Automated database setup using Ansible to configure MySQL for the application.

7. **NGINX Configuration:**
    - NGINX is configured as a front-end web server to proxy requests to the backend Spring Boot application.

8. **Validation and Testing:**
    - Automated testing of the deployed infrastructure to ensure stability and functionality.

9. **Monitoring Integration:**
    - CloudWatch Alarms are set up to monitor CPU usage and trigger alerts if thresholds are breached.

10. **Notifications:**
    - SNS is integrated to send notifications for successful or failed deployments.

