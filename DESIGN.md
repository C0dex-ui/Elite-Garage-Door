---
version: alpha
name: EliteGarageDoor
description: Industrial-warm Slidell garage-door homepage from user pack v3 layout, scrape facts only.
colors:
  primary: "#2B2B2B"
  secondary: "#7A7D80"
  tertiary: "#B84A1F"
  ink: "#0C1218"
  paper: "#F4EFE6"
  white: "#FBF8F3"
  muted: "#6A7380"
  line: "#E2D8C8"
  on-primary: "#FBF8F3"
  on-tertiary: "#FFFFFF"
typography:
  h1:
    fontFamily: Big Shoulders Display
    fontSize: 5.25rem
    fontWeight: 600
    lineHeight: 0.95
    letterSpacing: -0.02em
  h2:
    fontFamily: Big Shoulders Display
    fontSize: 3.25rem
    fontWeight: 600
    lineHeight: 0.95
    letterSpacing: -0.02em
  body-md:
    fontFamily: Libre Franklin
    fontSize: 1.0625rem
    fontWeight: 400
    lineHeight: 1.6
  label-caps:
    fontFamily: Libre Franklin
    fontSize: 0.6875rem
    fontWeight: 800
    letterSpacing: 0.22em
rounded:
  sm: 2px
  md: 2px
spacing:
  sm: 8px
  md: 16px
  lg: 32px
  xl: 88px
motion:
  duration: 550ms
  easing: cubic-bezier(0.22, 1, 0.36, 1)
  stagger: 80ms
components:
  button-primary:
    backgroundColor: "{colors.tertiary}"
    textColor: "{colors.on-tertiary}"
    rounded: "{rounded.sm}"
    padding: 14px
  button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.sm}"
    padding: 14px
---

## Overview

Warm industrial shop page for a Slidell residential garage-door crew. Pack v3 supplies the fold (ink header, full-bleed door still, paper booking ticket) and rust accent. Facts stay in `_scrape.json`. Uniqueness: **Big Shoulders Display + Libre Franklin, full-bleed residential door still with type left and a right paper booking ticket, photo-rail service slabs, 2px rust ticket edge.** Not ACE lower-left floating paper card / masonry. Not ACE dusk veil. Not Precision twin-gutter / measurement rows. Not ProLift half-open bay / door-panel stalls. Not Growfully period-stopped declaratives. Not our concrete 50/50 industrial still. Style: **Craftsmanship** (Pro Max search skipped — Python unavailable; Industrial Utility is ACE). Pattern: **Local Booking Ticket** — call path on the fold, services, then call again.

## Colors

Sampled from `logo.png` (graphite `#2B2B2B`, steel `#7A7D80`) plus pack v3 rust `#B84A1F` as the one high-chroma (also in the hero brick). Paper `#F4EFE6` / `#FBF8F3`. Ink `#0C1218`. **No brass / gold / yellow.** Rust does three jobs only: primary CTA, eyebrows, booking-ticket top bar.

## Typography

Big Shoulders Display for H1/H2/H3 — condensed poster, **negative tracking**. Libre Franklin for body, nav, chips. One italic pull in Libre Franklin italic — not Fraunces (Johntilly).

## Layout

- Hero pattern: full-bleed `assets/hero.jpg` (pack `install.jpg` — residential raised-panel door). Type column left, paper booking ticket right. Not a pool house; pack `hero.jpg` / `house.jpg` unused (off-niche).
- Photography: hero door still + springs still + repair still. Pack-sourced. `"photos": "mixed"`.
- Section rhythm: ink / paper / ink / paper. Padding ~88px desktop, ~56px mobile. No drawn brass rules.
- Card model: 2×2 photo-rail slabs — 168px cover still left, copy right.
- IA: Header → Hero → Trust → Services → About → Gallery → CTA → Areas → Reviews → FAQ → Contact → Footer. Reviews use only scrape quotes.

## Elevation & Depth

Quiet grain wash on paper bands. Ticket has a 4px rust top edge. Cards: paper fill + soft shadow, media flush left. Motion 400–700ms once, one soft float on the ticket, card hover lift. `prefers-reduced-motion: reduce` kills motion. No GSAP, no Lottie, no WebGL.

## Shapes

2px on buttons and ticket. 0px on stills. Hairline `#E2D8C8` on paper cards. No 99px pills except chips.

## Components

Header: mark + wordmark + call. Hero facts: H1 keyword, lede, two CTAs (Call + Request Estimate), ticket with phone. Service card: photo-rail. Review: Trustindex-style 3-up card grid (header + **Write a review** + equal cards + carousel), scrape quotes only, no Google rating or review count. Write a review opens Nextdoor. Form: **Submit** (`type="submit"`), confirms on-page, does not send. Footer + mobile call dock.

CTA lock (do not revert): Call = shop line; Request Estimate = `#contact`; form button = Submit; reviews header = Write a review.

## Do's and Don'ts

- Do use scrape NAP: 657 Whitney Dr, Slidell, LA 70461 · (985) 639-9748.
- Do keep H1 **Garage Door Repair in Slidell**.
- Don't print hours, (985) 261-2437, 2008, Angi/Yelp scores, Northshore cities, Clopay, LiftMaster, brass gold.
- Don't ship pack `hero.jpg` (pool) or `house.jpg` (no door) as the fold.
