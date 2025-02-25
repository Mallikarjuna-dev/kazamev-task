# To-Do List Application (WebSockets & HTTP)

This is a full-stack to-do list application built using Node.js, WebSockets (Socket.io), Redis, MongoDB, and React.js. The application allows users to add tasks via WebSockets, store them in Redis, and migrate older tasks to MongoDB. A frontend is also provided to interact with the API.

## Features

- Add new tasks using WebSockets (add event)

- Store tasks temporarily in Redis (FULLSTACK*TASK*<YOUR_FIRST_NAME> key)

- Automatically move tasks to MongoDB if the count exceeds 50

- Retrieve all tasks via an HTTP API (/fetchAllTasks endpoint)

- Frontend UI (React.js) with CSS/SCSS for styling

- Responsive design for mobile and tablet screens

- Reusable components for maintainability

## Tech Stach

- Backend: Node.js, Express, WebSockets (Socket.io), Redis, MongoDB

- Frontend: React.js.js with CSS/SCSS (Tailwind css)

- Database: Redis (caching) & MongoDB (persistent storage)

## Setup Instructions

- Prerequisites

- Node.js installed

- Redis server access

- MongoDB Atlas access

### Project tructure


/kazamev-task
├── backend
│   ├── configs
│   │    └── config.js
│   ├── models
│   │    └──Task.js
│   ├── routes
│   │    └── taskRoutes.js
│   ├── server.js
│   ├── .gitignore
│   ├── package.json
│   ├── .env
├── frontend
│   ├── src
│   │   ├── components
│   │   │   ├──Task.js
│   │   │   └──TaskList.js
│   │   ├── App.js
│   │   ├── index.js
│   │   ├── App.css/
│   ├── .gitignore
│   ├── package.json
│   ├── tailwind.config.js
└── README.md


### Backend Setup

- Clone the repository:

git clone https://github.com/your-username/todo-list-ws.git
cd todo-list-ws

- Install dependencies:

npm install

Create a .env file in the root directory and add the following credentials:

REDIS*HOST=redis-12675.c212.ap-south-1-1.ec2.cloud.redislabs.com
REDIS_PORT=12675
REDIS_USERNAME=default
REDIS_PASSWORD=dssYpBnYQrl01GbCGVhVq2e4dYvUrKJB
MONGO_URI=mongodb+srv://assignment_user:HCgEj5zv8Hxwa4xO@test-cluster.6f94f5o.mongodb.net/
DB_NAME=assignment
COLLECTION_NAME=assignment*<YOUR_FIRST_NAME>

- Start the backend server:
```
npm run dev
```
### Frontend Setup

- Navigate to the frontend directory:
```
cd frontend
```
- Install dependencies:
```
npm install
```
- Start the frontend server:
```
npm run start
```
### API Endpoints

Method

- GET

Endpoint

```
/fetchAllTasks
```
Fetch all tasks from DB

### URLs

Backend (Localhost): http://localhost:8080

Frontend (Localhost): http://localhost:3000

Deployed Backend: https://kazam-ev-task.onrender.com

Deployed Frontend: https://kazamev-task.vercel.app/
