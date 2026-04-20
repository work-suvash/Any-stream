# work-stream

## Overview
A static HTML/CSS/JS website that serves as a curated directory of streaming-related links (movies, TV, anime, manga, live TV, sports, and apps). Built with pure HTML5, CSS3, and vanilla JavaScript. Data is stored in `links.json`.

## Architecture
- **Type:** Static site (no build step required)
- **Server:** `http-server` (Node.js) serving files on port 5000
- **Data:** `links.json` — flat-file database of streaming site links
- **PWA:** Includes `manifest.json` for progressive web app support
- **Brand Icon:** Uses a lightweight inline SVG broadcast icon in navigation and `icon.svg` for favicon/PWA references instead of the old PNG logo.

## Project Structure
- `index.html` — Main page, dynamically loads links from `links.json`
- `about.html`, `dmca.html`, `404.html`, `site-request.html` — Additional pages
- `style.css` — Main stylesheet
- `css/` — Supplemental CSS (critical, flash effects)
- `js/` — JavaScript (main.js, mouse-effects.js, anti-cheat)
- `logo/` — Site logos categorized by type (anime, apps, livetv, manga, movies_shows, paid_apps)
- `assets/` — UI assets (browser icons, social logos, backgrounds)
- `fonts/` — Local font files (Clash Display)
- `links.json` — All streaming site data

## Running
- Workflow: "Start application" — runs `npx http-server . -p 5000 -a 0.0.0.0 --cors`
- Port: 5000
