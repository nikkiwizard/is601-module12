## Module 12

## DockerHub URL:
https://hub.docker.com/repository/docker/nikkiwizard/601_module12/general

## Github Actions Run:
![Actions](screenshots/actions.png "Github Actions Workflow screenshot")

## DockerHub Screenshot:
![DockerHub](screenshots/dockerhub.png "Dockerhub screenshot")

## App Screenshot:
![Application](screenshots/app.png "Application screenshot")

## Running Tests
Before running tests, be sure that Docker is up and running with the following command: <br>
docker compose up --build

To run tests locally, follow these commands: <br>
python3 -m venv venv <br>
source venv/bin/activate <br>
pip install -r requirements.txt <br>
docker compose exec web pytest <br>

A note: You could run pytest instead of docker compose exec web pytest but I had some trouble with just pytest. <br>

You can also manually test your application by doing manual checks via OpenAPI going to http://localhost:8000/docs. You can test registration, login, auth, and all the calculation endpoints by clicking "Try it out". 