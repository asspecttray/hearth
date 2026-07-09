# Hearth — Family Finance Ledger

A household net worth, budget, and goals tracker. React + Vite + Tailwind, backed by Supabase.

## Deploy this to the web (Vercel, free)

1. Create a new GitHub repository and upload every file in this folder (keep the folder structure —
   `src/App.jsx`, `src/main.jsx`, etc. — as-is).
2. Go to vercel.com, sign in with GitHub, click "Add New Project," and select this repository.
3. Leave all settings as their Vite defaults and click Deploy.
4. Vercel will give you a live URL (something like `hearth-yourname.vercel.app`) — that's your
   permanent app address, usable on your phone or computer, online or offline once loaded once.

## Run it locally first (optional, requires Node.js installed)

```
npm install
npm run dev
```

Then open the local address it prints (usually http://localhost:5173).

## Install on iPhone

Open your deployed Vercel URL in Safari → tap the Share icon → "Add to Home Screen." It'll behave
like a native app icon from then on.

## Notes

- Supabase URL and anon key are already wired into `src/App.jsx`. The anon key is safe to expose
  publicly — it only works within the Row Level Security policies already set up on your database.
- Sign-in uses a 6-digit email code rather than a magic link (see the comment at the top of `App.jsx`
  for why).
- Bank auto-sync (SimpleFIN) is a planned Phase 3 addition, not yet built.
