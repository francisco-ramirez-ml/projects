ArgoCD Skills Evaluation
Objective
The objective of this mini project is to evaluate your proficiency in using ArgoCD for
continuous delivery on Kubernetes. You will be required to perform tasks ranging from
basic setup and deployment to managing complex configurations and integrating with
CI/CD pipelines.
Project Tasks
Installing ArgoCD
Task: Install ArgoCD on your Kubernetes cluster. Verify the installation by accessing the
ArgoCD web UI.
Deliverable: Provide the steps and commands used to install ArgoCD and a screenshot
of the ArgoCD web UI.
Deploying a Simple Application with ArgoCD
Task: Create a simple Kubernetes deployment (e.g., Nginx) and deploy it using ArgoCD.
Use a Git repository as the source.
Deliverable: Provide the Git repository URL, the Kubernetes manifest files, and the steps
taken to deploy the application using ArgoCD.
Syncing Applications in ArgoCD
Task: Make a change to the deployed application (e.g., update the Nginx image version)
and sync the application using ArgoCD.
Deliverable: Provide the steps to make the change, sync the application, and a
screenshot of the ArgoCD UI showing the sync status.
Monitoring Application Status
Task: Monitor the status of the deployed application in ArgoCD and describe the
different statuses that an application can have.
Deliverable: Provide a description of the different application statuses and a screenshot
of the ArgoCD UI showing the status of your application.

Using ArgoCD Rollback
Task: Deploy a new version of the application with a breaking change and use ArgoCD to
rollback to the previous working version.
Deliverable: Provide the steps to deploy the new version, perform the rollback, and a
screenshot of the ArgoCD UI showing the rollback status.
Configuring Automatic Sync in ArgoCD
Task: Configure automatic synchronization for the deployed application in ArgoCD.
Deliverable: Provide the steps and configuration files used to enable automatic sync
and a screenshot of the ArgoCD UI showing the automatic sync settings.
Managing Secrets with ArgoCD and Sealed Secrets
Task: Use Kubernetes Sealed Secrets to manage sensitive data in your application
deployment and configure ArgoCD to use the sealed secrets.
Deliverable: Provide the steps, configuration files, and a description of how you used
Sealed Secrets with ArgoCD.
Deploying a Helm Chart with ArgoCD
Task: Create a Helm chart for your application and deploy it using ArgoCD. Use a Git
repository as the source.
Deliverable: Provide the Git repository URL, the Helm chart files, and the steps taken to
deploy the chart using ArgoCD.
Multi-Cluster Deployment with ArgoCD
Task: Configure ArgoCD to deploy applications to multiple Kubernetes clusters. Deploy
the same application to two different clusters.
Deliverable: Provide the steps and configuration files used to set up multi-cluster
deployment and a screenshot of the ArgoCD UI showing the applications in both
clusters.

Using ArgoCD ApplicationSets
Task: Use ArgoCD ApplicationSets to deploy multiple instances of an application with
different configurations.
Deliverable: Provide the steps, ApplicationSet configuration, and a screenshot of the
ArgoCD UI showing the deployed instances.
Integrating ArgoCD with GitHub Actions
Task: Set up a CI/CD pipeline using GitHub Actions to automatically deploy changes to
your application using ArgoCD.
Deliverable: Provide the GitHub Actions workflow file and a link to the repository.
Describe the steps to set up the CI/CD pipeline and verify a successful deployment.
ArgoCD Sync Waves
Task: Use ArgoCD sync waves to control the order in which resources are applied during
a sync operation.
Deliverable: Provide the steps, configuration files, and a description of how you used
sync waves in your deployment.
