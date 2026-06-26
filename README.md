# Mya Bolds personal site (al-folio)

This is Mya Bolds' personal academic site, built on the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme 


<!-- 
and filled in with her real CV — about page, CV (rendered from `assets/json/resume.json`, plus the original CV PDF), publications, teaching, projects, and news.

The repo has been trimmed down from the stock theme: demo blog posts, sample projects/books, and most of the theme's CI workflows have been removed, keeping only the one that builds and deploys the site.

<!-- ## 1. View it

You don't need to install anything to look at the site before publishing it — pick whichever of these is easiest:

**Option A — GitHub Codespaces (zero install, recommended for a first look)**
1. Push this repo to GitHub (see step 2 below).
2. On the repo's GitHub page, click the green **Code** button → **Codespaces** tab → **Create codespace on main**.
3. The container is pre-configured (`.devcontainer/`) to install Ruby/Jekyll and run the site automatically. Give it a minute or two on first launch, then a "Open in Browser" popup/port-forward notification will let you view the live site. Edits you make and save will auto-reload.

**Option B — Docker, on your own machine**
1. Install [Docker Desktop](https://www.docker.com/products/docker-desktop/).
2. From this folder, run:
   ```bash
   docker compose up
   ```
3. Open **http://localhost:8080** in your browser. First run takes a few minutes to build the image; later runs are fast, and the site live-reloads as you edit files. -->
<!-- 
**Option C — Ruby/Jekyll directly on your machine**
1. Install Ruby (3.x) and Bundler.
2. From this folder, run:
   ```bash
   bundle install
   bundle exec jekyll serve
   ```
3. Open **http://localhost:4000** in your browser. -->

> I built and edited all the content files here, but I can't actually run Ruby/Jekyll in my own sandbox to render a live preview for you — so use one of the options above for the first real look before you publish.

## 2. Post it (publish to GitHub Pages)

1. **Create a repo.** On GitHub, create a new repository named exactly `<your-username>.github.io` (use your real GitHub username) — this makes your site live at the root of that domain. (A different repo name also works; your site just lives at `<your-username>.github.io/<repo-name>` instead — see the note in `_config.yml` about `baseurl` if you go this route.)

2. **Push this folder to it:**
   ```bash
   cd al-folio
   git init
   git add .
   git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```

3. **Update `_config.yml`.** Open `_config.yml` and change the `url` field near the top to match your actual repo (e.g. `https://<your-username>.github.io`), and set `baseurl` to `""` if it's a `<username>.github.io` repo, or `/<repo-name>` otherwise. Commit and push that change.

4. **Let GitHub Actions build it.** Pushing to `main` triggers `.github/workflows/deploy.yml`, which installs everything, builds the site, and pushes the result to a `gh-pages` branch — you don't need to build anything locally for this to work. Check the **Actions** tab on your repo to watch it run (takes a couple of minutes).

5. **Turn on Pages.** Once that workflow finishes (and a `gh-pages` branch has appeared in your repo), go to **Settings → Pages**, and under "Build and deployment" set:
   - Source: **Deploy from a branch**
   - Branch: **gh-pages** / `(root)`

   Save. Your site will be live at the URL you set in step 3 within a minute or two.

After that, any future push to `main` re-builds and re-publishes automatically.

## 3. Things worth doing before/after you publish

- **Add your socials.** `_data/socials.yml` has your email and CV wired up; uncomment and fill in `github_username`, `linkedin_username`, `orcid_id`, or `scholar_userid` if you'd like those icons to show.
- **Keep the CV PDF in sync.** `assets/pdf/Mya_Bolds_CV.pdf` is the file you uploaded. If you update your CV, replace that file (same filename) and update `assets/json/resume.json` to match, so the on-page CV and the PDF download stay consistent.
- **`giscus` comments / analytics / newsletter** are all off by default — see the relevant sections in `_config.yml` if you want to turn any of them on later.

## What's where

- `_pages/about.md` — homepage bio
- `_pages/cv.md` + `assets/json/resume.json` + `assets/pdf/Mya_Bolds_CV.pdf` — CV page (rendered + downloadable PDF)
- `_bibliography/papers.bib` — publications
- `_projects/` — three research project write-ups
- `_teachings/` — your three TA roles
- `_news/` — short announcements shown on the homepage
- `_data/socials.yml` — contact/social icons
- `_config.yml` — site-wide settings (name, description, url, nav, etc.)

## Credit

Built on [al-folio](https://github.com/alshedivat/al-folio), licensed under the MIT License (see `LICENSE`). -->
