<div align="center">

**English** · [العربية](README.ar.md)

<a href="https://naturaloli-preview.onrender.com/"><img src="https://img.shields.io/badge/Live_site-naturaloli--preview.onrender.com-1B2340?style=for-the-badge" alt="Open the live site"></a>

</div>

<img src="assets/showcase.jpg" width="100%" alt="The Arabic home page on desktop and on a phone: a bottle of OLI olive oil in a stone arch, an olive sprig hanging beside it, the headline and a store button">

This is the new website for OLI (اولي), a Saudi brand that sells Italian extra virgin olive oil. The main page is in Arabic and there is a full English version at `/en`. It is for shoppers in Saudi Arabia, and every product card links to that product in the brand's online store.

Designed and built by **Mohammed Altounsi** · [LinkedIn](https://www.linkedin.com/in/mohammed-altounsi/)

The preview runs on Render's free tier, so the first visit after a quiet spell can take about a minute to load.

## Scrolling through the site

<img src="assets/scroll.gif" width="100%" alt="Screen recording of the Arabic page: the olive sprig sways in the hero, then the page scrolls past the About section and the first line drawings of how the oil is made">

## What's on the site

From top to bottom, on both the Arabic and English pages:

- **Hero.** A product photo inside a stone arch. Arrows (or a swipe) step through the range, and a button goes to the store. The olive sprig sways and moves with the pointer.
- **About.** Who the brand is and why it sources from Italy, with photos of the bottles.
- **Services.** Accordion rows, each with its own photo. On phones the photo opens under the row's title.
- **Products.** One card per product, stacking as you scroll. A card holds the description, tags and a link to order that product from the store.
- **Testimonials, FAQs and Contact.** The contact form sends to the brand's inbox.

Between the sections there are line drawings of how the oil is made: harvest, leaf removal and washing, crushing, malaxing, decanting, settling and bottling. Each drawing appears as you reach it. An olive drops out of the hero and falls down the page, lands on the edges of photos and cards, rolls off, and goes into each machine. The crusher turns it into paste and the decanter turns it into a drop of oil.

## How it's built

- Static HTML, CSS and JavaScript with no build step.
- The page layout started from a Framer export. Framer's runtime and assets are saved with the site, so it does not load anything from Framer.
- The hero, the olive's journey, the stacking product cards and the phone version of the services section are custom code in plain JavaScript and CSS, loaded on top of the exported pages. A small loader swaps Framer's original banner for the custom hero.
- One stylesheet recolours the Framer sections to the hero's palette of limestone, gold and navy.
- The hero and the journey check the visitor's reduced-motion setting.
- The contact form posts to a small PHP endpoint that rate-limits by IP and only accepts posts from the brand's domain.

## Screenshots

<table>
  <tr>
    <td width="50%"><img src="assets/desktop-en.jpg" alt="English home page at /en: the headline on the left and the bottle in the arch on the right"></td>
    <td width="50%"><img src="assets/journey.jpg" alt="Arabic page between sections: four figures about the oil above a line drawing of the leaf removal and washing step"></td>
  </tr>
  <tr>
    <td colspan="2"><img src="assets/products.jpg" alt="Products section: a card for the 750 ml bottle with its description, tags, a link to the store and a customer review"></td>
  </tr>
</table>

---

> This repo shows the design and front end of the site. The source code is private. If you want a website like this, message me on [LinkedIn](https://www.linkedin.com/in/mohammed-altounsi/).
