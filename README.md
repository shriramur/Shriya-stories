# ஸ்ரேயா கதைகள் — Shriya's Story World

A little website of animated, illustrated storybooks in Tamil — every story dreamed up by 4-year-old Shriya. 🌈

## What's here

- `index.html` — the main page, listing all stories (plus a "coming soon" section for new ones).
- `stories/` — one self-contained HTML file per story. Each story is a scrolling, page-by-page storybook with hand-drawn-style SVG art, gentle animations, and a "🔊 read aloud" button (uses the browser's built-in Tamil text-to-speech).

## Viewing it locally

No build step needed — just open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

then visit `http://localhost:8000`.

## Hosting on GitHub Pages

1. Push this repo to GitHub (already done if you're reading this from there).
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Pick the `main` branch (or whichever branch has these files) and the `/ (root)` folder.
5. Save — GitHub will give you a URL like `https://<username>.github.io/<repo-name>/` within a minute or two.

## Adding a new story

1. Create a new HTML file in `stories/` (the existing ones are a good template — same fonts, page structure, and read-aloud script).
2. Add a `<a class="home-btn" href="../index.html">🏠</a>` link near the top of `<body>` so kids can get back to the main page.
3. Add a new `<article class="card">` to the story grid in `index.html`, linking to the new file — or move one of the "coming soon" placeholder cards into a real story card.
