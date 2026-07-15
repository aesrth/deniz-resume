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

A few things are intentionally left as clearly-marked placeholders:

1. **Contact details** — in `index.html`, the Contact section (`#contact`) has a
   `TODO` comment. Replace the `mailto:hello@example.com` email, the LinkedIn URL,
   and the Scholar URL with the real ones (or remove any card you don't want).
2. **Domain / SEO URLs** — several tags use `https://deniz-dalgic.example.com/`
   as a placeholder: `<link rel="canonical">`, the `og:url`/`og:image` meta tags,
   and the JSON-LD `url`/`image` in `index.html`, plus `robots.txt` and
   `sitemap.xml`. Once you pick a domain, do a find-and-replace on
   `deniz-dalgic.example.com` and update the relative `assets/headshot.jpg`
   image URLs to absolute ones so link previews render.

All internal links and asset paths are **relative**, so the site works both at
`https://<username>.github.io/deniz-resume/` and at a custom domain root without
any changes.

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
