# Syed Mafooq Ul Hassan — Portfolio Website

This is a static academic portfolio designed for GitHub Pages and the custom domain:

`https://syedmafooqulhassan.com`

## Files

- `index.html` — all website content
- `styles.css` — responsive design and dark mode
- `script.js` — mobile navigation, theme toggle, active section, animations, and email copying
- `CNAME` — preserves the custom domain on GitHub Pages
- `.nojekyll` — tells GitHub Pages to serve files directly
- `assets/` — favicon, social preview, profile placeholder, CV PDF, and CV LaTeX source

## Replace the placeholder image

Upload your real portrait as `assets/profile.jpg`, then change this line in `index.html`:

```html
<img src="assets/profile-placeholder.svg" alt="Monogram placeholder for Syed Mafooq Ul Hassan">
```

to:

```html
<img src="assets/profile.jpg" alt="Syed Mafooq Ul Hassan">
```

A square or portrait image works best.

## Updating content

Edit `index.html`, commit the change to the `main` branch, and GitHub Pages will deploy it automatically.
