# Cursor-style landing page

A static HTML/CSS landing page inspired by Cursor’s marketing site.

## Tech stack

- **HTML** – single-page structure
- **CSS** – `style.css` for layout and styling
- **Font Awesome** – icons (CDN)
- **Google Fonts** – Century Gothic (CDN)

## Run locally

1. Open the project folder.
2. Serve the files with a local server (so paths resolve correctly), for example:
   - **VS Code:** Install “Live Server” and use “Go Live”.
   - **Node:** `npx serve .` then open `http://localhost:3000`.
   - **Python:** `python -m http.server 8000` then open `http://localhost:8000`.

Or open `index.html` directly in the browser (some features may behave differently without a server).

## Deploy on Vercel

1. Push this repo to GitHub (or connect another Git provider).
2. In [Vercel](https://vercel.com), import the repository.
3. Leave build settings as default (static site).
4. Deploy. The root URL will serve `index.html` automatically.

## Project structure

```
├── index.html          # Main page (entry point for deployment)
├── style.css           # Styles
├── images/             # All images and SVG assets
│   ├── lookup_logo.png
│   ├── image1.png
│   ├── feature1.png, feature2.png, feature3.png
│   ├── story1.png, story2.png, story3.png
│   ├── review2.png … review6.png
│   ├── diana-hu-avatar.webp
│   └── *.svg           # Logo assets (Stripe, OpenAI, etc.)
└── README.md
```

## Notes

- The main page must be named **`index.html`** so the root URL (`/`) works on Vercel and most static hosts.
- Image paths in HTML use the `images/` folder (e.g. `images/lookup_logo.png`); keep that structure when deploying.
