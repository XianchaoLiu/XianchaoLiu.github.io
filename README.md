# Personal academic website

Static site, no build step. Open `index.html` in a browser to view it locally.

## Files

| File | Page |
| --- | --- |
| `index.html` | Home: portrait, bio, one-line research statement, news, profile links |
| `research.html` | Three research thrusts + applications + methods |
| `publications.html` | Accepted journal and conference papers |
| `contact.html` | Email, office, mailing address, profiles |
| `style.css` | Shared stylesheet (colors, fonts, layout, phone breakpoint) |
| `assets/` | Images and PDFs: `portrait.jpg`, `gate-drive.jpg`, `module.jpg`, `embedded-die.jpg`, papers |

## Local debugging

- Double-click `index.html`; the four pages link to each other with relative paths, so they work from disk.
- For a local server (avoids browser file:// quirks), run in this folder:
  `python -m http.server 8000` and open http://localhost:8000
- Phone layout: shrink the browser window below 760 px wide, or use the browser's device toolbar (F12).
- Dark mode follows the operating system setting.

## Placeholders to replace

Search for `[` in the HTML files. Every `[Your Name]`, `[Example]`, `[paper title]`, `[Caption: …]`, `[Room]` is a placeholder.
To add a picture, replace the `<span>…</span>` inside the dashed box with an `<img>` tag — a commented-out example sits next to each box.

## Deploy to GitHub Pages

1. Create a public repository named `<username>.github.io`.
2. Copy these files into the repository root and push.
3. Settings → Pages → Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
4. The site appears at `https://<username>.github.io` within a few minutes.
