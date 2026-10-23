# NickDosc.dev — pixel-art developer portfolio

First public release of Nikolaos Doschoris’s RPG-style portfolio, adapted from his October 2026 CV.

## Local preview

From the directory containing `index.html`, run:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## GitHub Pages deployment

Use `bash launch_mac.sh` for the guarded initial GitHub upload, or upload the public website files manually to a public repository named `nickdosc.github.io` under the `nickdosc` account.

GitHub repository → Settings → Pages → Deploy from a branch → `main` → `/(root)` → Save.

GitHub repository → Settings → Pages → Custom domain → `nickdosc.dev` → Save, **before** updating DNS at Porkbun.

Porkbun DNS (root host blank): A 185.199.108.153; A 185.199.109.153; A 185.199.110.153; A 185.199.111.153. Add `www` CNAME to `nickdosc.github.io`. Remove conflicting default parking records (do not delete mail MX/TXT records). Enable **Enforce HTTPS** after certificate activation.

## Content caveats

- Game illustrations are CSS and handmade placeholder pixel sprites, **not** screenshots of the real games.
- App Store/Play Store and trailer URLs are intentionally omitted until verified.
- Public PDF omits phone number; original private DOCX is **not** in this repository.
- This first release uses plain HTML/CSS/JS for safe zero-build deployment; an Astro refactor can follow once the design settles.
