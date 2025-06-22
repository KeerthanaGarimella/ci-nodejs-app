# CI/CD Midterm - Node.js App

## Overview
This is a simple Node.js application used to demonstrate a CI pipeline with GitHub Actions.

## Project Setup
1. Clone the repo
2. Run `npm install`
3. Run `npm start`

## CI Pipeline Stages
- **Build:** Installs dependencies
- **Lint:** Runs ESLint on the codebase
- **Test:** Runs Jest unit tests
- **Docker:** Builds and pushes Docker image to DockerHub

## Docker
```bash
docker pull <your-docker-username>/ci-nodejs-app:develop
docker run -p 3000:3000 <your-docker-username>/ci-nodejs-app:develop
```

## Deployment
- `develop` branch triggers `dev` deployment
- `main` branch or manual trigger handles `prod`
