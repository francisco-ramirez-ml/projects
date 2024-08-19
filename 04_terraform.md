Terraform Skills Evaluation
Objective
The objective of this mini project is to evaluate your proficiency in developing Terraform
scripts. You will be required to develop scripts for AWS, Aure and GCP cloud
environments.
Project Tasks
Task 1: Basic Terraform Configuration (AWS)
Create a Terraform configuration file (main.tf) that:
Defines a provider for AWS.
Creates an AWS S3 bucket.
Creates an AWS EC2 instance in a specified region.
Initialize Terraform in your project directory and apply the configuration.
Verify the creation of the S3 bucket and EC2 instance using the AWS
Management Console.
Task 2: Basic Terraform Configuration (Azure)
Create a Terraform configuration file (main.tf) that:
Defines a provider for Azure.
Creates an Azure Resource Group.
Creates an Azure Virtual Network (VNet) and a subnet.
Initialize Terraform in your project directory and apply the configuration.
Verify the creation of the Resource Group, VNet, and subnet using the Azure
Portal.
Task 3: Intermediate Terraform Configuration (AWS)
Extend your AWS Terraform configuration to:
Create an IAM role and attach a policy to allow S3 read-only access.
Create an RDS instance with a MySQL database inside a VPC.
Output the RDS endpoint and the EC2 instance public IP address.
Apply the configuration and verify the resources.

Modify the configuration to add a tag to all created resources and apply the
changes.
Task 4: Intermediate Terraform Configuration (Azure)
Extend your Azure Terraform configuration to:
Create an Azure Storage Account.
Create an Azure Virtual Machine (VM) in the subnet created earlier.
Create an Azure SQL Database inside the VNet.
Output the VM's public IP address and the SQL Database server name.
Apply the configuration and verify the resources.
Modify the configuration to add tags to all created resources and apply the
changes.
Task 5: Advanced Terraform Configuration (AWS)
Create a new Terraform module for AWS that:
Takes the S3 bucket name, EC2 instance type, and RDS instance type as input
variables.
Creates the S3 bucket, EC2 instance, and RDS instance as defined in Task 3.
Outputs the S3 bucket name, EC2 instance public IP, and RDS endpoint.
Use these modules in your main Terraform configuration files to provision the
resources with different input variables.
Use the output variables from the AWS module to create a new S3 bucket policy
that allows access from the EC2 instance.
Apply the configurations and verify the resources.
Task 6: Advanced Terraform Configuration (Azure)
Create a new Terraform module for Azure that:
Takes the Resource Group name, VM size, and Storage Account SKU as input
variables.
Creates the Resource Group, Virtual Network, subnet, Storage Account, VM, and
SQL Database as defined in Task 4.
Outputs the Storage Account name, VM public IP, and SQL Database server
name.

Use these modules in your main Terraform configuration files to provision the
resources with different input variables.
Use the output variables from the Azure module to create a new Network
Security Group (NSG) rule that allows access to the SQL Database only from the VM.
Apply the configurations and verify the resources.
Task 7: Terraform State Management and Remote Backend
Configure a remote backend for your AWS Terraform state using an S3 bucket state
locking.
Configure a remote backend for your Azure Terraform state using Azure Storage
Account.
Migrate your existing Terraform state to the remote backend and verify the setup.
