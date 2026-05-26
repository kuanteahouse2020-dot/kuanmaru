# kuanmaru — personal site

Personal website for kuanmaru, sound artist & certified tea master.

Single-page static site. Pure HTML + CSS, no build step.

---

## How to deploy on GitHub Pages

### 1. Create a new repository

Go to https://github.com/new and create a public repo. Name suggestion:

- **`kuanmaru.github.io`** — if you want the URL to be `https://kuanmaru.github.io` (replace `kuanmaru` with your actual GitHub username)
- **`kuanmaru-site`** — if you want the URL to be `https://YOUR-USERNAME.github.io/kuanmaru-site/`

The first option gives a cleaner URL — recommended.

### 2. Upload these files

Upload three files to the root of the repo:

```
index.html
style.css
README.md   (this file, optional)
```

You can do this via the web interface ("Add file → Upload files") or via git command line.

### 3. Enable GitHub Pages

In the repo: **Settings → Pages**

- Source: `Deploy from a branch`
- Branch: `main` (or `master`) — folder: `/ (root)`
- Save

Wait 1–3 minutes. Your site will be live at:
`https://YOUR-USERNAME.github.io/` (or `/kuanmaru-site/` for the second naming option).

### 4. (Optional) Custom domain

If you buy a domain (e.g. `kuanmaru.com`):

1. In repo **Settings → Pages → Custom domain**, enter your domain.
2. At your domain registrar's DNS settings, add these A records pointing to GitHub:
   ```
   185.199.108.153
   185.199.109.153
   185.199.110.153
   185.199.111.153
   ```
3. Wait 10 min – 24 h for DNS to propagate.
4. Tick **Enforce HTTPS** in GitHub Pages settings.

---

## File structure

```
kuanmaru-site/
├── index.html       — page markup
├── style.css        — all styling
└── README.md        — this file
```

No JavaScript dependencies. Loads two Google Fonts (EB Garamond, JetBrains Mono, Noto Serif TC).

---

## Editing content

All content is in `index.html`. Sections are clearly marked with comments like `<!-- ============ ABOUT ============ -->`. To edit:

- Open `index.html` on github.com → click the pencil icon → edit → commit.
- Or download, edit locally, re-upload.

GitHub Pages re-deploys automatically within ~1 minute after each commit.
