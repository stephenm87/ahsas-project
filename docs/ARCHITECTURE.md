# Architecture

The AHSAS project is a multi-page web application built with Vite and vanilla JavaScript.

## Frontend
- **Framework:** Vite 6 + Vanilla JS
- **Pages:** 11 HTML pages (index, about, cer, cer-builder, compare, pieces, research, seminar, source-analyzer, sources, timeline)
- **Styling:** Vanilla CSS (`src/styles/`)
- **Structure:** Modular JavaScript in `src/js/` handling specific functionalities (auth, sync, research, supabase, timeline, progress, seminar, nav, source-analyzer)

## Backend / Serverless
- **Netlify Functions:** Located in `netlify/functions/`
  - `image-proxy.js`: Wikimedia proxy
  - `keep-alive.mjs`: Cron Supabase ping
  - `synthesize.js`: Gemini seminar synthesis

## Database (Supabase)
- **Auth:** Magic Link auth restricted to `@saschina.org`
- **Database:** PostgreSQL with Row Level Security (RLS)
- **Tables:** `user_data`, `essays`, `bookmarks`, `cer_submissions`
