# EC2_Webapp_With_Terraform

## Overview
Purpose: Use Terraform to provision a web server environment in AWS  
Author: James Downs  
Date: 8/17/2022  

### Project Structure
📦EC2_Webapp_With_Terraform  
 ┣ 📂module  
 ┃ ┣ 📂rds  
 ┃ ┃ ┣ 📜rds.tf  
 ┃ ┃ ┗ 📜varaible.tf  
 ┃ ┗ 📂vpc  
 ┃ ┃ ┣ 📜varaible.tf  
 ┃ ┃ ┗ 📜vpc.tf  
 ┣ 📂webserver  
 ┃ ┣ 📜varaible.tf  
 ┃ ┣ 📜webserver_alb.tf  
 ┃ ┗ 📜webserver_instance.tf  
 ┣ 📜README.md  
 ┣ 📜main.tf  
 ┗ 📜varaible.tf  
---

