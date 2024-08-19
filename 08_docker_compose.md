Docker Compose Evaluation Skills
Objective
The objective of this assignment is to evaluate your proficiency in using Docker
compose to manage multi container applications. You will be required to perform tasks
involving the creation and management of Docker compose files.
Project Tasks
Task 1 : Install Docker Compose
Ensure Docker Compose is installed on your local machine or use a cloud-based
instance with Docker Compose pre-installed.
Verify the Docker Compose installation by running the docker-compose --version
command.
Task 2: Basic Docker Compose Configuration
Create a Simple Web Application:
Create a directory named webapp.
Inside the webapp directory, create a file named index.html with the following content:
<!DOCTYPE html>
<html>
<head>
<title>Simple Web App</title>
</head>
<body>
<h1>Hello, Docker Compose!</h1>
</body>
</html>
Inside the webapp directory, create a Dockerfile that uses the nginx:latest image and
copies index.html to the appropriate location.
In the root directory (outside webapp), create a docker-compose.yml file that defines a
service named web which builds the webapp directory and exposes it on port 8080.

Build and start the application using docker-compose
Stop and remove the containers using docker-compose
Task 3: Adding a Database Service
Extend the Docker Compose File:
Extend the docker-compose.yml file to include a MySQL database service named db
with the following environment variables:
MYSQL_ROOT_PASSWORD: example
MYSQL_DATABASE: webapp_db
MYSQL_USER: user
MYSQL_PASSWORD: password
Build and Run the Application. Take the screenshot
Verify that both services are running . Take the screenshot
Task 4 : Multicontainer Application with networking
Create a Flask Application:
Create a directory named flaskapp.
Inside the flaskapp directory, create a file named app.py with the following
content
from flask import Flask, request
import mysql.connector
app = Flask(__name__)
@app.route('/')
def hello_world():
return 'Hello, Docker Compose with Flask!'
@app.route('/db')
def db_test():
conn = mysql.connector.connect(
host='db',
user='user',

password='password',
database='webapp_db'
)
cursor = conn.cursor()
cursor.execute('SELECT DATABASE()')
db_name = cursor.fetchone()[0]
cursor.close()
conn.close()
return f'Connected to database: {db_name}'
if __name__ == '__main__':
app.run(host='0.0.0.0', port=5000)
Inside the flaskapp directory, create a requirements.txt file with the following content:
Flask==2.0.1
mysql-connector-python==8.0.23
Inside the flaskapp directory, develop a Dockerfile
In the root directory (outside flaskapp), develop a docker-compose.yml
Build and Run the Application using docker compose
Verify that the application is accessible at http://localhost:5000.
Access the /db route to verify the connection to the database:
curl http://localhost:5000/db
Task 5: Extend the docker-compose.yml file to include a Redis cache service
Update app.py to use Redis is as below :
from flask import Flask, request
import mysql.connector
import redis

app = Flask(__name__)
cache = redis.Redis(host='redis', port=6379)
@app.route('/')
def hello_world():
return 'Hello, Docker Compose with Flask and Redis!'
@app.route('/db')
def db_test():
conn = mysql.connector.connect(
host='db',
user='user',
password='password',
database='webapp_db'
)
cursor = conn.cursor()
cursor.execute('SELECT DATABASE()')
db_name = cursor.fetchone()[0]
cursor.close()
conn.close()
return f'Connected to database: {db_name}'
@app.route('/cache')
def cache_test():
cache.set('message', 'Hello from Redis!')
return cache.get('message').decode('utf-8')

if __name__ == '__main__':
app.run(host='0.0.0.0', port=5000)
Rebuild and start the application using docker compose
Verify that the application is accessible at http://localhost:5000.
Access the /cache route to verify the connection to the Redis cache:
curl http://localhost:5000/cache
