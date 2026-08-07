# ugurmertyasar.github.io

Static personal site. No build step: these files *are* the site.

## Files
| Path | What it is |
|---|---|
| `index.html` | Home page |
| `research.html` | Ongoing projects |
| `style.css` | All styling. Palette variables at the top. |
| `assets/coverage-map.svg` | 92-society coverage map |
| `assets/portrait.jpg` | Headshot |
| `assets/cv.pdf` | **Not yet added** — see below |
| `_held/` | Written but deliberately not published |

## Common edits
- **Colours / fonts** → top of `style.css`, in `:root`
- **Number of societies** → search `92` in `index.html`
- **Add a paper** → copy an `<article class="paper">` block in `research.html`
- **New CV** → overwrite `assets/cv.pdf`, no other change needed

## `_held/enforcement-figure.html`
An interactive figure showing the two dimensions of norm enforcement. Held back
because it makes the argument of an unpublished paper very legible. To publish:
paste the `<figure>` block into `research.html` and the `<script>` block just
before `</body>`.

## To add the CV
Open the CV in Google Docs → File → Download → PDF Document.
Rename to `cv.pdf`, put it in `assets/`.
