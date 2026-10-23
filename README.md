# NOIRGRILL — Scroll-Assembled Burger Experience

A premium, dark, cinematic one-page website for a gourmet burger house. The hero is a **scroll-driven burger assembly**: as the visitor scrolls, a tall sticky stage stacks a burger layer by layer — bottom bun, smashed patty, melted cheese, tomato, lettuce, top bun — each layer gliding into place with its own caption. It delivers a "3D product" feel with zero 3D libraries, so it loads fast and runs anywhere.

## What's inside

- **Scroll-assembled burger hero** — 600vh scroll runway, sticky stage, six layers sliced from one hero photograph so they align perfectly, scroll-scrubbed transforms, per-layer captions, layer checklist, and a completion state ("Six layers. Zero shortcuts.") with order CTAs.
- **Menu** — 8 burgers with photos, descriptions, prices, and Add-to-Order buttons.
- **Working order cart** — slide-in drawer, quantity controls, itemised totals, demo checkout with order confirmation.
- **Our Story section** — brand narrative with photography.
- **Reservation / order-ahead form** — validated in the browser (name, phone, date, time, guests) with a success confirmation.
- **Visit section** — hours, address, phone.
- Fully responsive, vanilla HTML/CSS/JS in a single `index.html` — no build step, no dependencies.

## How a buyer customises it

1. **Name & branding** — search `index.html` for `NOIRGRILL` and swap in the restaurant name; change the accent colour via the `--amber` CSS variable at the top of the `<style>` block.
2. **Menu & prices** — menu items are plain HTML cards in the `#menu` section; edit names, descriptions and prices directly. Cart logic reads the price from each card automatically.
3. **Photos** — replace any file in `images/` keeping the same filename. `images/burger-hero.jpg` powers the assembly animation — use a straight-on, centred burger photo (dark background works best) and keep it at least 1000px wide.
4. **Hours / address / phone** — edit the Visit section and footer text.
5. **Form** — the reservation form is a front-end demo (shows a confirmation). Connect it to a real inbox by pointing the form at a service like Formspree, or wire the `reserveForm` submit handler in the script to your own API.

## Files

- `index.html` — the entire site (styles + scripts embedded)
- `images/` — all photography (Unsplash)
- `README.md` — this file

Open `index.html` in any browser, or drop the folder on Netlify / Vercel / GitHub Pages to go live.
