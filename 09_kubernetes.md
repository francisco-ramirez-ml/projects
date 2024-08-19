Kubernetes Skills Evaluation
Objective
The objective of this mini project is to evaluate your proficiency in using Kubernetes to
manage containerized applications. You will be required to perform tasks ranging from
basic to complex, demonstrating your understanding of Kubernetes concepts and best
practices.
Project Tasks
Kubernetes Cluster Setup:
Set up a local Kubernetes cluster using Minikube or Kind, K3s or use a cloud-
based Kubernetes service (e.g., GKE, EKS, AKS).
Task 1: Deploying and managing Pod
Create a nginx Pod using the imperative command with the dry-run clause to generate a
YAML file
Apply the YAML file to the cluster
How would you get detailed information about the nginx pod?
How would you Verify that the Pod is running?
Execute the command to view logs of the nginx pod
Execute a command in a running Pod (nginx) to check the configuration)
Port-forward a local port to a port on the Pod to access the application (8080:80)
Delete the nginx Pod
Create a new Pod with a mounted local volume. Create using imperative as well yaml
format.
Host path: /home/<user>/mylocalmount
mountPath: /usr/share/nginx/html
Task 2: Deployments and Services
Create an nginx Deployment with 3 replicas using the imperative command with dry-run
How would you verify the Deployment and replicas ?
Expose the nginx Deployment using a Service of type ClusterIP
Expose the nginx Deployment using a Service of type NodePort

Expose the nginx Deployment using a Service of type LoadBalancer
Scale the nginx Deployment to 5 replicas
Delete some of the Pods in the nginx Deployment
Observe the behavior of the Deployment and note down your observation.
Task 3: ConfigMaps and Secrets
Create a ConfigMap to store configuration data for a custom application.
APP_ENV=production
APP_DEBUG=false
How would you verify the created config map.
Create a Secret to store sensitive data (e.g., database credentials):
DB_USERNAME=<username>
DB_PASSWORD=<password>
How would you verify the created secrets?
Task 4: Persistent Volumes and Persistent Volume Claims
Create a Persistent Volume using the imperative command or YAML.
Use host path "/mnt/data"
How would you verfy the created PV
Create a Persistent Volume Claim using the imperative command or YAML
Task 5: Creating a StatefulSet
Create a StatefulSet for a MySQL database using the imperative command or YAML.
Task 6 : Horizontal Pod Autoscaler
Create a Horizontal Pod Autoscaler (HPA) to automatically scale the nginx Deployment
based on CPU utilization:
Task 7: Readiness and liveness probe
Add readiness and liveness probes to the nginx Deployment
Task 8: Set environment variables in a Pod
ENV=production
DEBUG=false

Task9: Namespace
Create a new namespace called test-namespace
Deploy a nginx Pod in the new namespace
List all namespaces in the cluster:
List all the nodes in the cluster
Get detailed information about a specific node
Task 10: Rolling update strategy
Create a Nginx Deployment with a rolling update strategy.
