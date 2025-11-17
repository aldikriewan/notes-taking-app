# Notes App

A simple but powerful notes application built with a modern JavaScript stack, featuring a separate backend API and a reactive frontend client. Perfect for learning and demonstrating full-stack development principles.

## Features

*   **Create, Read, Update, and Delete (CRUD)** notes seamlessly.
*   A clean and intuitive user interface for managing your notes.
*   Fast and responsive, built with Next.js for a great user experience.
*   RESTful API for all note operations.

## Project Structure

This project is a monorepo containing two main parts:

*   `notes-app-back-end/`: The heart of the application, a Node.js API server that handles all the logic and data.
*   `notes-app-frontend-1/`: The face of the application, a Next.js web client that users interact with.

---

## Tech Stack

### Backend (`notes-app-back-end`)

*   **Runtime**: Node.js
*   **Framework**: Hapi
*   **Utilities**: `nanoid` for unique IDs, `nodemon` for development workflow.
*   **Linter**: ESLint

### Frontend (`notes-app-frontend-1`)

*   **Framework**: Next.js (React)
*   **Styling**: Sass (SCSS Modules)
*   **Deployment**: Dockerfile included for containerization.

---

## Getting Started

To get this project up and running on your local machine, follow these steps.

### 1. Run the Backend Server

First, get the API server running:

```bash
# Navigate to the backend directory
cd notes-app-back-end

# Install dependencies
npm install

# Start the server (runs on http://localhost:5000 by default)
npm run start
```

### 2. Run the Frontend Client

In a new terminal, get the user interface running:

```bash
# Navigate to the frontend directory
cd notes-app-frontend-1

# Install dependencies
npm install

# Start the development server (runs on http://localhost:5000)
npm run dev
```

Once both are running, open your browser and visit `http://localhost:5000` to use the app!

---

## Backend API Endpoints

The backend provides the following endpoints to manage notes:

| Method | Path          | Description                |
| :----- | :------------ | :------------------------- |
| `POST` | `/notes`      | Create a new note.         |
| `GET`  | `/notes`      | Get all notes.             |
| `GET`  | `/notes/{id}` | Get a specific note by ID. |
| `PUT`  | `/notes/{id}` | Update a specific note.    |
| `DELETE`| `/notes/{id}` | Delete a specific note.    |

---

Happy coding!