# World Treasures — November 2026 brand refresh

## Logo
The existing open mystery-box logo illustration and rounded type silhouette are retained. The dark ink has been recolored to cream-white for the icon and WORLD, and muted treasure gold for TREASURES. Transparent WebP assets are in `assets/brand/`.

## Website palette
- Midnight navy: `#101F38` — header, footer and intro
- Treasure gold: `#E7B956` — logo accent, highlights and CTA
- Emerald green: `#177D69` — secondary accents and feedback
- Warm cream: `#F6F3EB` — shopping surfaces
- White: `#FFFFFF` — logo WORLD and text on dark surfaces

## Motion
The intro uses the actual product images in a perspective-based multi-face CSS 3D film, with chip particles and GSAP timing. This gives dimensional movement without loading heavy 3D meshes. It is **not** a fully modeled photorealistic packet with accurate printed backs/sides; those require licensed 3D assets. A product photo follows a curved path to the cart on add, implemented with native Web Animations API.
