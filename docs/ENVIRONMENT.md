# Environment Variables

The application requires the following environment variables. Do NOT commit real values to version control.

## Client-Side (Vite)
- `VITE_SUPABASE_URL`: URL of the Supabase project.
- `VITE_SUPABASE_ANON_KEY`: Anon/public key for Supabase.

## Server-Side (Netlify Functions)
- `GEMINI_API_KEY`: API key for Gemini AI synthesis (used in `synthesize.js`).

## Example `.env` file
```env
VITE_SUPABASE_URL=your_supabase_url_placeholder
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key_placeholder
GEMINI_API_KEY=your_gemini_api_key_placeholder
```
