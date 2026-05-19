# Task Manager - DevOps Assignment

A simple Task Manager web application with full CI/CD pipeline.

## Tech Stack
- **Frontend:** HTML, CSS, JavaScript
- **Backend:** Node.js, Express
- **Database:** MongoDB Atlas
- **Container:** Docker
- **CI/CD:** GitHub Actions

## Features
- Add tasks
- View all tasks
- Delete tasks

## How To Run Locally

### Prerequisites
- Node.js v20
- MongoDB Atlas account
- Docker

### Steps
1. Clone the repository
   git clone https://github.com/buddhisankalana/task-manager-devops.git

2. Install dependencies
   cd backend
   npm install

3. Create .env file in backend/
   MONGO_URI=your_mongodb_uri
   PORT=5000

4. Start the server
   node server.js

5. Open frontend/index.html in browser

## CI/CD Pipeline
- Push to main branch triggers GitHub Actions
- Pipeline installs dependencies
- Runs tests
- Builds Docker image
- Pushes image to Docker Hub

## Docker
- Pull image: docker pull buddhisankalana/task-manager-app:latest
- Run: docker run -p 5000:5000 --env MONGO_URI=your_uri buddhisankalana/task-manager-app:latest
