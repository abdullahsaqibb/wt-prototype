# World Treasures

Interactive imported snacks and drinks storefront prototype for South Africa.

## Upload to GitHub

1. Extract the ZIP on your computer.
2. Create a repository, for example `world-treasures`.
3. Upload the extracted files and the `assets` folder into the repository root. Upload the contents, not the ZIP or an extra enclosing folder.
4. Confirm that `index.html`, `vercel.json` and this README are visible at the top level, then commit to `main`.

## Deploy on Vercel

1. Import the GitHub repository into Vercel.
2. Use Framework Preset **Other** and the repository root as Root Directory.
3. The included `vercel.json` sets an empty Build Command and Install Command, with Output Directory `.`. No dependency installation or build is needed.
4. Deploy. No environment variables are required for this prototype.

Once Git integration is connected, commits to the configured production branch can deploy automatically. Use pull requests and preview deployments for reviewing later changes.

Vercel documentation: https://vercel.com/docs/builds/configure-a-build

## Files

- `index.html`: complete site, including inline CSS, JavaScript, product pictures and approved logo. This is the source to edit.
- `vercel.json`: static deployment settings.
- `assets/brand/`: standalone copies of the approved logo and icon for reuse. The page already embeds them, so they are not required to render the page.
- `BRAND.md`: approved palette and typography.

## Preview locally

Open `index.html` in a modern browser, or serve this directory using an existing static file server. Google Fonts and GSAP/ScrollTrigger require an internet connection. Product pictures and logo artwork are embedded in the HTML.

## Included functionality

- 15 products with category filters and search.
- Swipe, drag, horizontal trackpad and keyboard carousel controls.
- Intro, product assembly, scroll and hover animations, with reduced-motion support.
- Product details, configurable three-pack, shopping bag and checkout demo.
- Store pickup and sample local delivery zones.
- Card-only Payfast-style simulation, including cancellation and confirmation.
- WhatsApp enquiries to +92 315 0987000, including product-specific messages.
- Email contact: noveelkhan0@gmail.com.

WhatsApp links open a prefilled chat; visitors send the message themselves. Email links open the visitor's email application. No messages are sent by the website automatically.

## Prototype boundaries

This is a UI prototype, not a live ecommerce backend. Prices, stock, delivery zones, fees, times, reviews, address and opening hours are illustrative. Check product ingredients, allergens, origins and image permissions before commercial launch. Product source credits are included in the footer.

Cart state is in browser memory and resets on reload. Sign-in and newsletter submission are demonstrations; they do not create accounts or send email. The payment screen is a local simulation, not Payfast's live or sandbox checkout. It collects no card details, takes no money and creates no real order.

## Next development phase

Connect the repository and Vercel project for ongoing code changes. Add a backend for products, orders and authentication, then integrate Payfast on the server with verified payment notifications and real fulfillment rules. Keep merchant credentials in environment variables, never in this HTML or Git history.

## November 2026 visual update

- Brand assets updated to white/gold on navy and the palette revised across the website.
- New product-led perspective intro (Lay's, Takis, Red Bull), with a cinematic spin and particle accents. GSAP is loaded from CDN; the intro has a fallback if unavailable.
- Add-to-cart now flies an actual product photo to the cart icon using browser-native Web Animations, with cart bounce feedback.
- Reduced-motion settings bypass decorative sequences.
- Product images and demo commerce data remain illustrative. Exact real-world 3D packet backs and geometry are not available in the source package.
- Replace repository root files with the contents of this ZIP; do not upload the ZIP itself as a single GitHub file.

## November refinement

Short text-first brand reveal (skip/replay supported), dynamic product-color hero background restored, and full-sized product-to-header-cart animation that scales down along a curved path. The old resource-intensive pseudo-3D opener is removed. Text-and-icon brand lockup has no baked-in rectangular background.

## November 18 navigation and identity update

- Header remains sticky and floats above page content while scrolling; cart remains an accessible target.
- New scalable SVG mystery-box mark, aligned wordmark, white WORLD / gold TREASURES.
- Short vector brand reveal with two snack packs dropping into basket (about 1.65 seconds).
- Cart image animation now targets the bag icon inside the fixed header.
- Product-dependent carousel backgrounds stay in place.
- For best results preview and test on mobile before production.

## Navigation update — desktop/full-width, mobile/floating
- Desktop (>760px): full-width navy navigation bar remains visible while scrolling.
- Mobile (<=760px): floating rounded navy navigation remains visible while scrolling.
- Existing cart button remains in the persistent header, preserving the flying-to-cart target.
- Logo and intro animation deliberately left unchanged pending visual direction approval.

## November 2026 performance and identity update

- Desktop: full-width persistent navigation; mobile: floating compact navigation.
- Short unified animated mark and white/gold wordmark, with a skippable opening.
- Continuous scroll-scrub transitions and velocity impulses removed. Product/section reveal uses IntersectionObserver once per element.
- Product inspection remains readable and manually interactive without 3D scroll scrub.
- Product-specific hero backgrounds and flying-to-cart interaction retained.
- Respect reduced-motion settings.
- Validate on a mobile device and desktop before treating animation changes as final.
