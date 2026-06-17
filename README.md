# Your GIS Portfolio

A static portfolio site for showcasing GIS, remote sensing, and spatial analysis projects. Designed to be easy to extend — add a new project any time you finish one.

## What's in here

```
index.html              Home page
projects.html            Grid of all projects ("plates")
about.html               About / education / skills
css/style.css            All styling (one shared stylesheet)
images/                   All map images / screenshots
projects/                 One HTML file per project (case studies)
projects/_template.html   Copy this to start a new project page
projects/data/            Downloadable data files referenced by project pages
```

## 1. Fill in your details

Before publishing, search every HTML file for these placeholders and replace them:

- `YOUR NAME` / `Your Name` — your actual name
- `you@example.com` — your email
- `linkedin.com/in/yourprofile` — your LinkedIn URL
- `github.com/yourusername` — your GitHub URL
- `[University name]`, `[Expected graduation year]`, etc. in `about.html`
- `assets/resume.pdf` / `assets/resume.docx` — your résumé in both formats. Already filled in; replace these two files (keep the same filenames) whenever you update your resume, and the `resume.html` page and download buttons will pick up the new version automatically.

## 2. Add a new project (do this every time you finish one)

1. Copy `projects/_template.html`, rename it to something like `projects/my-new-project.html`.
2. Open it and replace every `[bracketed]` placeholder with your real content.
3. Drop your map images into `/images/` and point the `<img src="...">` tags at them.
4. If you have supporting data files (Excel, CSV, shapefiles zipped up, etc.), put them in `projects/data/` and link them from the "Data & downloads" section.
5. Open `projects.html`, copy the existing `<div class="plate">...</div>` block, paste a new one above it (newest projects go at the top), and update the title, thumbnail image, summary, tags, and the link to your new project page.
6. Optional: if it's your best/most recent work, also update the "Featured" plate on `index.html` the same way.

That's the whole workflow — no rebuild step, no framework, just plain HTML files.

## 3. Host it for free on GitHub Pages

1. Create a free GitHub account if you don't have one, and create a new repository (e.g. `gis-portfolio`).
2. Upload everything in this folder to that repository (drag-and-drop works on github.com, or use `git push` if you're comfortable with Git).
3. In the repository, go to **Settings → Pages**.
4. Under "Build and deployment", set **Source** to "Deploy from a branch", choose the `main` branch and `/ (root)` folder, then save.
5. GitHub will give you a live URL, usually `https://yourusername.github.io/gis-portfolio/`, within a minute or two.
6. Every time you push an update (e.g. a new project page), the live site updates automatically within a minute.

That URL is what you put on your CV, LinkedIn, and job applications.

## Notes

- The design borrows its visual language from the maps themselves — neatline borders, north arrows, scale-bar styling, "plate" numbering — so new projects will automatically look at home here, since they're map outputs too.
- The site uses Google Fonts (Fraunces, Inter, IBM Plex Mono) loaded via a CDN link in `css/style.css` — this just needs an internet connection when someone views the site, nothing to install.
- No build tools, frameworks, or dependencies. Any text editor works for future edits.
