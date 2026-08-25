# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some Oxlint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the Oxlint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and Oxlint's TypeScript related rules in your project.

---

## Backend (added: Express + SQLite)

A minimal backend has been added at [backend](/C:/Users/Jhasa/OneDrive/Desktop/REACT+VITE/backend). It uses Express and a local SQLite database (better-sqlite3).

Quick start:

1. Open a terminal and start the backend:

   cd backend
   npm run dev

2. The backend runs on port 4000 by default. Endpoints:
   - GET  /api/items        -> list items
   - POST /api/items        -> create item (JSON body: { "name": "..." })
   - DELETE /api/items/:id  -> delete item

3. The SQLite file is created at backend/db/database.sqlite. The backend README has more details: [backend/README.md](C:/Users/Jhasa/OneDrive/Desktop/REACT+VITE/backend/README.md)

From the React app, call the API at http://localhost:4000/api/* (or configure a proxy in Vite if preferred).
