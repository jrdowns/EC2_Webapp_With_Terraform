# EC2_Webapp_With_Terraform

## Overview
Purpose: Use Terraform to provision a web server environment in AWS  
Author: James Downs  
Date: 8/17/2022  

### Resources
- VPC  
- MySQL RDS  
- NGINX Web server
- Application Load balancer
- HTTP Listener

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
## Terraform Steps
### `terraform init`
The terraform init command is used to initialize a working directory containing Terraform configuration files. This command performs several different initialization steps in order to prepare the current working directory for use with Terraform. During init, the configuration is searched for module blocks, and the source code for referenced modules is retrieved from the locations given in their source arguments.

### `terraform plan`
The terraform plan command creates an execution plan, which lets you preview the changes that Terraform plans to make to your infrastructure. You can save the plan to a binary file for execution later with `terraform plan -out <file name>`. You can save a terraform plan as JSON with `terraform show -json <file name>`

### `terraform apply`
The terraform apply command executes the actions proposed in a Terraform plan. When you run terraform apply without passing a saved plan file, Terraform automatically creates a new execution plan as if you had run terraform plan, prompts you to approve that plan, and takes the indicated actions.

### `terraform destroy`
The terraform destroy command is a convenient way to destroy all remote objects managed by a particular Terraform configuration. Since this is just for pratice, I'll destroy the environment after it's been created.
