Docker Skills Evaluation
Objective
The objective of this project is to evaluate your proficiency in using Docker to
containerize applications, manage images and containers and work with Dockerfiles.
You will be required to perform tasks ranging from basic to complex, demonstrating your
understanding of Docker concepts and best practices.
Project Tasks
Task 1: Basic Docker Commands
Docker Installation and Setup:
Install Docker on your local machine or use a cloud-based instance with Docker
pre-installed.
Verify the Docker installation by running the docker --version command.
Hello World Container:
Run the official Docker "hello-world" container and verify its output.
Remove the "hello-world" container after verification.
Basic Container Management:
Pull the nginx image from Docker Hub.
Run an nginx container in detached mode.
List all running containers.
Stop the nginx container.
Remove the nginx container.
Run the nginx container again and map port 8080 on the host to port 80 in the
container.
Inspect the nginx container to view its details.
Rename the running nginx container to my_nginx.
View the logs of the my_nginx container.
Restart the my_nginx container.

Task 2: Dockerfile and Custom Image Creation
Creating a Dockerfile to dockerize following python flask application
Flask application:
-----------------------------------------------------------
# app.py
from flask import Flask
app = Flask(__name__)
@app.route('/')
def hello_world():
return 'Hello, World!'
if __name__ == '__main__':
app.run(host='0.0.0.0', port=5000)
------------------------------------------------------------------------
Building and Running the Custom Image:
Build the Docker image from the Dockerfile with the tag flask-app.
Run a container from the flask-app image in detached mode, mapping port 5000 on the
host to port 5000 in the container.
Verify that the application is accessible at http://localhost:5000 or the appropriate IP if
using a cloud-based instance.
Stop and remove the container.
Task 3: Image Management and Docker Hub
Image Tagging and Pushing to Docker Hub:
Tag the flask-app image with your Docker Hub username and a version tag (e.g.,
v1).
Push the tagged image to your Docker Hub repository.
Provide the link to the Docker Hub repository containing the flask-app image.

Managing Images:
List all Docker images on your local machine.
Remove the local flask-app image.
Task 4: Intermediate Container Operations
Data Persistence with Volumes:
Modify the Dockerfile to include a volume for the /data directory.
Rebuild the flask-app image.
Run a container from the new flask-app image, mounting a local directory
(/path/to/local/data) to the /data directory in the container.
Verify that files created in the /data directory inside the container are persisted to
the local directory on the host.
Environment Variables:
Modified the Flask application to read a message from an environment variable is as
below
-------------------------------------------------------------------
import os
from flask import Flask
app = Flask(__name__)
@app.route('/')
def hello_world():
message = os.getenv('MESSAGE', 'Hello, World!')
return message
if __name__ == '__main__':
app.run(host='0.0.0.0', port=5000)
----------------------------------------------------------------------------------
Update the Dockerfile to include the ENV instruction for the MESSAGE environment
variable.

Rebuild the flask-app image.
Run a container from the updated flask-app image, passing a custom message as an
environment variable.
Verify that the custom message is displayed when accessing the application.
Task 5: Advanced Docker Concepts
Multi-Stage Builds:
Optimize the Dockerfile to use multi-stage builds for reducing the final image size.
Health Checks:
Add a health check to the Dockerfile to ensure the container is running correctly.
HEALTHCHECK --interval=30s --timeout=10s --retries=3 CMD curl -f
http://localhost:5000/ || exit 1
Rebuild the flask-app image and run a container from the updated image.
Verify the health status of the running container.
