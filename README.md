# Mudassir Usmani — CV

Interactive one-page CV: switch between a **Researcher** and an **Engineer** view, filter by topic or skill, and expand any entry for details. It also prints cleanly to PDF.

## Publish on GitHub Pages

1. Create a new public repository on GitHub (for example `cv`).
2. Upload `index.html` and this `README.md` (**Add file → Upload files**), then commit.
3. Go to **Settings → Pages**, set *Source* to **Deploy from a branch**, choose `main` and `/ (root)`, and save.
4. After a minute the site is live at `https://usmani-m.github.io/cv/`.

> To serve it at `https://usmani-m.github.io/` instead, name the repository `usmani-m.github.io`.

## Editing

All content is in the `<script>` block near the bottom of `index.html`:

- `PROFILE`: headline and summary for each view
- `CONTACTS`, `STATS`
- `SECTIONS`: experience, publications, projects and so on. Each entry has `tags` (topic filters) and `skills` (which must match a name in `SKILLS`).
- `ORDER`: the section order for each view

You don't need a build step; it's plain HTML, CSS and JavaScript.
