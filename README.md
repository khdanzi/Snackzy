# Snackzy

    npm install
    npm run dev      # http://localhost:3000
    npm run build && npm start

## Where things live
- `src/config/site-config.ts` — business details, currency (AED) / locale (en-AE), contact, story copy (DRAFT), image paths. Placeholders are marked.
- `src/config/menu-data.ts` — editable menu; add `image` + `imageAlt` to any item to give it a photo.
- `src/lib/format.ts` — the ONLY price formatter. `src/lib/contact.ts` — WhatsApp order links.
- `src/app/globals.css` — brand tokens (`--color-brand` is the red/pink; change it once).
- Real photos: `public/images/` (webp). Hero cutout: `hero-burger.webp` (transparent).

## Still placeholders (replace before launch)

- WhatsApp number, phone, email, address, hours, Instagram/TikTok URLs, Google Maps URL (site-config.ts)
- Photos needed: chicken sandwich, loaded fries, drinks/coffee (menu items without photos show text-only rows)

## Pull-it-apart section
Built from the real double-smash photo. `public/images/burger/*.webp` are the cut-out layers
(bun, onion-patty, patty, base + flying bits); `src/config/burger-layers.json` holds their
positions in the source photo. Offsets/captions live in `src/components/burger/ExplodedBurger.tsx`.

## Logo
`public/images/logo-white.webp` (lockup), `logo-mark-white.webp` (nav), `logo-red.webp` (light backgrounds);
paths/sizes in `siteConfig.logo`. Favicon: `src/app/icon.png`.
