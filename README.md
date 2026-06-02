# Christen Gemeente Venlo

Een tijdelijke, statische under-construction website voor Christen Gemeente Venlo.

## Deploy

Deze site heeft geen build-stap nodig. Deploy de repository als statische website met `index.html` als entrypoint.

Geschikt voor onder andere:

- Render
- GitHub Pages
- Netlify
- Vercel
- Cloudflare Pages

## Deploy op Render

Deze repository bevat een `render.yaml` Blueprint. Daarmee kan Render de static site automatisch configureren.

1. Ga naar de Render Dashboard.
2. Kies **New** > **Blueprint**.
3. Koppel de GitHub repository `JPZ-12/ChristenGemeenteVenlo`.
4. Selecteer `main` als branch.
5. Render leest `render.yaml` en publiceert de site vanuit de repository-root.

Handmatig als **Static Site** kan ook:

- Build Command: `true`
- Publish Directory: `.`
- Branch: `main`

## Lokaal bekijken

Open `index.html` direct in de browser, of start een simpele lokale server:

```bash
python3 -m http.server 8000
```

Daarna staat de site op `http://127.0.0.1:8000/`.
