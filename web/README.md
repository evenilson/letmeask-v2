# Let Me Ask v2 – Frontend

This is the frontend for Let Me Ask v2, a modern web application for creating and managing question rooms with AI-powered answers and audio transcription. Built with React and TypeScript, it provides a fast, accessible, and responsive user experience.

## 🚀 Tech Stack

- **React 19.1** – User interface library
- **TypeScript 5.8** – Static type checking
- **Vite 7.0** – Build tool and dev server
- **TailwindCSS 4.1** – Utility-first CSS framework
- **React Router Dom 7.6** – Routing
- **TanStack React Query 5.8** – Server state management
- **Radix UI** – Accessible UI primitives
- **shadcn/ui** – Component system
- **Lucide React** – Icon library

## 📂 Project Structure

```
src/
├── components/ui/    # UI components
├── pages/            # Application pages
├── lib/              # Utilities and configuration
└── app.tsx           # Root component
```

## ⚙️ Setup & Installation

### Prerequisites
- Node.js (v18 or higher)
- npm or yarn

### Installation

1. Clone the repository and navigate to the `web` folder:
   ```bash
   git clone <repo-url>
   cd letmeask-v2/web
   ```
2. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```
3. Start the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```
4. Access the app at [http://localhost:5173](http://localhost:5173)

### Available Scripts
- `npm run dev` – Start the development server
- `npm run build` – Build for production
- `npm run preview` – Preview the production build

## 🔗 Backend API

This frontend consumes the Let Me Ask v2 API, which must be running on [http://localhost:3333](http://localhost:3333) by default. Make sure to start the backend before using the frontend. See the [server/README.md](../server/README.md) for backend setup.

## 🛠️ Design Patterns
- **Component-based Architecture** – Modular React components
- **File-based Routing** – Page routing with React Router
- **Server State Management** – Data fetching and caching with React Query
- **Variant-based Components** – Flexible UI with CVA
- **Composition Pattern** – Composable UI with Radix Slot
- **Path Aliasing** – `@/` points to `src/`

## License

This project is provided for educational and demonstration purposes. 