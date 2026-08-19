# ugurmertyasar.github.io

Static site. No build step: these files *are* the site.

## Repository layout
```
index.html
research.html
style.css
README.md
assets/
    portrait.jpg
    cv.pdf          <- render from the Quarto source, then drop here
```

## Common edits
- **Colours** -> `:root` at the top of `style.css`. Background is `--paper`.
- **Add a paper** -> copy an `<article class="paper">` block in `research.html`
- **New CV** -> overwrite `assets/cv.pdf`

## The map
`index.html` contains the coverage map inline as SVG (~127 KB, ~46 KB over the
wire). It has to be inline rather than an `<img>`, because an SVG loaded as an
image is sealed off from the page and cannot be styled or made interactive.
The block is fenced with `<!-- MAP -->` comments; scroll past it when editing.

Each country carries `data-n` (name) and `data-l` (survey language), and a
`<title>` element so the names still work for screen readers and with
JavaScript disabled.

To regenerate it you need the world-atlas topology and the language table; ask
Claude rather than hand-editing the path data.

## Do not commit
Anything you would not hand to a stranger. The repository is public and git
keeps deleted files in history. The unpublished enforcement figure lives in
`_held/` on the local machine and must stay there.
