Kubernetes Helm Charts Skills Evaluation
Objective
The objective of this mini project is to evaluate your proficiency in using Helm charts to
manage Kubernetes applications. You will be required to perform tasks ranging from
creating and deploying Helm charts to managing complex configurations and
integrating with CI/CD pipelines.
Project Tasks
Installing Helm
Task: Install Helm on your local machine or Kubernetes cluster. Verify the installation by
running helm version.
Deliverable: Provide the steps and commands used to install Helm and the output of
helm version.
Creating a Simple Helm Chart
Task: Create a new Helm chart named my-app using the helm create command.
Explore the directory structure and describe the purpose of each file.
Deliverable: Provide the commands used to create the Helm chart and a brief
explanation of each file in the chart directory.
Deploying a Helm Chart
Task: Deploy the my-app Helm chart to your Kubernetes cluster using the helm install
command.
Deliverable: Provide the commands used to deploy the Helm chart and the output of
helm ls showing the deployed release.
Customizing Values in a Helm Chart
Task: Customize the my-app Helm chart by modifying the values.yaml file to change the
replica count and service type. Deploy the updated chart.
Deliverable: Provide the modified values.yaml file, the commands used to deploy the
chart, and the output of kubectl get pods,svc showing the changes.

Creating a ConfigMap with Helm
Task: Update the my-app Helm chart to include a ConfigMap that contains application
configuration data. The ConfigMap should be created from a file in the templates
directory.
Deliverable: Provide the updated Helm chart files and the commands used to deploy
the chart. Verify the ConfigMap creation with kubectl get configmaps.
Using Helm Hooks
Task: Add a Helm pre-install hook to the my-app chart that creates a ConfigMap before
the main application pods are deployed.
Deliverable: Provide the updated Helm chart files with the pre-install hook and the
commands used to deploy the chart. Verify the hook execution with kubectl get
configmaps.
Creating a Helm Chart with Dependencies
Task: Create a new Helm chart named my-webapp that depends on the nginx chart
from the Helm stable repository. Define the dependency in the Chart.yaml file and
deploy the chart.
Deliverable: Provide the Chart.yaml file with the dependency definition and the
commands used to add the repository and deploy the chart. Verify the deployment with
helm ls and kubectl get pods.
Templating with Helm
Task: Modify the my-app Helm chart to use Helm templating features to dynamically set
the image tag and replica count based on values provided in values.yaml.
Deliverable: Provide the updated Helm chart templates and values.yaml file. Deploy the
chart with different values and provide the commands and output verifying the changes.
Creating a Helm Library Chart
Task: Create a Helm library chart named common-library with common templates that
can be reused in other Helm charts. Include a template for a ConfigMap and a
deployment.
Deliverable: Provide the common-library chart files and an example chart that uses this
library chart. Deploy the example chart and verify the deployment.

Helm Chart Testing
Task: Add a Helm test to the my-app chart that verifies the application is running
correctly. The test should run a simple curl command to check the application's health
endpoint.
Deliverable: Provide the updated Helm chart files with the test configuration and the
commands used to run the test. Verify the test results with helm test.
Helm Chart Rollback
Task: Deploy a new version of the my-app chart with a breaking change. Perform a Helm
rollback to the previous working version.
Deliverable: Provide the commands used to deploy the new version, verify the issue,
and perform the rollback. Provide the output of helm ls and kubectl get pods showing
the rollback.
Integrating Helm with CI/CD
Task: Set up a CI/CD pipeline using GitHub Actions to automatically deploy the my-app
Helm chart to a Kubernetes cluster on every push to the main branch.
Deliverable: Provide the GitHub Actions workflow file and a link to the repository.
Describe the steps to set up the CI/CD pipeline and verify a successful deployment
