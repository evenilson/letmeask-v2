# Let Me Ask v2 – Backend

This is the backend API for Let Me Ask v2, a modern web application for creating and managing question rooms with AI-powered answers and audio transcription. Built with Node.js, Fastify, and PostgreSQL, it provides a robust, scalable, and type-safe API for the frontend.

## 🚀 Tech Stack

- **Node.js** with native TypeScript (experimental strip types)
- **Fastify** – High-performance web framework
- **PostgreSQL** with **pgvector** extension for vector search
- **Drizzle ORM** – Type-safe database operations
- **Zod** – Schema validation
- **Docker** – Database containerization
- **Biome** – Code linting and formatting

## 🏗️ Architecture

- Modular separation of routes, schemas, and database connection
- Schema validation with Zod for type safety
- Type-safe ORM with Drizzle
- Centralized environment variable validation

## ⚙️ Setup & Configuration

### Prerequisites
- Node.js (with support for `--experimental-strip-types`)
- Docker & Docker Compose

### 1. Clone the repository
```bash
git clone <repo-url>
cd letmeask-v2/server
```

### 2. Configure the database
```bash
docker-compose up -d
```

### 3. Configure environment variables
Create a `.env` file in the project root:
```env
PORT=3333
DATABASE_URL=postgresql://docker:docker@localhost:5432/letmeask-v2
GEMINI_API_KEY=your_google_gemini_api_key
```

### 4. Install dependencies
```bash
npm install
```

### 5. Run database migrations
```bash
npx drizzle-kit migrate
```

### 6. (Optional) Seed the database
```bash
npm run db:seed
```

### 7. Start the server
- Development:
  ```bash
  npm run dev
  ```
- Production:
  ```bash
  npm start
  ```

The API will be available at [http://localhost:3333](http://localhost:3333).

## 📚 Available Scripts
- `npm run dev` – Start the server in development mode with hot reload
- `npm start` – Start the server in production mode
- `npm run db:seed` – Seed the database with example data

## 🌐 API Endpoints
- `GET /health` – Health check
- `GET /rooms` – List available rooms
- `POST /rooms` – Create a new room
- `GET /rooms/:roomId/questions` – List questions for a room
- `POST /rooms/:roomId/questions` – Submit a question and get an AI answer
- `POST /rooms/:roomId/audio` – Upload and transcribe audio for a room

## 🗄️ Database
- PostgreSQL with `pgvector` for vector-based search
- Tables: `rooms`, `questions`, `audio_chunks`
- Migrations managed with Drizzle ORM

## License

This project is provided for educational and demonstration purposes. 