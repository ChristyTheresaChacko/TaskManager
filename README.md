# TaskManager


A lightweight and user-friendly task management application built using **React**, **Spring Boot**, and **PostgreSQL**. The app allows users to manage tasks with features like category filtering, view deadline , and CRUD operations.

---

## Features

- Add, update, delete tasks
- Filter tasks by **category** (e.g., Work, Personal)
- Auto-colored task cards using `randomcolor`
- Category-based task filtering with backend support
- Responsive and clean UI (Bootstrap)

---

##  Tech Stack

###  Frontend – React

- React 18+
- Bootstrap 5
- Axios for API calls
- RandomColor for dynamic UI backgrounds

###  Backend – Spring Boot



###  Database

- PostgreSQL  
  

---

##  ER Diagram
 Task

- id (PK) 
- title
-  description 
- status 
- category 
- deadline 


---

## REST API Endpoints

Base URL: `http://localhost:8080/api/tasks`

| Method | Endpoint                         | Description                     |
|--------|----------------------------------|---------------------------------|
| GET    | `/api/tasks`                     | Get all tasks                   |
| GET    | `/api/tasks/{id}`                | Get task by ID                  |
| POST   | `/api/tasks`                     | Create a new task               |
| PUT    | `/api/tasks/{id}`                | Update a task                   |
| DELETE | `/api/tasks/{id}`                | Delete a task                   |
| GET    | `/api/tasks/c/{category}` | Get tasks by category           |

### Sample Task Payload (POST/PUT)
```json
{
  "title": "Finish project",
  "description": "Complete the frontend UI",
  "status": "Pending",
  "category": "Work",
  "deadline": "2025-07-20"
}

