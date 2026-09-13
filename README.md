# Savannah Food Guide

An interactive, single-page guide to forty hand-picked places to eat and drink in
Savannah, Georgia's Historic District — ten each for **Breakfast**, **Lunch**,
**Dinner** and **Drinks**.

**Live site:** https://stphnwlsh.github.io/savannah-food-guide/

## What's on each card

| | |
|---|---|
| **Rank & badge** | Position within its category; the top three are highlighted |
| **Style of food** | Cuisine descriptor (e.g. "Lowcountry fine dining", "South African sandwiches") |
| **Price** | `$`–`$$$$`, *relative to the other venues in this guide* — Budget, Moderate, Upscale, Splurge |
| **Reservations** | No reservations / Walk-in ok / Book ahead / Booking essential, plus a one-line note on how hard a table is to get |
| **Tags** | Practical flags such as Cash only, Rooftop, Dress code, Patio, Tasting menu |
| **Highlights** | What the place is known for |
| **Address** | Opens a Google Maps search for the venue |
| **Map** | An embedded Google map, expanded on demand (loaded lazily, so the page stays fast) |
| **Menu** | Opens a web search for the venue's current menu |

## Features

- Four filter tabs with smooth cross-fade and staggered card animation
- Responsive card grid — three-up on desktop, single column on mobile
- Light and dark themes, following the system preference and remembered per browser
- Deep links per category (`#breakfast`, `#lunch`, `#dinner`, `#drinks`)
- Keyboard-accessible tabs (arrow keys, Home/End) with correct ARIA roles
- Respects `prefers-reduced-motion`

## Tech

A single self-contained `index.html` — vanilla HTML, CSS and JavaScript, no build
step, no dependencies, no external scripts. The dataset lives in a `GUIDE` object
inline at the top of the page script; edit it there to change venues.

## Deployment

GitHub Pages, served from the root of the `main` branch:

1. **Settings → Pages**
2. **Source:** *Deploy from a branch*
3. **Branch:** `main`, folder `/ (root)` → **Save**

`.nojekyll` is present so the files are published as-is.

## A note on the data

Venue names, addresses and highlights come from the curated source list. The
price tier and reservation guidance are editorial judgements — price is relative
to the rest of this guide rather than to restaurants nationally, and booking
policies change. Call ahead for the ones that matter.
