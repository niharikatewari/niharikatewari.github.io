# Academic Homepage Template — Sidebar Layout

Same content sections as a classic academic homepage (about, news,
publications, service, honors, teaching) but a genuinely different layout:
a sticky left sidebar (photo, name, jump-nav, contact links) next to a single
scrolling content column on the right. No table-style publication blocks, no
thumbnails — publications are typographic entries with a left accent rule.
Plain HTML/CSS, no build step, no JavaScript.

## What's included

```
index.html          ← everything (content + styling) lives in this one file
images/headshot.jpg  ← your photo
files/               ← put your CV.pdf here
```

Publications in this layout don't use thumbnail images — it's a cleaner,
text-only list. If you'd rather have thumbnails, you can add an `<img>` back
into each `.pub-entry` block; ask and I can do that version too.

## How to use it

1. **Create your GitHub Pages repo** named `yourusername.github.io`.
2. **Upload** `index.html`, `images/headshot.jpg`, and the `files/` folder.
3. **Replace placeholder content** directly in `index.html`:
   - Sidebar: name, role/department, contact links
   - About paragraph(s)
   - News items — copy/paste a `.news-item` div to add more
   - Publications — copy/paste a `.pub-entry` div to add more
   - Service / Honors / Teaching — copy/paste a `.line-row` div to add more
4. **Add your CV** as `files/CV.pdf`.
5. **Enable GitHub Pages**: repo **Settings → Pages → Source**, branch `main`,
   folder `/ (root)`, save.

## Notes

- The sidebar nav numbers (01–06) link to each section via `id` anchors —
  if you rename a section's `<h2>`, leave the `id="..."` on the parent
  `<section>` tag alone, or update both together.
- Accent color (currently a muted brick red, `#9a3324`) and all other colors
  live in the `:root { --variable }` block at the top of `<style>`.
- On narrow/mobile screens the sidebar collapses to a horizontal bar above
  the content automatically — no separate mobile markup needed.
