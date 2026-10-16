TIDY - installable cleaning checklist (PWA)

Files
  index.html              the app
  manifest.webmanifest    install info (name, colors, icons)
  sw.js                   service worker (offline support)
  icons/                  app icons

Run / host
  A PWA must be served over HTTPS (or localhost), not opened as a file.
  - Quick test:  cd into this folder, run  python3 -m http.server 8000
                 then open http://localhost:8000
  - Free hosting: drag the folder onto Netlify Drop, or push to GitHub Pages / Cloudflare Pages.

Install
  iPhone: open in Safari > Share > Add to Home Screen
  Android/Chrome/Edge: menu > Install app

Updating
  After editing any file, change CACHE = "tidy-v3" in sw.js to "tidy-v2" so devices pick up the update.
