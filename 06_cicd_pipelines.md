CI/CD Pipelines - Applications
Objective
The objective of this mini project is to evaluate your proficiency in developing CI/CD
pipelines using Jenkins, Azure Pipelines, and GitHub Actions. You will be required to
create CI/CD pipelines for a Python application, a Node.js application, and a Java
application. Each pipeline should include a build stage and a deploy stage, with
deployments to Dev, Test, and Prod environments.
Project Tasks
Python Application
1. Python Application Setup
Create a Simple Flask Application:
Create a directory named python-app.
Inside the python-app directory, create a file named app.py containing a simple Flask
application that returns a "Hello, CI/CD with Flask!" message.
Create a requirements.txt file that includes the necessary dependencies for the Flask
application.
2. Jenkins Pipeline for Python Application
Create a Jenkins Pipeline:
Create a Jenkinsfile in the root of the python-app directory.
The pipeline should have a build stage that installs dependencies and packages the
application into an artifact (e.g., a tarball).
The pipeline should have deploy stages to deploy the artifact to Dev, Test, and Prod
environments. Use SCP and SSH commands to transfer the artifact and run the
application on remote servers.
3. Azure Pipelines for Python Application
Create an Azure Pipelines Configuration:
Create an azure-pipelines.yml file in the root of the python-app directory.
The pipeline should have a build stage that installs dependencies and packages the
application into an artifact.

The pipeline should have deploy stages to deploy the artifact to Dev, Test, and Prod
environments. Use appropriate tasks to transfer the artifact and run the application on
remote servers.
4. GitHub Actions for Python Application
Create a GitHub Actions Workflow:
Create a .github/workflows/main.yml file in the root of the python-app directory.
The workflow should have a build job that installs dependencies and packages the
application into an artifact.
The workflow should have deploy jobs to deploy the artifact to Dev, Test, and Prod
environments. Use appropriate actions to transfer the artifact and run the application
on remote servers.
Node.js Application
1. Node.js Application Setup
Create a Simple Express Application:
Create a directory named nodejs-app.
Inside the nodejs-app directory, create a file named app.js containing a simple Express
application that returns a "Hello, CI/CD with Express!" message.
Create a package.json file that includes the necessary dependencies for the Express
application.
2. Jenkins Pipeline for Node.js Application
Create a Jenkins Pipeline:
Create a Jenkinsfile in the root of the nodejs-app directory.
The pipeline should have a build stage that installs dependencies and packages the
application into an artifact (e.g., a tarball).
The pipeline should have deploy stages to deploy the artifact to Dev, Test, and Prod
environments. Use SCP and SSH commands to transfer the artifact and run the
application on remote servers.
3. Azure Pipelines for Node.js Application
Create an Azure Pipelines Configuration:
Create an azure-pipelines.yml file in the root of the nodejs-app directory.

The pipeline should have a build stage that installs dependencies and packages the
application into an artifact.
The pipeline should have deploy stages to deploy the artifact to Dev, Test, and Prod
environments. Use appropriate tasks to transfer the artifact and run the application on
remote servers.
4. GitHub Actions for Node.js Application
Create a GitHub Actions Workflow:
Create a .github/workflows/main.yml file in the root of the nodejs-app directory.
The workflow should have a build job that installs dependencies and packages the
application into an artifact.
The workflow should have deploy jobs to deploy the artifact to Dev, Test, and Prod
environments. Use appropriate actions to transfer the artifact and run the application
on remote servers.
Java Application
1. Java Application Setup
Create a Simple Spring Boot Application:
Create a directory named java-app.
Inside the java-app directory, generate a basic Spring Boot application using the Spring
Initializr (https://start.spring.io/). Include dependencies for Spring Web.
Extract the generated project into the java-app directory.
2. Jenkins Pipeline for Java Application
Create a Jenkins Pipeline:
Create a Jenkinsfile in the root of the java-app directory.
The pipeline should have a build stage that uses Maven to build the application and
produce a JAR file.
The pipeline should have deploy stages to deploy the JAR file to Dev, Test, and Prod
environments. Use SCP and SSH commands to transfer the artifact and run the
application on remote servers.
3. Azure Pipelines for Java Application
Create an Azure Pipelines Configuration:
Create an azure-pipelines.yml file in the root of the java-app directory.

The pipeline should have a build stage that uses Maven to build the application and
produce a JAR file.
The pipeline should have deploy stages to deploy the JAR file to Dev, Test, and Prod
environments. Use appropriate tasks to transfer the artifact and run the application on
remote servers.
4. GitHub Actions for Java Application
Create a GitHub Actions Workflow:
Create a .github/workflows/main.yml file in the root of the java-app directory.
The workflow should have a build job that uses Maven to build the application and
produce a JAR file.
The workflow should have deploy jobs to deploy the JAR file to Dev, Test, and Prod
environments. Use appropriate actions to transfer the artifact and run the application
on remote servers.
