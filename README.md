# Github Portfolio

- **Live site:** https://hisaylama.github.io
- **Repo:** https://github.com/hisaylama

---

## Features
- Minimal, fast, and easy to edit (Markdown-first)
- Home page with hero + featured projects
- Data‑driven projects list via `/_data/projects.yml`
- Optional publications list via `/_data/publications.yml`
- About & Projects subpages
- Works with GitHub Pages out of the box

---

## Quick Start
### 1) Create or use the Pages repo
This repo should be named **`hisaylama.github.io`** (exactly your username).

### 2) Add these files
Make sure the root contains:
```
_config.yml
index.md
about.md
projects.md
_data/projects.yml
_data/publications.yml
assets/img/avatar.svg
404.md
```

### 3) Publish on GitHub Pages
- Go to **Settings → Pages**
- **Source:** `main` branch, `/ (root)`
- Open **https://hisaylama.github.io**

---

## Customize
### Site settings (`_config.yml`)
```yml
title: Hisay Lama homepage
description: Bookmark this to keep an eye on my project updates!
theme: jekyll-theme-minimal
email: hisaylama@gmail.com
github_username: hisaylama
logo: /assets/img/avatar.svg
kaggle_username: hisaylama
linkedin_url: https://www.linkedin.com/in/your-link-here/
timezone: Europe/London
```

### Home page content (`index.md`)
The home page renders a short bio and loops over `/_data/projects.yml` to show featured projects.

### Projects data (`_data/projects.yml`)
Add/edit projects like this:
```yml
- name: AFM HeightProfileApp
  link: https://github.com/hisaylama/AFM-data-height-profile-analysis
  description: MATLAB app to visualize AFM surfaces, extract line profiles, perform baseline correction, and fit peaks.
  tags: [MATLAB, AFM, Gaussian fits]

- name: Statistical Physics Algorithms
  link: https://github.com/hisaylama/Statistical_Physics_Algorithm_Computation
  description: Notebooks on sampling/integration, path integrals, Bose–Einstein stats, and Ising Monte Carlo.
  tags: [Jupyter, Monte Carlo, Ising]
```

### Publications (`_data/publications.yml`)
```yml
- authors: A. Author, H. Lama
  title: Title of the paper
  venue: Journal Name
  year: 2024
  url: https://doi.org/xx.xxxx/xxxxx
```

### Pages
- `about.md` — longer bio
- `projects.md` — lists all items from `/_data/projects.yml`

> Tip: To add a **CV**, upload `cv.pdf` to the repo root and link to it from `index.md` or `_config.yml` (the theme supports `show_downloads` if you want a download link).

---

## Local Preview (optional)
If you want to run it locally before pushing:
```bash
gem install bundler jekyll
jekyll serve
```
Then open http://localhost:4000

---

## Troubleshooting
- **404 on publish:** Ensure **Settings → Pages** points to the `main` branch root.
- **Changes not visible:** Hard refresh (Ctrl/Cmd+Shift+R). Wait ~1 minute for Pages to rebuild.
- **Theme not applied:** Check `theme: jekyll-theme-minimal` in `_config.yml` and that your files are at the repo root.
- **Broken image:** Confirm paths like `/assets/img/avatar.svg` exist and match `_config.yml`.

---

## License & Credits
Content © Hisay Lama. 
