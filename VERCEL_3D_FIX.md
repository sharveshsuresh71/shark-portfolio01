# Vercel asset fix

The original project referenced Lovable-only `/__l5e/assets-v1/...` image URLs.
Those URLs are not present on Vercel.

This rebuild stores four self-contained local assets in `public/`:
- `blackhole.jpg`
- `starfield.jpg`
- `moon.jpg`
- `mountains.jpg`

The homepage now references them as root-relative URLs (`/blackhole.jpg`, etc.).
No Lovable asset manifest is required for these images.

Deploy with:
- Build command: `npm run build`
- Output directory: `dist`
