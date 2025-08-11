# planner-v9
Persönlicher Assistenten 
# Planner v9 — Netlify-ready PWA

This repo contains Planner v9, a PWA personal planner with:
- Calendar (Day/Week/Month/Year)
- Day time-grid (06:00–23:00) with automatic slot assignment
- Drag & drop (week + day slots)
- Long-term goals -> subgoals -> calendar integration
- Repeating events support
- XP / Level system, intro + mini-setup
- Offline-capable (service worker)

## How to deploy (GitHub → Netlify)

1. Create a **new repository** on GitHub (public or private).
2. Add these files to the repo (use GitHub web "Add file → Create new file" or Upload):
   - `index.html`
   - `style.css`
   - `app.js`
   - `manifest.json`
   - `service-worker.js`
   - `assets/icon-192.svg`
   - `assets/icon-512.svg`
   - `README.md`
3. In Netlify:
   - Go to **app.netlify.com** → New site → **Import from Git**
   - Connect GitHub, pick the repo
   - Build settings: _no build command_ (leave blank)
   - Publish directory: `/` (root)
   - Deploy site
4. Open the live URL. On first load you will see the intro (mini-setup).

## Troubleshooting
- If you see a white page:
  - Open the debug overlay (top-right) → press **Unreg SW** and **Clear Cache**, then reload.
  - Or open the site in a Private/Incognito window to bypass SW cache.
- If icon is missing, ensure `assets/` files uploaded correctly. SVG icons are acceptable.

## Notes & next steps
- The app stores data in `localStorage` (client-side). If you want multi-device sync later, we can add a backend sync (optional).
- Want push notifications, calendar export or iCloud sync? I can add them in v9.x.

---

## Ich helfe live
Wenn du magst, begleite ich dich jetzt Schritt-für-Schritt beim Erstellen des GitHub-Repo und beim Hochladen in Netlify.  
Sag „Start GitHub“ und ich leite dich durch **jeden** Klick (oder sag mir, wenn du die Dateien schon hochgeladen hast — dann sag mir den Repo-Link und ich prüfe sofort die Struktur).
