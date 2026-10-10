# Resume site

A static resume site (plain HTML and CSS, no build step, no backend).

## Before you deploy

1. Pick your final URL (for example `https://siddharth-palnitkar.vercel.app`).
2. Find and replace `https://YOUR-SITE.vercel.app` with it in:
   `public/index.html`, `public/robots.txt`, `public/sitemap.xml`, `public/llms.txt`.
3. Check the LinkedIn URL in `public/index.html`, `public/llms.txt` and `public/resume.md`.

## Deploy on Vercel

1. Push this folder's contents to a GitHub repository.
2. In Vercel: Add New, Project, import the repository.
3. Framework Preset: **Other**. Leave Build Command and Install Command empty.
   The output directory comes from `vercel.json` (`public`).
4. Deploy. Every push to `main` redeploys automatically.

## How it is made readable by chatbots

- Semantic HTML (one `h1`, sections with headings, a real table for education).
- `schema.org` Person data in JSON-LD inside `index.html`.
- `/resume.md` is the same resume as plain Markdown.
- `/llms.txt` summarizes the site for AI assistants.
- `/robots.txt` explicitly allows common AI crawlers, and `/sitemap.xml` lists the pages.

## Privacy

No phone number or home address appears anywhere in the site or its metadata.
