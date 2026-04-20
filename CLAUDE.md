# Navvix — Project Context for Claude

This is Tim Norris-Wiles' personal site, blog, and portfolio, served at **https://www.navvix.co**.

Repo lives at `/Users/timnw/claudecode/navvix/repo` (origin: https://github.com/typedformiles/navvix.git, branch: main). The parent `navvix/` folder is the working directory but is NOT the git root.

## Stack

- **Jekyll 4.4** static site generator
- **GitHub Pages** hosting, served from `main` branch
- Plain HTML/CSS... no framework, no build pipeline beyond Jekyll
- Custom domain via `CNAME` file
- Analytics via Goat Counter
- Jekyll plugins: `jekyll-sitemap`

Local build: `/opt/homebrew/lib/ruby/gems/4.0.0/bin/jekyll build` or `serve --port 4567`.

## Structure

- `_posts/` — blog posts, filename format `YYYY-MM-DD-slug.md`
- `_posts/drafts/` — local drafts, gitignored, not published
- `_showcase/` — showcase collection items
- `_layouts/` — `default.html`, `post.html`, `showcase-item.html`
- `assets/images/` — all blog and page imagery
- `index.html` — homepage (terminal / ASCII-art aesthetic)
- `about.html` — biography page (prose style, `.post-content` class)
- `blog.html` — blog index
- `showcase.html` — showcase index
- `llms.txt` — machine-readable site overview for LLM crawlers
- `style.css` — single stylesheet for the whole site

## Writing style (important)

- **No em dashes.** Ever. Tim does not use them.
- Use ellipses (`...`) liberally, including in places where grammar purists wouldn't approve. That's intentional and part of his voice.
- Ellipses are NOT a replacement for em dashes... they serve a different purpose (trailing thought, pause).
- Instead of em dashes, use: normal hyphens, commas, semi-colons, or restructure the sentence. Pick whichever reads most naturally.
- Semi-conversational tone. First-person. Opinionated.
- Avoid classic AI lingo endings like "Quietly. Reliably." or aphoristic final paragraphs. Tim will call these out.

## Blog post conventions

Frontmatter template:

```yaml
---
layout: post
title: "Title Here"
date: YYYY-MM-DD
tag: opinion  # one of: opinion, media, video, pr, project, podcast
---
```

Tags map to badge colours defined in `style.css` (`.badge-opinion`, `.badge-media`, etc.).

Permalink config in `_config.yml` is `/blog/:title/`, so a post file `2026-04-17-my-post.md` is served at `/blog/my-post/`.

Images referenced as `/assets/images/filename.ext`.

## SEO and LLM visibility strategy

This is a deliberate focus. Several elements work together:

1. **Static site, no runtime JS dependency.** Google indexes fast and ranks these pages well. Same pattern applied to [isitaderby.co.uk](https://isitaderby.co.uk) which ranks organically on page 1 for competitive football queries. Validated approach.
2. **`llms.txt` file** at the root, following the emerging convention. Lists site purpose, Tim's background, and every blog post grouped by category (Original Writing, Media & Interviews, Video & Podcasts, Press Releases, Side Projects). **Every new blog post MUST be added to `llms.txt`** in the appropriate section.
3. **Jekyll sitemap plugin** generates `sitemap.xml` automatically.
4. **`robots.txt`** explicitly allows all crawlers.
5. **OG tags and canonical URLs** set in `_layouts/default.html` using page-level metadata.
6. **Cross-linking** between related blog posts, and from the About page to relevant posts. Every piece of content should link to at least one other piece of content on the site.
7. **Custom `description` field** in page frontmatter where possible, feeds both `<meta description>` and `og:description`.
8. **Semantic HTML** in layouts (`<article>`, `<nav>`, `<main>`) to help parsers understand structure.

## Playbook for adding a new blog post

1. Create `_posts/YYYY-MM-DD-slug.md` with the frontmatter block above.
2. Pick an appropriate `tag` for badge colour.
3. Add images to `assets/images/` and reference as `/assets/images/filename.ext`.
4. Cross-link to at least one other post on the site where relevant.
5. **Add an entry to `llms.txt`** in the appropriate section with URL, title, and one-line description.
6. Preview locally: `/opt/homebrew/lib/ruby/gems/4.0.0/bin/jekyll serve --port 4567`, visit `http://localhost:4567/blog/slug/`.
7. Commit and push. GitHub Pages rebuilds automatically.

## Useful context

- Tim is currently scaling **Neuralift AI** (deep learning customer segmentation). Blog often touches on AI, martech, adtech, data, sovereign AI, federated learning.
- Previous roles: LiveRamp, Habu (acq. LiveRamp), mParticle (acq. Rokt), Krux (acq. Salesforce), AOL Platforms, WebFusion.
- He writes about industry events he attends... Flower Labs AI Summit, Databricks reports, Retail Media Summit, etc.
- Side projects: `isitaderby.co.uk`, `oneaura.fit` (wife's PT business), moOde audio display, Blissify, DungeonLift.
- The homepage uses a terminal/ASCII aesthetic... don't change this. Other pages use clean prose in `.post-content`.
