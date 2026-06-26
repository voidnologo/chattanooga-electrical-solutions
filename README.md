# Chattanooga Electrical Solutions — landing page

Static, single-file marketing site for Felipe Rojas, Master Electrician.
No build step, no dependencies. Served as a static site (GitHub Pages).

## Files
- `index.html` — the entire page (HTML + inline CSS).
- `assets/logo.jpg` — brand mascot/logo (also used as social preview + apple-touch-icon).
- `.nojekyll` — tells GitHub Pages to serve files as-is.
- `IMG_20260619_1323363.jpg` — original logo upload (kept as source; safe to delete).

## Preview locally
Open `index.html` in a browser, or serve the folder:
```
python3 -m http.server 8000   # then visit http://localhost:8000
```

## Before going live — replace the PLACEHOLDERS
Everything that needs Felipe's real details is marked with a `PLACEHOLDER`
comment in `index.html`. Search the file for `PLACEHOLDER` and update:

| Placeholder            | Where it appears                                  |
|------------------------|---------------------------------------------------|
| Phone `(423) 555-0142` | header, hero, contact section, footer (and `tel:` links) |
| Email                  | contact section + footer (`mailto:` links)        |
| License number `#E-00000000` | footer                                      |
| Domain                 | `<title>`/canonical/Open Graph + JSON-LD          |
| Reviews & stats        | testimonials + the "15+/500+" credential numbers  |

### Wire up the quote form (Formspree)
The form is ready for [Formspree](https://formspree.io) (free tier, works on
static hosting). Create a form, then replace `YOUR_FORM_ID` in the
`<form action="...">` tag. Submissions will be emailed to Felipe — no backend.

## Notes
- Colors and type are derived from the logo (black field, electric red, amber).
- Fully responsive; respects reduced-motion and keyboard focus.
- All content is prototype copy meant to show layout and possibilities.
