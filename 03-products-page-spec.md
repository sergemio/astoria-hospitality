# Astoria Hospitality — Products Page Spec
**Date:** 2026-04-02
**Type:** New page — editorial product showcase
**Tech:** Static HTML/CSS/JS, same stack as landing page
**URL:** `/products.html` (linked from header nav)

---

## Problem

The current Astoria site has a "Products" dropdown with 7 categories (Tableware, Glassware, Flatware, Buffet Items, Kitchen Equipment, Linen & Amenities, Furniture & Lighting). Each leads to a page with random product photos, no descriptions, no brand info, nothing actionable. A procurement director can't understand what Astoria actually offers or why it's premium.

## Solution

One beautiful long-scroll page — an editorial product showcase. Each of the 7 categories gets its own section with styled imagery (Gemini-generated), editorial copy, brand associations, and a CTA. A sticky category nav at the top lets visitors jump to any section instantly.

Think: luxury lookbook, not product catalog.

---

## Entry Points

1. **Header nav: "Products"** — replaces/renames current "Services" link in the main nav on both the landing page and products page
2. **Landing page "What We Supply" cards** — each card deep-links to the corresponding anchor (e.g., `/products.html#flatware`)
3. **Landing page hero CTA** — "Explore Our Products" (rename from "Explore Our Brands")

## Page Structure

### 1. Hero Section
- Compact hero (50-60vh, not full viewport)
- Background: Gemini-generated image — an overhead shot of a beautifully set hotel dining table
- Dark overlay + centered text:
  - Gold label: "OUR PRODUCTS"
  - H1: "Curated for the World's Finest Hotels"
  - Subline: "Discover our full range of premium hospitality products, from tableware to turnkey solutions"
- No CTA buttons here — the sticky nav below does the job
- Same navy + gold palette, Playfair Display + Outfit fonts

### 2. Sticky Category Nav
- Horizontal bar that sticks below the main header nav on scroll
- Background: dark navy with subtle gold bottom border (same feel as main nav)
- 7 category pills/links in a row:
  - Tableware | Glassware | Flatware | Buffet & Banquet | Kitchen Equipment | Linen & Amenities | Furniture & Lighting
- Active section highlighted with gold underline (scroll-spy behavior)
- Smooth scroll on click
- Horizontally scrollable on mobile (with subtle scroll indicator)
- Becomes sticky after scrolling past the hero

### 3. Seven Category Sections

Each section follows the same template but with unique content:

```
[Full-width image — Gemini-generated, editorial quality]

[Gold label: category number — "01"]
[H2: Category Name]
[Editorial paragraph: 2-3 sentences about what Astoria offers in this category, the quality level, the use cases]

[Brands strip: "Brands we carry" → logo-style text list of partner brands for this category]

[CTA: "Request [Category] Catalog" — gold outline button]
```

#### Layout Options (alternating for visual rhythm):
- **Odd sections (1, 3, 5, 7):** Image left (60%), text right (40%)
- **Even sections (2, 4, 6):** Text left (40%), image right (60%)
- On mobile: always image on top, text below

#### The 7 Sections:

**01 — Tableware**
- Description: Fine china, porcelain, and ceramic collections from the world's premier manufacturers. From classic white bone china to contemporary textured designs.
- Brands: Churchill, Costa Nova, Dudson, Saturnia, By Bone, Fortessa
- Image: Elegant stacked plates, bowls, serving pieces on a dark surface

**02 — Glassware**
- Description: Crystal and glass collections for every occasion — from delicate wine stems to sturdy everyday tumblers. Precision-crafted for durability and elegance.
- Brands: Schott Zwiesel, Utopia, Topkapi
- Image: Wine glasses, champagne flutes, tumblers catching light

**03 — Flatware**
- Description: Cutlery that elevates every place setting. Stainless steel, silver-plated, and gold-finished collections in modern and classical designs.
- Brands: Cutipol, Fortessa, Kapp
- Image: Flatware sets laid out on linen, mix of silver and gold finishes

**04 — Buffet & Banquet**
- Description: Statement pieces for grand buffets and banquet halls. Chafing dishes, display risers, serving stations, and presentation equipment built for volume and visual impact.
- Brands: Intermetal, Lava, Onon
- Image: Dramatic buffet setup with chafing dishes, tiered displays

**05 — Kitchen Equipment**
- Description: Professional-grade commercial kitchen equipment. Prep stations, cooking equipment, refrigeration, and back-of-house essentials from industry-leading manufacturers.
- Brands: Kapp, Yetkin, Ormel
- Image: Clean commercial kitchen, stainless steel surfaces

**06 — Linen & Amenities**
- Description: Premium textiles and guest amenities that define the guest experience. Table linen, bed linen, towels, bathrobes, and in-room amenity collections.
- Brands: Bedtex, Libanfibre, Berfa
- Image: Folded white linens, towels, amenity sets on marble surface

**07 — Furniture & Lighting**
- Description: Bespoke hospitality furniture and atmospheric lighting solutions. Dining chairs, lounge seating, tables, and decorative lighting designed for commercial durability.
- Brands: HNI, Guren, Face
- Image: Hotel restaurant interior with elegant chairs, pendant lighting

### 4. Bottom CTA Section
- Full-width, similar to the showroom CTA on the landing page
- "Can't Find What You're Looking For?"
- "Our team can source any hospitality product from our network of 25+ international brands. Let's talk."
- Two CTAs: "Request a Custom Consultation" | "Visit Our Showroom"

### 5. Footer
- Same footer as landing page (shared component)

---

## Design Details

### Visual Treatment per Section
- Images: Gemini-generated initially, replaced with real showroom/product photos later
- Each image has a subtle gold frame/border treatment on desktop (like the about section on the landing page)
- Scroll-triggered reveal animations (same IntersectionObserver system as landing page)
- Section numbers ("01", "02"...) displayed large and semi-transparent as a decorative element (behind the heading, gold at 10% opacity, oversized Playfair Display)

### Sticky Nav Behavior
- Below main nav (combined height: ~140px when both stuck)
- Background: `var(--bg-secondary)` with `backdrop-filter: blur(20px)`
- Active pill: gold text + gold underline (2px)
- Inactive pills: `var(--text-secondary)`, gold on hover
- Scroll-spy: IntersectionObserver on each section, updates active pill
- Mobile: horizontal scroll with `overflow-x: auto`, hide scrollbar, subtle fade on edges

### Color Palette
- Same as landing page — no new colors
- Section backgrounds alternate: `--bg-primary` / `--bg-secondary` for rhythm

### Typography
- Same Playfair Display + Outfit as landing page
- Section numbers: Playfair Display, 120px, gold at 10% opacity, positioned absolute behind heading
- H2: Playfair Display, clamp(32px, 5vw, 48px)
- Body: Outfit, 17px, `--text-secondary`, line-height 1.8
- Brand names: Outfit, 14px, uppercase, letter-spacing 2px, `--text-muted`

### Responsive
- Desktop (1200px+): alternating image/text split (60/40)
- Tablet (768-1199px): same but 55/45 split
- Mobile (<768px): stacked — image full-width on top, text below
- Sticky category nav: scrollable horizontal pills on mobile

### Arabic Support
- Same i18n system as landing page — `data-i18n` attributes + `lang/` translations
- RTL: image/text split mirrors, sticky nav direction flips
- Category names translated

### SEO
- Meta title: "Hotel & Restaurant Supplies | Astoria Hospitality — Oman & Lebanon"
- Meta description: "Explore our curated range of premium hospitality products: tableware, glassware, flatware, kitchen equipment and more. 25+ international brands. Showrooms in Muscat and Beirut."
- H1: "Curated for the World's Finest Hotels"
- Each H2: category name (keyword-rich)
- Schema.org: `ItemList` with 7 `ListItem` entries
- Alt tags on all images with category + brand keywords

### Performance
- Same targets as landing page (<2.5s LCP)
- Images: lazy-loaded, WebP via Gemini or Unsplash
- Shared CSS: consider extracting common styles into a shared file (or keep inline for simplicity in v1)

---

## Changes to Existing Landing Page

1. **Header nav:** Rename "Services" → "Products", link to `/products.html`
2. **Hero CTA:** Rename "Explore Our Brands" → "Explore Our Products", link to `/products.html`
3. **"What We Supply" cards:** Each card links to `/products.html#[category-id]`
4. **Mobile nav:** Update link text accordingly

---

## Implementation Notes

- Single HTML file: `products.html` in the repo root
- Reuse CSS patterns from `index.html` (consider shared styles later)
- Shared nav and footer markup (copy for now, componentize in Phase 2)
- Gemini images generated first, swapped for real photos when Elissar provides them
- Arabic translations added to the same i18n system

---

*Ref: Addresses problems P5 (SEO), P6 (no case studies/detail), P8 (partners underused), P10 (no CTAs), P14 (no product detail) from 01-audit-current-site.md*
