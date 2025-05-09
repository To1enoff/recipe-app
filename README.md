# 🍽️ Recipe Guide App
A simple web application that lets users search for meals and view recipes using the TheMealDB API.
Built with HTML/CSS/JavaScript, served via Nginx in a Docker container, and powered by GitHub Actions CI/CD.

# 🚀 Features
Search recipes by dish name

View meal details and instructions

Responsive UI with clean design

Hosted in a Docker container using Nginx

CI/CD pipeline with GitHub Actions

# 🐳 Docker
Build & Run with Docker
```
docker build -t recipe-app .
docker run -p 8080:80 recipe-app
```
Or use Docker Compose
```
docker compose up -d --build
```
Then open http://localhost:8080 in your browser.

# ⚙️ CI/CD Pipeline (GitHub Actions)
Whenever changes are pushed to the main branch:

GitHub Actions builds the Docker image.

The image is pushed to DockerHub (to1enoff/recipe-app).

Credentials are securely handled via GitHub Secrets.

Secrets required:

DOCKER_USERNAME = to1enoff

DOCKER_PASSWORD = your DockerHub password or access token

📁 Project Structure
pgsql

```
.
├── Dockerfile
├── docker-compose.yml
├── index.html
├── .github
│   └── workflows
│       └── docker-deploy.yml
└── README.md
```
# 📦 Image on DockerHub
Pull the latest image:

bash
```
docker pull to1enoff/recipe-app:
``` 
# 📝 License
This project is open-source and available under the MIT License.
