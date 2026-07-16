# Deniz Ece Dalgic-Tetikol — consultant site

Personal / professional site for **Deniz Ece Dalgic-Tetikol, PhD** — an
independent economist and regulatory consultant working on energy, transport,
and network industries. It's a static site (HTML + CSS + a little vanilla JS)
built to be hosted on GitHub Pages.

No build step, no framework. Edit the files, push, and the site updates.

The site is structured to market independent consultancy work: it leads with
**services** ("How I can help") and **selected projects**, then experience,
expertise/credentials, and publications.

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The whole site (hero, about, services, projects, experience, expertise, publications, contact) |
| `styles.css` | Styling, light/dark themes |
| `script.js` | Theme toggle + footer year |
| `assets/headshot.jpg` | Profile photo |
| `robots.txt` / `sitemap.xml` | SEO helpers |
| `.nojekyll` | Tells GitHub Pages to serve files as-is |

## Before you publish — fill in the placeholders

The site is configured for the custom domain **`ddalgic.com`** (see the `CNAME`
file and the absolute URLs in `index.html`, `robots.txt`, and `sitemap.xml`).
All internal links and asset paths are **relative**, so the site also works at
`https://<username>.github.io/deniz-resume/` without changes.

Contact details (email + LinkedIn) are already filled in the Contact section.

## Editing content

Everything lives in `index.html`, organized into numbered sections. Edit the text
directly. The colour accent, fonts, and spacing are CSS variables at the top of
`styles.css` (`--accent` is the deep-teal accent).

### Adding a project

Copy one `<li class="project"> … </li>` block inside `<ul class="projects">` and
edit the title, client, role, description, and `<li>` tags.

### Adding a service

Copy an `<article class="card"> … </article>` block inside `<div class="cards">`.

## Publishing on GitHub Pages

1. Push this repo to GitHub.
2. Repo **Settings → Pages**.
3. Under **Build and deployment**, set **Source: Deploy from a branch**, pick the
   branch and `/ (root)` folder, then **Save**.
4. (Optional) To use a custom domain, add a `CNAME` file containing just your
   domain, enter the domain under **Settings → Pages → Custom domain**, and point
   your DNS at GitHub Pages. See the GitHub docs on
   [configuring a custom domain](https://docs.github.com/en/pages/configuring-a-custom-domain-for-your-github-pages-site).
