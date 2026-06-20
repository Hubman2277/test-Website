# Dunbar Scaffold Hire — Website

Statische Website (HTML/CSS/JS, **kein** Build-Schritt). Die eigentliche Seite liegt im Ordner [`projekt-dumber2.0/`](projekt-dumber2.0/).

## Seiten
- `index.html` — Startseite
- `about.html`, `news.html`, `join-our-team.html`, `privacy.html`
- `assets/` — `style.css`, `main.js`, lokale Fonts (`assets/fonts/`)

## Auf Vercel deployen
1. Repo auf GitHub pushen (siehe unten).
2. Auf [vercel.com](https://vercel.com) → **Add New → Project** → dieses GitHub-Repo importieren.
3. **Wichtig:** Bei **Root Directory** den Ordner `projekt-dumber2.0` auswählen.
4. **Framework Preset: Other** — kein Build Command, kein Output Directory nötig.
5. **Deploy** klicken. Fertig.

`projekt-dumber2.0/vercel.json` setzt sichere HTTP-Header und Langzeit-Caching für die Fonts.

## Nach GitHub pushen
Remote `origin` ist bereits gesetzt (→ `test-Website`):

    git push -u origin main

## Nicht im Repo / nicht deployed
Per `.gitignore` ausgeschlossen (bleiben nur lokal): `.claude/`,
`projekt-dumber2.0/.agents/`, `skills-lock.json`, `index-standalone.html`,
`_review_*.html`, `DEPLOY-NOTES.md`.

## Vor dem echten Go-Live
Siehe lokale `projekt-dumber2.0/DEPLOY-NOTES.md` — offene Punkte: Bilder
self-hosten (Rechte), ABN, Datenschutz-Platzhalter, Kunden-Freigaben.
