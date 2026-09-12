# Richie's Tavern Operating System (RT-OS)

## Project identity
- **Name:** RT-OS — Richie's Tavern Operating System
- **Restaurant:** Richie's Tavern, 835 12th Street, Paso Robles, CA 93446
- **Opening:** September 16, 2026 (17 seats, walk-in only, dark/green/brass aesthetic)
- **Repo:** github.com/Julianonciela/richiestavern-os
- **Live:** https://richiestavern-os.vercel.app
- **Owner/Admin:** Juliano Incorvaia (Julianonciela)
- **Direction:** Richie, Uli

## Tech stack
- Static HTML/CSS/JS — no build step, no framework
- Deployed on Vercel (auto-deploy from GitHub main branch)
- Auth: localStorage-based role system (superadmin/direction/staff)
- Knowledge base: Markdown files in `academy/` folder

## File map
```
/workspace/rt-os/
├── index.html          # Login (3 roles: superadmin/direction/staff)
├── hub.html            # Management dashboard (checklist, timeline, decisions)
├── academy.html        # Staff training (lessons loaded from academy/*.md)
├── admin.html          # Superadmin panel (access management, system status)
├── floor-plan-en.html  # Interactive floor plan presentation (EN)
├── floor-plan.html     # Interactive floor plan presentation (FR)
├── vercel.json         # Vercel static deploy config
└── academy/
    ├── lesson-1.md     # The First Impression
    └── lesson-2.md     # Reading the Room
```

## Access codes
- Superadmin (Juliano): `juliano2026`
- Direction (Richie/Uli): `richie2026`
- Staff: `teamrt2026`

## Key conventions
- All content in English (client-facing and staff-facing)
- Internal notes in French for Juliano
- Checklist state persisted in localStorage (per-browser)
- Lessons added as `.md` files in `academy/` — auto-loaded by academy.html
- No backend, no database, no API — everything is static files

## Active cron jobs (VPS)
- `6c9326eb49d4` — RT-OS Daily Brief (8am UTC, telegram)
- `69273c831807` — Paso Robles Competition Watch (every 6h, telegram)
- `6071c5457f6e` — RT-OS Checklist Reminder (9am UTC, telegram)

## Design tokens
- Background: #0d1510 (dark green-black)
- Primary: #c9a84c (brass/gold)
- Secondary: #8b3a3a (brick red)
- Text: #e8dcc8 (cream)
- Headings: Playfair Display (serif)
- Body: DM Sans (sans-serif)