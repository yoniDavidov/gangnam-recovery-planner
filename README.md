# Gangnam Recovery Planner

A one-page planner for people flying to Seoul for beauty treatments. Enter your landing date, your flight home and what you're booking, and it shows each trip day as treatment, rest, low-key, out and about, or photo-ready. It also warns when:

- your flight is earlier than clinics usually allow after that procedure
- a follow-up (stitch or splint removal) falls after you leave
- you won't look photo-ready before your last day
- two surgeries are booked inside each other's rest period

Each treatment also gets a "book by" date so you can plan backwards from your flight.

## Run it

It's a single static `index.html` with no build step and no dependencies. Open it in a browser.

## Deploy

**GitHub Pages:** push this folder to a repo, then Settings → Pages → Deploy from branch → `main` / root.

**Vercel:** `npx vercel` in this folder, or import the repo at vercel.com. No config is needed.

## Recovery data

All timings live in the `TREATMENTS` object at the top of the script, one line per procedure, so a clinic or editor can correct them without touching the logic. They are typical planning ranges, not medical advice, and the page says the clinic's own aftercare plan always wins.
