# FormX Golf

Golf tech & gear review site built with Astro. Deploys to Cloudflare Pages.

## Getting Started

```bash
npm install
npm run dev
```

Open http://localhost:4321

## Publishing a New Article

1. Create a new `.md` file in `src/content/articles/`
2. Use this frontmatter:

```markdown
---
title: "Your Article Title"
description: "A short description for SEO and card previews."
pubDate: "2026-06-10"
category: "GPS Watches"   # or: Rangefinders, Launch Monitors, Simulators, Swing Analyzers
featured: false           # set to true to show in Featured section
---

Your article content here in Markdown...
```

3. Save, commit, push to GitHub → Cloudflare Pages auto-deploys.

## Deploy to Cloudflare Pages

1. Push this repo to GitHub
2. In Cloudflare Pages → Create a project → Connect to GitHub repo
3. Build settings:
   - **Build command:** `npm run build`
   - **Output directory:** `dist`
4. Add custom domain: `formxgolf.com`

## Structure

```
src/
  content/articles/   ← Your Markdown articles go here
  layouts/            ← Page templates
  components/         ← Header, Footer, ArticleCard
  pages/              ← Routes (index, about, disclosure, articles)
public/               ← Static assets (favicon, images)
```
