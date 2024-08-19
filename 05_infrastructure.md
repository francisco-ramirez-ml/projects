CICD – Infrastructure
Objective
The objective of this mini project is to evaluate your proficiency in developing CI/CD
pipelines using Jenkins, Azure Pipelines, and GitHub Actions. You will be required to
create CI/CD pipelines for Terraform Automation.
Task1 : Jenkins pipeline
Create a Jenkins pipeline (Jenkinsfile) that:
Checks out the code from your GitHub repository.
Initializes Terraform.
Validates the Terraform configuration.
Plans the Terraform deployment.
Applies the Terraform configuration to create AWS/Azure resources .
Use Jenkins credentials plugin to manage AWS and Azure secrets securely.
Configure the pipeline to run automatically when changes are pushed to the
main branch.
Verify the pipeline execution and resource creation on AWS/Azure
Task2: Azure Pipeline
Create an Azure Pipeline (azure-pipelines.yml) that:
Checks out the code from your GitHub repository.
Installs Terraform.
Initializes Terraform.
Validates the Terraform configuration.
Plans the Terraform deployment.
Applies the Terraform configuration to create AWS/Azure resources
Configure the pipeline to trigger automatically on changes to the main branch.
Use Azure key Vault/pipeline variables securely manage all the credentials
Verify the pipeline execution and resource creation on AWS/Azure

Task 3: GitHub Actions
Create a GitHub Actions workflow (gt-terraform.yml) that:
Checks out the code from your GitHub repository.
Sets up Terraform.
Initializes Terraform.
Validates the Terraform configuration.
Plans the Terraform deployment.
Applies the Terraform configuration to create AWS/Azure resources.
Use GitHub Secrets to securely manage AWS/Azure credentials.
Configure the workflow to trigger automatically on changes to the main branch.
Verify the workflow execution and resource creation on AWS/Azure
