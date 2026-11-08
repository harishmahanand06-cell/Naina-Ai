# NAINA AI — Groq starter project

This is a starter web app for personal testing. It uses Groq's OpenAI-compatible API from the server. The API key must stay on the server and must never be placed in `public/index.html` or committed to GitHub.

## Files
- `public/index.html` — NAINA chat interface and browser speech features
- `server/index.js` — Express API proxy to Groq
- `.env.example` — environment variable names only; do not put real secrets here

## Run locally
1. Install Node.js 20 or later.
2. Run `npm install`.
3. Copy `.env.example` to `.env`.
4. Put your Groq key in `.env` as `GROQ_API_KEY=...`.
5. Run `npm start` and open `http://localhost:3000`.

## Deploy
Set these environment variables in your hosting provider's dashboard:
- `GROQ_API_KEY` = your Groq secret key
- `GROQ_MODEL` = `llama-3.3-70b-versatile` (or another model currently available to your Groq account)
- `NODE_ENV` = `production`

Start command: `npm start`

Do not upload `.env` or share your API key. Free hosting and free API plans have usage limits and may sleep or change terms. Browser speech recognition and Sambalpuri voice availability depend on the Android browser/device and are not guaranteed.

This starter does not yet include a native Android APK, database, persistent memory, reminders, or a real PIN-lock implementation. It is not deployed until you complete hosting setup.
