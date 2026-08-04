# Supabase Configuration

## Authentication
- **Provider:** Magic Link (Email).
- **Restriction:** Allowed only for `@saschina.org` domains.

## Database Schema & RLS
- **Tables:** `user_data`, `essays`, `bookmarks`, `cer_submissions`
- **Security:** Row Level Security (RLS) is enabled.
- **Migration Files:**
  - `supabase/migrations/001_enable_rls_user_data.sql`
  - `supabase-auth-setup.sql` (Configures essays, bookmarks, cer_submissions with RLS)

## Setup Requirements
Supabase client relies on `VITE_SUPABASE_URL` and `VITE_SUPABASE_ANON_KEY` for initialization (`src/js/supabase.js`).
