Flask Docker POC
This is a proof of concept (POC) that demonstrates how to containerize a Flask web app using Docker. It shows how to build a Flask application, containerize it with Docker, and run it in a Docker container.

1. Features
Flask web app that responds with a simple message.

Containerized using Docker for easy deployment.

2. Prerequisites
Docker installed.

3. Project Structure
flask_docker_poc/

app.py # Flask application code

requirements.txt # Python dependencies

Dockerfile # Dockerfile for Flask app

4. Steps to Run the POC
4.1 Clone the repository:
bash
Copy
Edit
git clone <repository_url>
cd flask_docker_poc
4.2 Build the Docker image:
bash
Copy
Edit
docker build -t flask_docker_poc .
4.3 Run the Docker container:
bash
Copy
Edit
docker run -p 5000:5000 flask_docker_poc
4.4 Access the app:
Open your browser and visit http://localhost:5000. The Flask app should show a simple greeting message.

4.5 Stop the container:
To stop the container, press Ctrl+C in the terminal or use:

bash
Copy
Edit
docker stop <container_id>
5. How It Works
Flask is used to create a simple web application.

Docker containers the Flask app, making it easy to deploy across different environments without worrying about dependency issues.

The app listens on port 5000, which is exposed to the host machine so you can access it via localhost:5000.

