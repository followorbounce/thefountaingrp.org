# thefountaingrp.org

The Fountain Group — a psychiatric care practice (Dr. Prashanth Pillai,
Dr. Ksenia Pillai). Jekyll static site on GitHub Pages, custom domain.
Cloned into this environment for the first time on 2026-09-19 (it
previously existed only on GitHub).

## Structure
- `_layouts/default.html` — base layout, all other layouts extend it via `layout: default` front matter.
- `_layouts/doctor.html`, `_layouts/page.html` — extend `default`; used by doctor-bio pages and general content pages respectively.
- `_includes/nav.html`, `_includes/footer.html`, `_includes/doctor-card.html` — shared partials.
- `pages/*.html` — content pages (about, booking, contact, services), each with Jekyll front matter.
- `pages/doctors/*.html` — individual doctor bio pages.
- `index.html` — homepage, `layout: default`.
- `brand-identity.html` — standalone self-contained page (own `<head>`, not templated).

## Conventions
- Never use Russian in code/UI/docs unless the task explicitly calls for it.
- This is a live client site — be conservative with changes beyond what's explicitly asked.

## Analytics
Cloudflare Web Analytics beacon added 2026-09-19 — own site (host `thefountaingrp.org`, see `[[cloudflare-analytics-setup]]` in the assistant's memory). Injected into `_layouts/default.html` (covers `doctor.html`/`page.html` too, since both extend it) plus the standalone `brand-identity.html`.

## Deploy
GitHub Pages from `main`, custom domain `thefountaingrp.org` (CNAME file present). Remote: `github.com/followorbounce/thefountaingrp.org`.
