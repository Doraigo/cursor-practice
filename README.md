# Full-Stack Project

This project has a **backend** (Express) and a **frontend** (React with Vite).

## Prerequisites

- Node.js (v18 or later recommended)
- npm

## Running the project

### Backend

From the project root:

```bash
cd backend
npm start
```

The API runs at **http://localhost:3000**.

For development, you can use the same command or add a dev script with a file watcher (e.g. `nodemon`).

### Frontend

In a separate terminal, from the project root:

```bash
cd frontend
npm run dev
```

The app runs at **http://localhost:5173** (Vite default). Open this URL in your browser.

### Running both

1. Terminal 1: `cd backend && npm start`
2. Terminal 2: `cd frontend && npm run dev`
3. Use the frontend at http://localhost:5173; it can call the backend at http://localhost:3000.

## Project structure

```
├── backend/          # Express server (port 3000)
│   ├── server.js
│   └── package.json
├── frontend/          # Vite + React (port 5173)
│   ├── src/
│   └── package.json
└── README.md
```

## Backend dependencies

- **express** – web server
- **cors** – cross-origin requests (for frontend)
- **dotenv** – environment variables (e.g. `.env` in `backend/`)
- **openai** – OpenAI API client

Put secrets (e.g. `OPENAI_API_KEY`) in `backend/.env` and ensure `.env` is in `.gitignore`.
