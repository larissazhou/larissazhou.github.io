# GitHub Pages Blog Starter (drop-in)

This adds a simple blog to an existing GitHub Pages site using Jekyll and the built-in **minima** theme.

## What this includes
- `_config.yml` → turns your repo into a Jekyll site (your existing static files will still be served)
- `blog/index.md` → blog homepage at `/blog/`
- `_posts/` with a sample post
- optional `Gemfile` for local preview (`bundle exec jekyll serve`)

## How to use
1. Copy these files **into the root** of your existing website repo (do not delete your current files).
2. Commit & push to the branch GitHub Pages is building from (usually `main`).
3. In your site header or homepage, add a link to `/blog/`.
4. Add posts by creating new files in `_posts/` with the format `YYYY-MM-DD-title.md` and front matter like:
   ```yaml
   ---
   layout: post
   title: "My Post Title"
   date: 2025-08-26 10:00:00 +0500
   categories: [notes, personal]
   ---
   ```
5. (Optional) For local preview:
   - Install Ruby + Bundler
   - Run `bundle install`
   - Run `bundle exec jekyll serve` and visit `http://localhost:4000`

If your repo already used GitHub Pages, no extra config is needed. If not, enable it in **Settings → Pages**.