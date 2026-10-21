# ShowCase: Product Gallery with Image Upload

MERN stack lab project (NU MOA, BS Information Technology).

## Structure
- `client/`  React + Vite + Tailwind CSS (deploy to Vercel, root directory `client`)
- `server/`  Express + Mongoose API (deploy to Render, root directory `server`)
- `extras/App.activity1.jsx`  Activity 1 version of App.jsx (in-memory, no API)

## Activity 1 (Frontend only)
1. `cd client && npm install`
2. Copy `extras/App.activity1.jsx` over `client/src/App.jsx`
3. `npm run dev` and open http://localhost:5173
   (Restore the final App.jsx afterward for Activity 3.)

## Activity 2 (Backend)
1. Create the MongoDB Atlas cluster, user, and Network Access `0.0.0.0/0` (Steps 17-21).
2. `cd server && npm install`
3. Copy `.env.example` to `.env` and put your real connection string in `MONGO_URI`.
4. `npm start` and open http://localhost:5000/api/products (should show `[]`).

## Activity 3 (Hosting)
1. Push to GitHub (`.gitignore` already excludes `.env`, `node_modules`, `dist`).
2. Render: Root Directory `server`, Build `npm install`, Start `npm start`, env var `MONGO_URI`.
3. Put your Render URL in `client/.env` as `VITE_API_URL` (no trailing slash).
4. Vercel: Root Directory `client`, Framework Vite, env var `VITE_API_URL`.

## Before you submit
- Replace `[Section]` in `client/src/App.jsx` (footer) and `extras/App.activity1.jsx`.
- Name is already set to Marc David Gonzales in the hero (`GalleryPage.jsx`) and footer.
