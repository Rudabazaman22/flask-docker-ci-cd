# Docker + GitHub Actions CI/CD Project Documentation

## Project Goal

Build a simple Flask web application, containerize it using Docker, automate image build & push using GitHub Actions, and deploy it using Docker.


## Tools Used

| Tool            | Purpose                 |
| --------------- | ----------------------- |
| Python + Flask  | Backend web application |
| Docker          | Containerization        |
| DockerHub       | Image registry          |
| GitHub          | Code version control    |
| GitHub Actions  | CI/CD automation        |
| WSL2 / Terminal | Command-line interface  |

---

## Project Structure

```
flask-docker-ci-cd/
├── app.py
├── requirements.txt
├── Dockerfile
└── .github/
    └── workflows/
        └── docker-ci.yml

### Run the Container:

in bash run
docker run -d -p 5000:5000 rudaba/flask-docker-ci-cd

### View Running Containers:

in bash run to see all the list
docker ps

### Stop the Container:

in bash run if docker needs to stop
docker stop <CONTAINER_ID>


## GitHub Actions Output Example (in Actions tab)
Checkout code
Log in to DockerHub
Build Docker image
Push Docker image

## End Result

* Docker container runs a live Flask app
* CI/CD pipeline builds and pushes new images on every commit to `main`
* Fully reproducible, portable, and automated
