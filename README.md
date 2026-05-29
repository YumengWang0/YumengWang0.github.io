# Yumeng Wang — Personal Webpage

Personal academic and professional website hosted on GitHub Pages.
Live at: [yumengwang0.github.io](https://yumengwang0.github.io)

---

## File Structure

```
├── _layouts/
│   └── default.html        # Main HTML template (nav + CSS wrapper)
├── _includes/
│   └── nav.html            # Navigation bar — edit once, updates all pages
├── assets/css/
│   └── style.css           # All styles and colors
├── images/
│   └── YumengWang.jpg      # Profile photo
├── files/
│   ├── CV_YumengWang.pdf   # CV / resume
│   ├── Paper1.pdf
│   └── Paper2.pdf
├── index.md                # Bio page (homepage)
├── _pages/
│   ├── news.md             # News
│   ├── papers.md           # Publications
│   ├── experience.md       # Work experience + education
│   ├── projects.md         # Personal projects
│   └── contact.md          # Contact
├── _config.yml             # Site settings
└── Gemfile                 # Jekyll dependencies
```

---

## How to Update Content

### Add a news item
Open `_pages/news.md`, copy this block and paste at the top of the list:
```html
<div class="news-item">
  <span class="news-date">MM/YYYY</span>
  <span class="news-text">Your news here.</span>
</div>
```

### Add a paper
Open `_pages/papers.md`, copy this block and paste at the top:
```html
<div class="card">
  <div class="pub-title">Paper title here</div>
  <div class="pub-venue">Journal Name · Year</div>
  <div class="pub-authors"><span class="pub-me">Yumeng Wang</span>, Co-author Name</div>
  <a href="/files/PaperX.pdf" target="_blank" class="btn-outline">PDF</a>
</div>
```
Then upload the PDF to the `files/` folder.

### Add a project
Open `_pages/projects.md`, copy this block:
```html
<div class="card">
  <div class="proj-title">Project title</div>
  <div class="proj-tech">Tech stack · Tools used</div>
  <div class="proj-desc">Brief description of the project.</div>
  <a href="https://github.com/YumengWang0/repo" target="_blank" class="btn-outline">GitHub</a>
</div>
```

### Update bio text
Open `index.md` and edit the paragraph inside `<p class="hero-bio">`.

### Update availability status
Open `index.md` and find:
```html
Available for full-time roles · August 2026
```
Change the text or remove the whole `available-badge` block when no longer job searching.

### Replace profile photo
Upload a new photo to `images/` and name it `YumengWang.jpg`.
Make sure it is a square crop for best results.

### Replace CV
Upload new PDF to `files/` and name it `CV_YumengWang.pdf`.

### Change colors
Open `assets/css/style.css` and edit the variables at the top:
```css
:root {
  --accent:  #f59e0b;   /* amber — main highlight color */
  --bg:      #1c1c1e;   /* dark background */
  --text-1:  #f0ebe0;   /* primary text */
  --text-2:  #a89880;   /* secondary text */
}
```

---

## Deployment

This site uses **Jekyll** and is hosted on **GitHub Pages**.

- Push any change to the `main` branch
- GitHub automatically rebuilds the site in 1–2 minutes
- No local setup required

---

## Tech Stack

- Jekyll (static site generator)
- GitHub Pages (hosting)
- HTML / CSS (no JavaScript frameworks)
- Google Fonts: Syne + Outfit
