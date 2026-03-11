# HARI Engineering Website (Static Export for cPanel)

This repository contains the HARI Engineering marketing website + /portal UI shell.

## Tech
- Next.js (App Router)
- Tailwind CSS
- Static export (`next export`) for shared hosting (cPanel)

## Development
```bash
npm install
npm run dev
```

## Build & Export
```bash
npm run export
```
This generates an `out/` folder.

## Deploy to cPanel
1. In cPanel File Manager, open `public_html/`
2. Upload the **contents of `out/`** into `public_html/`
3. Ensure your domain points to this hosting account

## WhatsApp Button
WhatsApp floating button is shown on public pages only (not on `/portal`).

## Trusted By Logos
Place client logos in `public/logos` and they will render grayscale -> color on hover.

## Supabase (Portal backend)
Create `.env.local` (do not commit):
```bash
NEXT_PUBLIC_SUPABASE_URL=...
NEXT_PUBLIC_SUPABASE_ANON_KEY=...
```
SQL templates are in `supabase/`.