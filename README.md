# Lahcen Bounader — personal academic website

A fast, self-contained static site (no build step, no dependencies). Just HTML, CSS, and a little JavaScript.

```
website/
├── index.html      # main page (about, research, publications, contact)
├── vita.html       # CV page
├── styles.css      # all styling + dark mode
├── script.js       # theme toggle, scroll effects
└── README.md       # this file
```

## Preview locally
Double-click `index.html`, or serve it:
```
cd website
python -m http.server 8000   # then open http://localhost:8000
```

## Deploy to GitHub Pages (free)

1. Create a GitHub account if you don't have one.
2. Create a **new public repository** named exactly:
   **`<your-username>.github.io`** (e.g. `lahcenbounader.github.io`).
3. Upload the contents of this `website/` folder to the repo root
   (so `index.html` sits at the top level — **not** inside a `website/` subfolder).
   - Easiest: on the repo page, click **Add file → Upload files**, drag in
     `index.html`, `vita.html`, `styles.css`, `script.js`, and your photo/CV.
4. Go to **Settings → Pages**. Under *Build and deployment*, set
   **Source = Deploy from a branch**, **Branch = `main` / `root`**, then **Save**.
5. Wait ~1 minute. Your site is live at `https://<your-username>.github.io`.

### Custom domain (optional)
Buy a domain (e.g. `lahcenbounader.com`), then in **Settings → Pages → Custom domain**
enter it and follow the DNS instructions. GitHub gives you free HTTPS.

## Things to personalize
- **Photo:** in `index.html`, replace the `.hero__avatar` initials block with
  `<img src="photo.jpg" alt="Lahcen Bounader" class="hero__photo" />` and drop a
  square `photo.jpg` in this folder.
- **CV PDF:** put `Bounader_CV.pdf` in this folder — the CV buttons already point to it.
- **Accent color:** change `--accent` / `--accent-2` at the top of `styles.css`.
- **Paper links:** the publication links point to RePEc/journal pages — please click
  through and confirm each one resolves; swap in official IMF/journal/DOI URLs where
  you prefer.
- **Replication & Teaching:** fill in the placeholder sections in `index.html` as you
  post files.

## Notes on the content
Publication list was compiled from your RePEc/IDEAS author page (Google Scholar blocks
automated reads). Please double-check titles, co-authors, and especially the external
links before publishing.
