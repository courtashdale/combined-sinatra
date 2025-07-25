[![Frontend Deployment](https://img.shields.io/badge/Vercel-Online-brightgreen?logo=vercel)](https://sinatra-pi.vercel.app)
[![Backend Status](https://img.shields.io/badge/Render-Online-brightgreen?logo=render)](https://backend.sinatra.live)
# 🎸 Sinatra

Sinatra is a full-stack web application for sharing Spotify listening habits. The app lets users sign in with Spotify, analyze playlists and genres, and display a public profile accessible from a unique URL. It provides a FastAPI backend with MongoDB storage and a React frontend build with Vite. 


This repository contains both the FastAPI backend and the React frontend of Sinatra that previously existed in separate repositories.

## 🗺️ Architecture
- `backend/` - FastAPI server and services
  - `api/` - route modules
  - `services/` - Spotify, token, and other helpers
  - `db/` - MongoDB connection utilities
- `frontend/` - React application
  - `src/` - Pages and components
  - `public/` - Static assets

## 👷 Development

1. Install Python dependencies
```bash
cd backend
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

2. Install frontend dependencies
```bash
cd ../frontend
npm install --legacy-peer-deps
```

3. Start both servers (from /frontend)
```bash
npm run dev:all
```
This runs the Vite dev server and the FastAPI backend together.

## 🧼 Fortmatting

Run `npm run format` inside `frontend/` to format both projects. It formats the React code with Prettier and the backend with Black.
