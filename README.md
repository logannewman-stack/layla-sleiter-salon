# Layla Sleiter Salon Studio â Website

A refined, professional marketing website for **Layla Sleiter Salon Studio**, a
full-service hair and nail salon in **Des Moines, Iowa** specializing in hair
extensions, color & balayage, precision cuts, manicures, and pedicures.

Design language: a warm, editorial **cream / white / black** palette, elegant
serif display type (Cormorant Garamond) paired with a clean sans (Jost), and
soft scroll-reveal motion throughout. Built for a polished desktop experience
and fully responsive down to mobile.

## Tech stack

- **React + Vite + TypeScript** â fast, typed SPA
- **Tailwind CSS** â custom warm-neutral luxury design system
- **Framer Motion** â scroll reveals, sticky nav, animated booking modal

## Sections

- **Hero** â headline, rating/trust row, and a featured photo slot
- **Marquee** â scrolling strip of specialties
- **Services** â six service cards (extensions, color, cuts, manicures, pedicures, packages)
- **About Layla** â owner story + key stats
- **Gallery** â editorial photo grid
- **Pricing** â service & price menu
- **Reviews** â client testimonials
- **Booking** â hours, location, contact + a booking form modal (opens the guest's
  email pre-filled to the salon â no backend required)

## Editing content

All business details, services, pricing, hours, testimonials, and image paths
live in one file:

```
src/data/salon.ts
```

Change the phone number, address, prices, or copy there and it updates
everywhere.

## Swapping in your own photos

Every image is a slot backed by an on-brand placeholder frame in
`public/images/` (`hero.svg`, `portrait.svg`, `extensions.svg`, `color.svg`,
`haircut.svg`, `nails.svg`, `pedicure.svg`, `interior.svg`).

To use your own photo, either:

1. Drop your image into `public/images/` and point the matching key in the
   `images` object in `src/data/salon.ts` at it (e.g. `hero: '/images/hero.jpg'`), or
2. Replace the placeholder file directly and keep the path.

Portrait-oriented photos (4:5) work best for `hero` and `portrait`; landscape
(16:9) for `interior`; roughly square for `nails` and `pedicure`.

## Develop

```bash
npm install
npm run dev      # start dev server
npm run build    # type-check + production build
npm run preview  # preview the production build
```
