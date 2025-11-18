# The Wild Oasis — Website

Modern web app built with Next.js (App Router) and Tailwind CSS. It integrates Supabase for backend/services and uses NextAuth for authentication. UI leverages Heroicons, date-fns, and react-day-picker.

## Overview

- **Framework**: Next.js 14 (App Router in `app/`)
- **Styling**: Tailwind CSS
- **Auth**: NextAuth v5 (beta)
- **Backend/DB/Storage**: Supabase
- **Date utilities**: date-fns
- **Date picker**: react-day-picker

## Tech Stack

- next@14.2.x, react@18, react-dom@18
- tailwindcss@^3, postcss
- @supabase/supabase-js
- next-auth@^5.0.0-beta
- date-fns, @heroicons/react, react-day-picker

## Requirements

- Node.js 18+ (recommended LTS)
- npm, yarn, pnpm, or bun
- Supabase project and credentials

## Setup

1. Install dependencies:
   ```bash
   npm install
   # or: yarn | pnpm i | bun i
   ```
2. Create `.env.local` at the project root and add the environment variables below.
3. Start the dev server:
   ```bash
   npm run dev
   ```
4. Open http://localhost:3000

## Environment Variables

Create a `.env.local` file with the following (placeholders shown; adjust to your setup):

```
# Supabase
NEXT_PUBLIC_SUPABASE_URL=<your_supabase_url>
NEXT_PUBLIC_SUPABASE_ANON_KEY=<your_supabase_anon_key>

# NextAuth
NEXTAUTH_URL=http://localhost:3000
NEXTAUTH_SECRET=<generate_a_strong_secret>

# (Optional) Provider credentials / additional secrets if used
# GOOGLE_CLIENT_ID=...
# GOOGLE_CLIENT_SECRET=...
```

If you deploy (e.g., on Vercel), set the same variables in the deployment environment. Do not commit secrets.

## Available Scripts

From `package.json`:

- `npm run dev` — Start Next.js dev server
- `npm run build` — Create production build
- `npm run start` — Start production server
- `npm run prod` — Build then start in production mode
- `npm run lint` — Run Next.js ESLint

## Running Locally

```bash
npm run dev
```

Then visit http://localhost:3000. Changes in `app/` hot-reload automatically.

## Building for Production

```bash
npm run build
npm run start
```

## Linting

```bash
npm run lint
```

## Deployment

- **Hosting**: Vercel is recommended for Next.js
- **Env**: Add `.env` values (Supabase + NextAuth) to your hosting provider
- **Supabase**: Ensure Database/Auth/Storage policies and redirects (if using OAuth) are configured

Notes:

- NextAuth v5 is in beta; verify adapter/provider setup and callbacks as needed
- If you use image optimization, configure allowed domains in `next.config.js`
