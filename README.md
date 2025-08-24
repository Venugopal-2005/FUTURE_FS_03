# PatagonAI — AI Redesign (Next.js + Tailwind + Firebase/Strapi-ready)

This is a **unique AI-assisted concept redesign** of an outdoor brand. It ships with:
- **Modern UI** (Next.js App Router + Tailwind)
- **AI branding** (procedural color palette + SVG logo in `/public/logo.svg`)
- **SEO** (`robots.ts`, `sitemap.ts`, Open Graph/Twitter)
- **Mobile-first** responsive pages
- **CMS-ready** with adapters for **Strapi** (via env `NEXT_PUBLIC_STRAPI_URL`) or local mock data. Firebase boilerplate is included in `lib/firebase.ts`.

## Run
```bash
npm i
cp .env.example .env.local   # optional
npm run dev
```
Open http://localhost:3000 (or the next available port).

## Configure Strapi (optional)
Set `NEXT_PUBLIC_STRAPI_URL=https://your-strapi-domain` in `.env.local`.  
Ensure a `posts` collection exists with fields: `title`, `excerpt`, `cover` (media), `publishedAt`.

## Pages
/ — Hero + latest posts  
/products — product grid  
/sustainability — concept initiatives  
/blog — posts (Strapi if configured, otherwise mock)  
/about — concept rationale

## Notes
- This is an educational concept and not affiliated with any real brand.
- Re-theme by editing `branding.palette.json` or replacing `/public/logo.svg`.
