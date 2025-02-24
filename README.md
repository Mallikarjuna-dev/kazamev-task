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

### Backend Setup

- Clone the repository:

git clone https://github.com/your-username/todo-list-ws.git
cd todo-list-ws

- Install dependencies:

npm install

- Start the backend server:

npm run dev

### Frontend Setup

- Navigate to the frontend directory:

cd frontend

- Install dependencies:

npm install

- Start the frontend server:

npm run start
