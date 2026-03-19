# Juan Joy - Personal Site v2

A bold, editorial-style personal website built with Hugo. Features a tabbed projects section, work experience timeline, blog, and about page.

---

## Quick Start

### 1. Install Hugo

**Mac:** `brew install hugo`
**Windows:** `choco install hugo-extended`
**Linux:** `sudo snap install hugo`

### 2. Run Locally

```bash
cd hugo-site-v2
hugo server -D
```

Open [http://localhost:1313](http://localhost:1313)

---

## Deploy to GitHub Pages (Free)

1. Create repo named `yourusername.github.io` on GitHub
2. Push:
```bash
git init
git add .
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/yourusername/yourusername.github.io.git
git push -u origin main
```
3. Go to repo → Settings → Pages → Source → **GitHub Actions**
4. Site goes live at `https://yourusername.github.io` in ~2 minutes

---

## How to Update Content

### Add a new blog post
```bash
hugo new blog/my-new-post.md
```
Edit the file, set `draft: false`, then `git add . && git commit -m "new post" && git push`.

### Add a new project
```bash
hugo new projects/my-project.md
```

### Edit work experience
Open `data/work.yaml` - each job is a YAML entry with title, company, location, period, bullets, and tags. Add, remove, or reorder entries.

### Edit community engagement
Open `data/community.yaml` - same format as work.

### Edit the about page
Open `content/about/index.md`.

### Edit the hero text or Light Patches tab
Open `layouts/index.html` - the hero and Light Patches content are directly in this template.

### Change colors or fonts
Edit `static/css/style.css` - all values are in CSS variables at the top.

---

## File Structure

```
hugo-site-v2/
├── archetypes/          # Templates for new content
├── content/
│   ├── about/           # About page
│   ├── blog/            # Blog posts (Markdown)
│   └── projects/        # Project pages (Markdown)
├── data/
│   ├── work.yaml        # Work experience timeline data
│   └── community.yaml   # Community engagement data
├── layouts/
│   ├── _default/        # Fallback templates
│   ├── about/           # About page layout
│   ├── blog/            # Blog list + single layouts
│   ├── partials/        # Header + footer
│   ├── projects/        # Project list + single layouts
│   └── index.html       # Homepage (hero, tabs, timeline, blog)
├── static/
│   ├── css/style.css    # All styles
│   └── js/main.js       # Tab switching + smooth scroll
├── .github/workflows/   # Auto-deploy to GitHub Pages
├── hugo.toml            # Site config
└── README.md
```

---

## Optional: Custom Domain

1. Buy a domain (~$10/year) from Namecheap, Cloudflare, or Porkbun
2. Add DNS records:
   - A records: `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
   - CNAME: `www` → `yourusername.github.io`
3. GitHub repo → Settings → Pages → Custom domain → enter your domain
4. Update `baseURL` in `hugo.toml`
