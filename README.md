# MERN Management System (CRUD)

A simple Employee Management System built with the MERN stack.

## Tech Stack

- MongoDB
- Express.js
- React (Vite)
- Node.js

## Features

- Create employee records
- Read/list all employees
- Update existing employees
- Delete employees
- Search employees by name, department, role, or email

## Project Structure

```text
.
|-- backend
|   |-- package.json
|   `-- src
|       |-- config
|       |   `-- db.js
|       |-- controllers
|       |   `-- employeeController.js
|       |-- models
|       |   `-- Employee.js
|       |-- routes
|       |   `-- employeeRoutes.js
|       `-- server.js
`-- frontend
    |-- package.json
    |-- index.html
    |-- vite.config.js
    `-- src
        |-- App.jsx
        |-- main.jsx
        `-- styles.css
```

## Run Locally (Without Docker)

1. Install MongoDB and make sure it is running locally.
2. Configure environment files:
   - Copy `backend/.env.example` to `backend/.env`
   - Copy `frontend/.env.example` to `frontend/.env`
3. Install dependencies:

```bash
cd backend
npm install
cd ../frontend
npm install
```

## Run

Start backend:

```bash
cd backend
npm run dev
```

Start frontend in another terminal:

```bash
cd frontend
npm run dev
```

Open the app:

```text
http://localhost:5173
```

Local backend API base URL:

```text
http://localhost:5000/api
```

## API Endpoints

- `GET /api/employees`
- `GET /api/employees/:id`
- `POST /api/employees`
- `PUT /api/employees/:id`
- `DELETE /api/employees/:id`
