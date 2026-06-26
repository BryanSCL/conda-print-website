# Conda Print & Bind — Website

A single-file, responsive website for **Conda Print & Bind** (Bras Basah Complex, Singapore).
Everything lives in **`index.html`** — HTML, CSS, and JavaScript in one file, with no
external build step and no image files to manage.

- **Phone:** +65 6336 7244
- **Address:** 231 Bain St, #01-71, Bras Basah Complex, Singapore 180231
- **Hours:** Mon–Fri 10.30am–6.30pm · Sat 10.30am–5pm · Sun & PH closed

---

## Publish it on GitHub

You need a free GitHub account: https://github.com/signup

### Option A — Upload in the browser (no commands)

1. Go to https://github.com/new and create a repository, e.g. `conda-website`. Leave it **Public**.
2. On the new repo page, click **"uploading an existing file"**.
3. Drag in **`index.html`** and **`README.md`** from this folder, then click **Commit changes**.

### Option B — Push from your computer (Git command line)

First create an **empty** repo on github.com (no README), and copy its URL.
Then, from a terminal **inside this folder**:

```bash
git init
git add .
git commit -m "Initial commit: Conda Print & Bind website"
git branch -M main
git remote add origin https://github.com/YOUR-USERNAME/conda-website.git
git push -u origin main
```

---

## Put it online for free (GitHub Pages)

1. In your repo, go to **Settings → Pages**.
2. Under **Build and deployment → Source**, choose **Deploy from a branch**.
3. Branch: **main**, folder: **/ (root)**. Click **Save**.
4. Wait ~1 minute. Your site goes live at:
   `https://YOUR-USERNAME.github.io/conda-website/`

Because the homepage is named `index.html`, GitHub Pages serves it automatically.

---

## How to keep editing later

### Quick edits in the browser
1. Open your repo on GitHub and click **`index.html`**.
2. Click the **pencil (✏️) icon** at the top right to edit.
3. Make your change, scroll down, and click **Commit changes**.
   If GitHub Pages is on, the live site updates within a minute.

### Common things you may want to change
All of these are plain text inside `index.html` — use your browser's find (Ctrl/Cmd-F) to locate them:

- **Phone number:** search for `6336 7244` and `tel:+6563367244` (update both).
- **Address:** search for `231 Bain St`.
- **Opening hours:** search for `Opening hours` / `10.30am`.
- **Services:** search for `What we offer` to find the service cards.
- **Colours:** near the top, inside `:root{ ... }`, change `--ink` (main blue) and
  `--accent` (orange). Every element using them updates automatically.
- **Add an email later:** search for the contact section (`id="contact"`) and add a row;
  for a clickable email use `<a href="mailto:you@example.com">you@example.com</a>`.
- **Add photos later:** replace any CSS graphic block with an `<img src="...">` tag, or
  add an image to the repo and reference it by filename.

### Editing on your computer
```bash
git clone https://github.com/YOUR-USERNAME/conda-website.git
cd conda-website
# open index.html in any editor or double-click to preview in a browser
git add .
git commit -m "Update site"
git push
```

---

## Notes

- The site is fully self-contained: no photos, no dependencies, fast to load.
- Business details were compiled from Conda's public business listing. Verified Google
  review snippets/star rating and social links can be added later if