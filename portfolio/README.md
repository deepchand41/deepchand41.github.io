# Deepchand's Portfolio

A clean, editorial-style personal portfolio site — inspired by nirajbasnet.github.io.

## Files

| File | Purpose |
|------|---------|
| `index.html` | Home / hero page |
| `about.html` | About me + skills |
| `works.html` | Professional experience (timeline) |
| `projects.html` | Project cards |
| `blogs.html` | Blog post list |
| `contact.html` | Contact links |
| `style.css` | All styles |
| `main.js` | Mobile nav + fade-in |

---

## 🚀 How to deploy on GitHub Pages

### Step 1 — Backup your current repo (optional)
In your current repo, you can create a branch to save the old Jekyll site:
```
git checkout -b old-jekyll-site
git push origin old-jekyll-site
```

### Step 2 — Clear the main branch
In your `deepchand41.github.io` repo on GitHub:
1. Go to **Settings → Branches** and make sure `main` is the default branch.
2. Clone the repo locally (if you haven't already):
   ```
   git clone https://github.com/deepchand41/deepchand41.github.io.git
   cd deepchand41.github.io
   ```

### Step 3 — Replace the files
Delete all old files except `.git/`, then copy in the new files:
```bash
# From inside the cloned repo folder:
find . -not -path './.git*' -delete   # removes old files
# Now copy in the 7 new files: index.html, about.html, works.html,
# projects.html, blogs.html, contact.html, style.css, main.js
```

Or just drag-and-drop the new files into the GitHub web UI and commit.

### Step 4 — Push & enable GitHub Pages
```bash
git add .
git commit -m "Replace Jekyll site with new HTML portfolio"
git push origin main
```

Then on GitHub:
1. Go to **Settings → Pages**
2. Source: **Deploy from a branch**
3. Branch: `main`, folder: `/ (root)`
4. Click **Save**

Your site will be live at **https://deepchand41.github.io** within a minute or two.

---

## ✏️ Customisation Checklist

Replace all placeholder content with your real info:

- [ ] **index.html** — Update role/tagline and bio text
- [ ] **about.html** — Rewrite bio paragraphs + update skills list
- [ ] **works.html** — Add your real jobs, dates, and bullet points
- [ ] **projects.html** — Replace project cards with your actual projects + GitHub links
- [ ] **blogs.html** — Link to your real blog posts (or your existing Jekyll posts)
- [ ] **contact.html** — Add your real email and LinkedIn URL
- [ ] All pages — Replace `your@email.com` and LinkedIn URL in footer
- [ ] **Profile photo** — Put your photo at `images/profile.jpg` and replace the `hero-image-placeholder` div with `<img src="images/profile.jpg" alt="Deepchand" />`

---

## 🎨 Customising the look

Open `style.css` and adjust the `:root` variables at the top:

```css
:root {
  --bg: #f9f7f4;          /* page background */
  --fg: #1a1714;          /* main text */
  --accent: #8b4a2f;      /* highlight colour — change this to your preference */
  --muted: #6b6560;       /* secondary text */
}
```
