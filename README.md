# Vishal MV, SEO Specialist Portfolio

A fast, responsive portfolio for an SEO specialist. The design borrows from a search results page: the hero is a search query with the candidate as the top result, and each case study is laid out like a result with its URL line, title and outcome. Dark mode follows the visitor's system setting.

The site also practices what it sells: semantic HTML, Next.js metadata, Open Graph tags, `Person` JSON-LD, `sitemap.xml` and `robots.txt`.

## Tech stack
Next.js 14 (App Router), React 18, TypeScript, Tailwind CSS 3. No API keys or environment variables required.

## Run locally
```bash
npm install
npm run dev
```
Open http://localhost:3000. For a production check: `npm run build && npm start`.

## Customize
- **All text** (name, positioning, stats, case studies, experience, skills, education, certifications) is in `lib/content.ts`.
- **Colors** are CSS variables at the top of `app/globals.css` (light and dark values).
- **Section layout** lives in `components/`, one file per section; reorder sections in `app/page.tsx`.
- **Live URL**: optionally set `NEXT_PUBLIC_SITE_URL=https://your-domain.com` (in `.env.local`) so the sitemap, canonical URL and JSON-LD use your domain.

## Deploy
Push to GitHub and import the repo into Vercel or Netlify. No configuration needed.
