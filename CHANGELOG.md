# Astoria Hospitality — Changelog

## 2026-04-03

### Performance
- Input font-size 14px -> 16px (prevents iOS auto-zoom on contact form)
- Google Fonts trimmed from 17 to 9 variants (~50KB savings)
- Added width/height to all img tags (prevents layout shift / CLS)
- Added `<meta name="theme-color">` for navy mobile browser chrome
- Added dns-prefetch for images.unsplash.com
- Removed cursor:none from form inputs (accessibility fix)

### Content
- Favicon: white A on navy background (.ico + 180px PNG)
- Social media links in footer now point to real accounts (Instagram, Facebook, LinkedIn)
- Le Gray moved to 3rd in carousel, Smallville to 5th (real photos shown early)

### Clients Carousel
- Expanded from 3 cards to all 21 hotel clients from old site
- Infinite horizontal carousel with mouse proximity speed control
- Center dead zone for comfortable hovering, edges accelerate scroll
- Mobile: auto-scroll + touch drag
- Real photos added: The Smallville Hotel Beirut, Le Gray Beirut (WebP, ~90KB each)

## 2026-04-02

### Products Page (NEW)
- `products.html` — editorial product showcase with 7 category sections
- Sticky category nav (Tableware | Glassware | Flatware | Buffet | Kitchen | Linen | Furniture)
- Scroll-spy highlights active section
- Alternating image/text layout per section
- Brand tags per category (which Astoria partners supply each)
- "Request [Category] Catalog" CTA per section
- Bottom CTA: "Can't Find What You're Looking For?"
- Full Arabic/English toggle
- Schema.org ItemList, Open Graph, SEO meta tags
- Logo gold particles (desktop only)

### Landing Page Updates
- Nav: "Services" renamed to "Products", links to products.html
- Hero CTA: "Explore Our Brands" renamed to "Explore Our Products"
- "What We Supply" cards now deep-link to products.html#category

## 2026-04-01

### Landing Page (NEW)
- `index.html` — single-page editorial luxury landing page
- Design: deep navy (#0D1B2A) + warm gold (#C8963E), Playfair Display + Outfit fonts
- 10 sections: nav, hero, trust bar, about, services, brands, projects, showroom CTA, contact, footer
- Three-tier gold particle system: logo (25) > H1 (18) > ambient (25)
- Ken Burns hero zoom, scroll-triggered reveal animations
- Infinite marquee trust bar with 12 hotel client names
- 25 brand partner grid with hover effects
- Contact form with dual-office info (Oman + Lebanon)
- Full Arabic/English toggle with RTL support (Noto Kufi Arabic)
- Schema.org (Organization + 2 LocalBusiness), Open Graph, SEO meta
- Custom gold cursor (desktop), mobile hamburger nav
- Responsive: desktop, tablet, mobile breakpoints
- GitHub Pages deployment via Actions workflow

### Documentation
- `01-audit-current-site.md` — 15 problems documented (P1-P15)
- `02-research-and-design.md` — market research, SEO strategy, design spec
- `03-products-page-spec.md` — products page specification
