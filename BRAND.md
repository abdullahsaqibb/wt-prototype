# World Treasures visual system

- Midnight navy `#101F38` for header, footer and branded moments.
- Treasure gold `#E7B956` for TREASURES and accents.
- Warm cream `#F6F3EB` for shopping surfaces.
- Hero product-stage backgrounds change with each product (no forced navy).
- Transparent icon asset + live-text wordmark are used in header, footer and intro.
- Intro is approximately 1.85 seconds long and uses lightweight CSS animations.

Primary brand mark: `assets/brand/treasure-mark.svg` (transparent scalable original artwork). Header is navy with white WORLD, gold TREASURES.


## Live colour palette switcher (footer)
The storefront includes three visitor-selectable navy-first palettes. The footer controls apply site-wide and remember the choice in localStorage. The selected hero product still controls its hero background independently.

- **Treasure Gold** (default): Midnight Navy `#101F38`, Gold `#E7B956`, Emerald `#177D69`, Cream `#F6F3EB`.
- **Sunset Coral**: Navy `#12233D`, Coral `#FF795B`, Peach `#F4B9A9`, Ivory `#FFF5EB`.
- **Coastal Teal**: Deep Navy `#0B2135`, Teal `#42CCB4`, Ice Blue `#91C9E7`, Mist `#EFF7F8`.

### Additional themes
- Electric Lime: Navy #10293C · Lime #C6EA58 · Green #409A75 · Paper #F7FAED
- Royal Violet: Navy #1B1C40 · Lilac #B7A2F2 · Violet #8D65BB · Paper #F7F3FF
- Berry Rose: Navy #16253D · Rose #EF8CAA · Berry #B65180 · Paper #FFF4F6
Each product's hero colorway is independent of the global theme.

### Palette implementation note
Product-derived colors apply only to the hero display. The Closer Look background uses each palette's stable `--wt-inspect-bg`, while global brand accent styling uses `--wt-highlight`. Real packaging images are never recolored.
