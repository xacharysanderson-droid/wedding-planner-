# Aisle

A wedding planning app for UK couples — budget, guests, tables, schedule, music, and mood board. Single-page, no backend, lives in your browser.

## Try it locally

Just open `index.html` in any modern browser. That's it. Your data is saved to `localStorage` so it persists between visits on the same device.

## Deploy free on GitHub Pages

1. Create a new GitHub repository (public is fine).
2. Upload `index.html` (and this `README.md`) to the root of the repo.
3. In the repo go to **Settings → Pages**.
4. Under "Build and deployment" → "Source", choose **Deploy from a branch**.
5. Pick the `main` branch and the `/ (root)` folder, then click **Save**.
6. After a minute or two GitHub will show you a URL like `https://<your-username>.github.io/<repo-name>/`. That's your live app.

## What's in the app

- **Home** — countdown to the day, headline numbers (budget, RSVPs, next payment, open tasks), recent activity.
- **Plan** — task list with priorities, due dates, and assignees.
- **Guests** — full guest list with households, RSVP status, dietary and accessibility tags, table assignments.
- **Tables** — add tables, drop unseated day guests onto them, over-capacity warnings.
- **Money** — GBP budget with categories, line items, payments, caps, and progress bars.
- **Day** — visual wedding-day timeline with critical-moment and buffer markers.
- **Music** — moments (processional, first dance, last song…) with must-play / do-not-play lists.
- **Mood** — image board with categories, love/maybe/no, palette swatches; upload from your phone or paste a URL.
- **Vendors** — supplier list with status, quote, deposit, balance, rating, notes.
- **Settings** — wedding details, JSON export/import backup, reset to demo data.

## Tech notes

- React 18 + Babel standalone via CDN. No build step.
- All state is in React, persisted to `localStorage` (`aisle.*` keys).
- Designed mobile-first; sidebar collapses to a horizontal tab strip under 880px.
- WCAG-leaning palette and large touch targets; will benefit from a proper a11y audit before launch.

## What to add next (after MVP)

- Real partner/collaborator accounts with roles (will require a backend — Supabase or Firebase is a good next step).
- PDF exports for the seating chart, schedule, and rooming list.
- iOS / Android share-sheet extension for direct screenshot capture to the mood board.
- Realtime multiplayer table planner.

## Licence

MIT — use this however you'd like.
