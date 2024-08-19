Ansible Skills Evaluation
Objective
The objective of this mini project is to evaluate your proficiency in using Ansible for
configuration management and automation. You will be required to perform tasks ranging
from basic setup and playbook creation to managing complex configurations and integrating
with other tools.
Project Tasks
Basic Questions
1. Installing Ansible
o Task: Install Ansible on your local machine. Verify the installation by running
ansible --version.
o Deliverable: Provide the steps and commands used to install Ansible and the
output of ansible --version.
2. Creating an Inventory File
o Task: Create a simple Ansible inventory file that defines a group of hosts (e.g.,
webservers) with at least two hosts (these can be local VMs, cloud instances,
or any other accessible machines).
o Deliverable: Provide the inventory file and a description of the hosts
included.
3. Running Ad-Hoc Ansible Commands
o Task: Use Ansible ad-hoc commands to perform basic operations (e.g., ping
all hosts, check disk usage) on the hosts defined in your inventory file.
o Deliverable: Provide the ad-hoc commands used and the output of each
command.
Intermediate Questions
4. Creating a Simple Playbook
o Task: Write a simple Ansible playbook to install Nginx on all hosts in the
webservers group. Ensure Nginx is started and enabled to start on boot.
o Deliverable: Provide the playbook and the commands used to run it. Verify
the installation by accessing Nginx on each host.
5. Using Variables in Playbooks
o Task: Modify the Nginx playbook to use variables for the package name and
service name. Define these variables in a separate file and include them in
the playbook.
o Deliverable: Provide the updated playbook, the variables file, and the
commands used to run the playbook.
6. Creating and Using Templates
o Task: Create an Ansible template for an Nginx configuration file using Jinja2
templating. Update the playbook to deploy this template to the hosts and
restart Nginx.

o Deliverable: Provide the template file, the updated playbook, and the
commands used to run the playbook. Verify the new configuration by
accessing Nginx.
7. Handling Handlers in Playbooks
o Task: Modify the Nginx playbook to use handlers. Ensure that Nginx is
restarted only if the configuration file is changed.
o Deliverable: Provide the updated playbook with handlers and the commands
used to run the playbook. Verify the handler execution by making a change to
the configuration file.
Advanced Questions
8. Using Ansible Roles
o Task: Create an Ansible role for installing and configuring Nginx. Structure the
role according to Ansible best practices and use it in your playbook.
o Deliverable: Provide the role files and directory structure, the updated
playbook that includes the role, and the commands used to run the playbook.
9. Managing Users and Groups
o Task: Write an Ansible playbook to create a new user and group on all hosts.
Ensure the user has specific sudo privileges.
o Deliverable: Provide the playbook and the commands used to run it. Verify
the user creation and sudo privileges on each host.
10. Using Ansible Vault
o Task: Secure sensitive data (e.g., user passwords) in your playbook using
Ansible Vault. Encrypt the variables file containing the sensitive data.
o Deliverable: Provide the steps to create and encrypt the variables file, the
updated playbook, and the commands used to run the playbook with Ansible
Vault.
11. Deploying a Web Application
o Task: Write an Ansible playbook to deploy a simple web application (e.g., a
Flask or Node.js app) on the webservers. Ensure the application is started and
enabled to start on boot.
o Deliverable: Provide the playbook and the commands used to run it. Verify
the application deployment by accessing it on each host.
12. Configuring Load Balancing with Ansible
o Task: Write an Ansible playbook to install and configure HAProxy as a load
balancer for your web application. Ensure the load balancer distributes traffic
across the webservers.
o Deliverable: Provide the playbook and the commands used to run it. Verify
the load balancing setup by accessing the web application through the load
balancer.

Complex Questions
13. Integrating Ansible with CI/CD
o Task: Set up a CI/CD pipeline using Jenkins to automatically run your Ansible
playbook for deploying the web application whenever there is a change in the
application code repository.
o Deliverable: Provide the Jenkins pipeline configuration, the playbook, and a
link to the application code repository. Verify the CI/CD integration by making
a change to the repository and observing the deployment.
14. Using Dynamic Inventory
o Task: Configure Ansible to use a dynamic inventory script for managing cloud
instances (e.g., AWS EC2 instances). Deploy the Nginx playbook to instances
managed by the dynamic inventory.
o Deliverable: Provide the dynamic inventory script, the updated playbook, and
the commands used to run the playbook. Verify the deployment by accessing
Nginx on the cloud instances.
15. Automating Database Setup
o Task: Write an Ansible playbook to install and configure a MySQL database on
a separate group of hosts (e.g., dbservers). Ensure the database is started
and enabled to start on boot.
o Deliverable: Provide the playbook and the commands used to run it. Verify
the database setup by connecting to it from one of the webservers and
creating a sample database.
