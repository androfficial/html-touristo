# Touristo

Landing page for Touristo, a travel agency, with an advanced tour search, a filterable catalog of discounted tours and sliders. The site is in Ukrainian. Built in July 2021 as a learning project.

**Live demo:** [androfficial.github.io/touristo](https://androfficial.github.io/touristo/)

## Features

- The advanced search button slides open extra search fields (jQuery): a date range picker (Air Datepicker), a trip duration range slider from 2 to 120 days (noUiSlider) and a travellers dropdown with plus and minus counters for adults and children.
- Country and tour type buttons filter the catalog of discounted tours with animated MixItUp transitions; hovering a tour card animates the borders of its labels.
- The newsletter form checks the email format and empty fields when a field loses focus and marks invalid fields with a red border and a hint. On touch screens below 992 px, two tabs switch between email and SMS sign-up.
- Swiper sliders: special offers with clickable dots, and traveller reviews with three, two or one review per view, arrows and dots.
- The fixed header shrinks after 120 px of scrolling on screens wider than 1024 px, and a burger button opens the menu at 992 px and below.
- On touch phones narrower than 481 px, the footer link groups collapse into accordions with a height animation.

## Tech stack

- **Framework:** none, plain HTML and JavaScript
- **UI:** jQuery 3, Swiper 6, MixItUp 3
- **Styling:** SCSS compiled to CSS (the SCSS sources are not in the repository)
- **Forms:** Air Datepicker 2, noUiSlider
- **Tooling:** built with Gulp 4, which produced the plain and minified bundles in `css/` and `js/`
- **Hosting:** GitHub Pages

## Getting started

The repository holds the compiled site, with no dependencies and no build step. The icons come from an external SVG sprite that browsers do not load from `file://`, so serve the folder over HTTP, for example with `npx serve .` on Node.js 18 or later.

```bash
git clone https://github.com/androfficial/touristo.git
cd touristo
npx serve .
```

Then open the local address that `serve` prints.

## Notes

- The search and newsletter forms send nothing, and the catalog links and "add to comparison" buttons have no targets.
