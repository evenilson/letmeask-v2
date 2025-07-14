# Let Me Ask v2

Let Me Ask v2 is a modern web application for creating and managing question rooms, featuring AI-powered answers and audio transcription. The project is split into two main parts: a React-based frontend and a Node.js backend API. This repository contains both components, designed for easy local development and deployment.

## Features

- Create and manage question rooms
- Submit questions and receive AI-generated answers
- Audio recording and transcription for questions
- Modern, modular architecture for scalability

## Tech Stack

- **Frontend:** React, TypeScript, Vite, TailwindCSS, React Query, Radix UI
- **Backend:** Node.js, Fastify, TypeScript, PostgreSQL (with pgvector), Drizzle ORM, Zod
- **AI/ML:** Google Gemini API for transcription and answer generation
- **DevOps:** Docker, Docker Compose

## Project Structure

```
letmeask-v2/
├── web/      # Frontend (React)
├── server/   # Backend (Node.js API)
└── README.md # Project overview
```

## Getting Started

### Prerequisites
- Node.js (v18+)
- npm or yarn
- Docker & Docker Compose (for database)

### 1. Clone the repository
```bash
git clone <repo-url>
cd letmeask-v2
```

### 2. Setup the Backend (API)
See [server/README.md](server/README.md) for detailed instructions.

- Configure and start the PostgreSQL database with Docker
- Set up environment variables
- Install dependencies and run migrations
- Start the backend server (default: http://localhost:3333)

### 3. Setup the Frontend (Web)
See [web/README.md](web/README.md) for detailed instructions.

- Install dependencies
- Start the development server (default: http://localhost:5173)

## Development Workflow
- Start the backend first to provide the API for the frontend
- Then start the frontend and access the app in your browser

## License

This project is provided for educational and demonstration purposes.
