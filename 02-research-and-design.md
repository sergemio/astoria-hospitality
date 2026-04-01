# Astoria Hospitality — Research, SEO Strategy & Design Spec
**Date:** 2026-04-01  
**Project:** Full website redesign (landing page first, then multi-page)  
**Tech stack:** Static site — HTML/CSS/JS, GitHub Pages  
**Language:** English primary, Arabic toggle (i18n-ready from day 1)

---

## Part 1: Market Research

### 1.1 What Astoria Does

Astoria Hospitality is a B2B hospitality supply & consulting company based in **Oman (Muscat)** and **Lebanon (Beirut)**. They supply hotels and restaurants across Arab/Gulf markets with premium international products:

- Tableware, Glassware, Flatware
- Buffet Items, Kitchen Equipment
- Linen & Amenities
- Furniture & Lighting
- Hospitality consulting

**Business model:** Inquiry-based (not e-commerce). Showrooms for viewing. Catalogs sent on request. Clients come primarily through word-of-mouth and reputation.

**Key differentiators:**
- 25 premium international brand partnerships (Churchill, Fortessa, Schott, Cutipol, Costa Nova, Dudson, Saturnia…)
- 21+ major hotel clients (Four Seasons, Kempinski, InterContinental, Radisson, Rotana, Wyndham, DoubleTree, Movenpick…)
- Dual-market presence (Oman + Lebanon)
- CEO Elissar Maalouf — hands-on leadership

### 1.2 MENA Hospitality Market

- **Market size:** $310 billion (2025) → projected $487 billion by 2032
- **Growth drivers:** Gulf tourism expansion (Saudi Vision 2030, Oman tourism push), new hotel developments, luxury segment growth
- **Supply chain:** Hotels rely on specialized OS&E (Operating Supplies & Equipment) suppliers for everything from tableware to furniture
- **Key trade events:** HORECA Oman, The Hotel Show Dubai, HORECA Lebanon

### 1.3 Competitive Landscape

#### Direct Competitors (Oman/Lebanon/Gulf)

| Company | Location | Since | Strengths | Weaknesses | Website Quality |
|---|---|---|---|---|---|
| **HSI International** | Oman + UAE | 2000 | OS&E specialist, multi-country, clear categories | No content, no SEO, outdated design, empty video section | Poor |
| **Arcus Hospitality** | Oman | 2017 | Swiss JV (credibility), Royal Hospitality Qatar partnership | Small, limited web presence | Basic |
| **Synergy Business** | Oman | — | World-renowned brands, new hotel projects | Generic site | Basic |
| **Danube Hospitality** | UAE/Gulf-wide | — | Regional scale, full product range, multi-country | Site blocks scraping (403), generic feel | Unknown |
| **GM Hotel Supplies** | Region | — | Multi-country | Outdated website | Poor |

#### International Best-in-Class (Design/SEO Reference)

| Company | What They Do Right |
|---|---|
| **Front of the House** (USA) | Collections by mood/aesthetic, downloadable catalogs (40+ PDFs), sustainability messaging, blog for SEO, BOGO promotions, distributor network |
| **Renarte** (UAE) | Luxury visual approach, full-viewport hero, Montserrat/Karla typography, dual CTAs, clean dark palette, 18 years credibility |
| **Everstyle** (UAE, 30+ yrs) | "Former hoteliers" credibility angle, B2B + retail split, regional offices display, brand-forward (Costa Nova, Serax, Riedel) |

#### Key Competitive Insight

**Almost no competitor in the Oman/Lebanon HORECA supply market has a well-built website or SEO strategy.** HSI (25 years in business) has zero content. Arcus is minimal. The bar is extremely low. Whoever builds real content and SEO first captures regional search traffic. This is Astoria's window.

### 1.4 Best Practices Extracted

From analyzing 8+ competitor/reference sites:

1. **Hero = credibility in 5 seconds** — name, what you do, who you serve, one stunning visual
2. **Client logos > everything** — hotels trust other hotels. Show the portfolio prominently
3. **Brand partners = authority** — "authorized distributor of Churchill/Fortessa" is a trust signal
4. **Collections by category/mood** — not product catalogs, but curated visual groupings
5. **Showroom/consultation CTA** — B2B hospitality is relationship-driven, drive physical meetings
6. **Regional presence** — show offices/showrooms on a map, multi-country = scale signal
7. **Project showcases** — "We supplied X for Four Seasons Muscat" = SEO + social proof goldmine
8. **Downloadable resources** — catalogs, lookbooks = lead capture mechanism
9. **Clean, dark, luxury palette** — navy/black + gold/copper is the industry standard
10. **Mobile-first** — procurement managers browse on tablets during site visits

---

## Part 2: SEO Strategy

### 2.1 Target Keywords

#### Primary (high intent, medium competition)
| Keyword | Target Page |
|---|---|
| `hospitality supplier Oman` | Homepage |
| `hotel supplier Oman` | Homepage |
| `hotel equipment supplier Muscat` | Homepage |
| `HORECA supplier Middle East` | Homepage / About |
| `hotel supplier Lebanon` | Homepage |
| `restaurant supplies Oman` | Homepage |

#### Secondary (category-specific)
| Keyword | Target Page |
|---|---|
| `hotel tableware supplier Oman` | Services/Tableware |
| `commercial kitchen equipment Oman` | Services/Kitchen |
| `hotel linen supplier Middle East` | Services/Linen |
| `buffet equipment supplier Gulf` | Services/Buffet |
| `hotel amenities supplier Oman` | Services/Amenities |
| `hotel furniture supplier Muscat` | Services/Furniture |

#### Long-tail (content/blog opportunities)
| Keyword | Content Type |
|---|---|
| `how to choose tableware for 5-star hotel` | Blog article |
| `best hotel amenities brands 2026` | Blog article |
| `hotel OS&E supplier Oman` | About / Services |
| `luxury hotel supplies Middle East` | Homepage |
| `hotel opening supplies checklist` | Blog / Lead magnet |
| `Churchill tableware distributor Oman` | Brand partner page |
| `Fortessa flatware supplier Gulf` | Brand partner page |

#### Brand-Specific (each partner = SEO page)
Every brand partnership is a keyword opportunity:
- `Churchill china supplier Oman`
- `Cutipol flatware Middle East`
- `Schott Zwiesel glassware Oman`
- `Costa Nova tableware Gulf`
- etc.

### 2.2 Technical SEO Requirements

| Element | Implementation |
|---|---|
| **Meta titles** | Unique per page, keyword-optimized, <60 chars |
| **Meta descriptions** | Unique per page, CTA-driven, <155 chars |
| **H1 hierarchy** | One H1 per page with primary keyword |
| **Schema.org** | `Organization`, `LocalBusiness` (x2: Oman + Lebanon), `BreadcrumbList` |
| **Open Graph** | Title, description, image for every page |
| **Sitemap.xml** | Auto-generated, submitted to GSC |
| **robots.txt** | Standard, allow all |
| **Canonical URLs** | Self-referencing on every page |
| **hreflang** | `en` + `ar` when Arabic is added |
| **Page speed** | Target <2s load, optimized images (WebP), minimal JS |
| **Mobile-first** | Responsive, touch-friendly CTAs, readable on tablets |
| **HTTPS** | GitHub Pages default |
| **Internal linking** | Every page links to related services + contact |

### 2.3 Content Strategy (Post-Launch)

**Phase 1 — Launch content (built into site):**
- Homepage with keyword-rich copy
- About page with company story + team
- 7 service category pages (one per product line)
- Brand partners overview + individual brand pages (top 10 first)
- Client portfolio with project descriptions
- Contact page (Oman + Lebanon)

**Phase 2 — Blog / ongoing (1-2 posts/month):**
- Hotel opening guides
- Product spotlights (brand features)
- Project case studies
- Industry trend pieces
- "Best of" lists (e.g., "Best Tableware Brands for Luxury Hotels")

**Phase 3 — Backlink strategy:**
- Get listed on Hotelier Middle East supplier directory
- HORECA Oman trade show presence → backlinks
- LinkedIn articles from Elissar → links to site
- Brand partner websites → "find a distributor" backlinks

### 2.4 Google Business Profile

- **Create/claim** GBP for both locations (Muscat + Beirut)
- Category: "Hospitality supply service" / "Restaurant supply store"
- Photos of showrooms, products, team
- Regular posts (monthly)
- Collect reviews from hotel clients

---

## Part 3: Landing Page Design Spec

### 3.1 Overview

A single-page, scroll-based landing page that serves as the new homepage. Designed to:
1. Establish credibility in 5 seconds
2. Showcase brand partners and hotel clients
3. Drive two conversions: "Request a Catalog" + "Visit Our Showroom"
4. Rank for primary keywords
5. Be expandable into a full multi-page site

### 3.2 Color Palette

Based on current Astoria branding (keep + refine):

| Role | Color | Hex (approx) | Notes |
|---|---|---|---|
| Primary background | Deep navy | `#0D1B2A` | Slightly darker than current, richer |
| Secondary background | Darker navy | `#070F1A` | For alternating sections |
| Accent | Warm gold | `#C8963E` | Unified gold (current has inconsistent shades) |
| Accent hover | Light gold | `#D4A94E` | Hover states |
| Text primary | White | `#FFFFFF` | Main text on dark backgrounds |
| Text secondary | Soft white | `#B8C4D0` | Subtitles, descriptions |
| Text accent | Gold | `#C8963E` | Links, highlights |
| Subtle borders | Gold 20% | `rgba(200,150,62,0.2)` | Dividers, card borders |
| CTA button | Gold fill | `#C8963E` | Primary actions |
| CTA secondary | Gold outline | `transparent + #C8963E border` | Secondary actions |

**No purple.** Let navy dominate. Gold for all accents.

### 3.3 Typography

| Element | Font | Weight | Size (desktop) |
|---|---|---|---|
| Logo / brand | Keep existing Astoria font | — | — |
| Headings | Montserrat or Cormorant Garamond | 500-700 | 48-64px hero, 32-40px sections |
| Subheadings | Montserrat | 400-500 | 18-24px |
| Body | Inter or Karla | 400 | 16-18px |
| Buttons | Montserrat | 600 | 14-16px, uppercase, tracked |

**Rationale:** Montserrat = modern luxury (used by Renarte). Cormorant Garamond = elegant serif option that pairs with Astoria's brand. Inter = clean body text.

### 3.4 Page Sections (Scroll Order)

#### Section 1: Navigation Bar (Sticky)
- Astoria logo (left)
- Nav links: About | Services | Partners | Clients | Contact (center/right)
- Language toggle: EN | AR (right)
- "Request a Catalog" CTA button (right, gold)
- Dark navy background, subtle gold border-bottom
- Hamburger menu on mobile

#### Section 2: Hero
- Full-viewport height (100vh)
- Background: stunning hospitality image (elegant table setting / hotel dining room) — generate via Gemini initially
- Dark overlay gradient (left to right or bottom to top)
- Left-aligned content:
  - Logo mark (smaller, above text)
  - **H1:** "Premium Hotel & Restaurant Supplies"
  - **Subline:** "Equipping the finest hotels across the Gulf — from tableware to turnkey solutions"
  - **Keywords baked in:** "hotel", "restaurant", "supplies", "Gulf"
  - Two CTAs: "Explore Our Brands" (gold fill) | "Request a Catalog" (gold outline)
- Bottom: subtle scroll indicator arrow
- **SEO:** H1 with primary keyword, meta title: "Astoria Hospitality | Hotel & Restaurant Supplier in Oman & Lebanon"

#### Section 3: Trust Bar
- Single horizontal strip
- "Trusted by 3,460+ clients across the Gulf"
- Immediately followed by 6-8 top hotel client logos (Four Seasons, Kempinski, InterContinental, Radisson, Rotana, Hilton brand) in a row, white/light versions
- Subtle auto-scroll animation
- **Purpose:** Instant credibility. This is the most important conversion element.

#### Section 4: Who We Are (Brief)
- **H2:** "Your Hospitality Partner Since [year]"
- 2-3 sentences max: what Astoria does, where they operate, why hotels trust them
- Key stats in 3 columns:
  - "25+ Premium Brands"
  - "Oman & Lebanon"
  - "3,460+ Clients Served"
- "Learn More About Us" text link → future About page
- **SEO:** keywords "hospitality supplier Oman", "hotel equipment Lebanon"

#### Section 5: What We Supply (Services Grid)
- **H2:** "Everything Your Hotel Needs"
- 6-7 cards in a responsive grid (3 columns desktop, 2 tablet, 1 mobile):
  - Tableware
  - Glassware
  - Flatware
  - Buffet & Banquet
  - Kitchen Equipment
  - Linen & Amenities
  - Furniture & Lighting
- Each card: icon or image + category name + 1-line description
- Gold border on hover
- Each card links to future service page (or scrolls to contact for now)
- **SEO:** category keywords as H3s

#### Section 6: Our Brands (Partner Showcase)
- **H2:** "Representing the World's Finest Brands"
- Logo grid: all 25 brand partners, organized cleanly
- Logos in white/light versions on dark background
- Subtle hover effect (gold glow or slight scale)
- Subtext: "Authorized distributor of leading international hospitality brands"
- CTA: "View Our Brand Portfolio" → future partners page
- **SEO:** "authorized distributor", brand names in alt tags

#### Section 7: Featured Projects / Social Proof
- **H2:** "Trusted by the Region's Leading Hotels"
- 3-4 featured project cards:
  - Hotel name + logo
  - 1-line scope ("Full tableware & glassware supply")
  - Elegant image of the setup
- Or: testimonial quotes from hotel clients if available
- CTA: "See All Projects" → future portfolio page
- **SEO:** hotel names + "supplier" as long-tail keywords

#### Section 8: Showroom CTA
- Full-width section with background image (showroom or elegant product display)
- Dark overlay
- **H2:** "Experience Our Collections in Person"
- Subtext: "Visit our showrooms in Muscat and Beirut"
- Two CTAs: "Book a Showroom Visit" | "Request a Catalog"
- **Purpose:** Primary conversion section. This is where word-of-mouth leads come to take action.

#### Section 9: Contact / Locations
- **H2:** "Get in Touch"
- Two-column layout:
  - **Oman office:** Address, phone (+968 99326424, +968 24137733), email (elissarmaalouf@astoriahosp.com)
  - **Lebanon office:** Address, phone (+961 3078727, +961 70310123), email (aliaojeil@astoriahosp.com)
- Simple contact form: Name, Company, Email, Phone, Message
- Social media icons: Instagram, Facebook, LinkedIn
- **SEO:** `LocalBusiness` schema for both locations

#### Section 10: Footer
- Astoria logo
- Quick links: About | Services | Partners | Clients | Contact
- Social media links
- "OMAN | LEBANON"
- Copyright 2026
- **NO fake addresses. NO template placeholders.**

### 3.5 Responsive Breakpoints

| Breakpoint | Layout |
|---|---|
| Desktop (1200px+) | Full layout, 3-column grids, side-by-side sections |
| Tablet (768-1199px) | 2-column grids, stacked hero content |
| Mobile (<768px) | Single column, hamburger nav, full-width cards, larger touch targets |

### 3.6 Performance Targets

| Metric | Target |
|---|---|
| First Contentful Paint | < 1.5s |
| Largest Contentful Paint | < 2.5s |
| Total page size | < 2MB |
| Images | WebP, lazy-loaded, responsive srcset |
| Fonts | System stack + 1 Google Font (preloaded) |
| JavaScript | Minimal — scroll animations, mobile nav, form handling only |

### 3.7 i18n Architecture (for Arabic toggle)

- All text content stored in a `lang/en.json` and `lang/ar.json` file
- Language toggle switches content via JS (no page reload)
- HTML `dir="rtl"` applied when Arabic active
- CSS uses logical properties (`margin-inline-start` not `margin-left`)
- Fonts: include Arabic-compatible font (Noto Sans Arabic or IBM Plex Arabic)

### 3.8 Form Handling

- Contact form + Catalog request form
- Backend: Formspree, Netlify Forms, or a simple Firebase endpoint
- Fields: Name, Company, Email, Phone, Message, Checkbox (Catalog / Showroom / General)
- Thank-you message inline (no redirect)
- Optional: send notification email to Elissar

---

## Part 4: Multi-Page Site Roadmap (Phase 2)

After the landing page is live and validated:

| Page | Content | SEO Target |
|---|---|---|
| `/about` | Company story, Elissar + team, history, values | `hospitality company Oman` |
| `/services` | Overview of all 7 categories | `hotel supplies Oman` |
| `/services/tableware` | Tableware detail + associated brands | `hotel tableware supplier Oman` |
| `/services/glassware` | Glassware detail + brands | `hotel glassware Muscat` |
| `/services/flatware` | Flatware detail + brands | `flatware supplier Gulf` |
| `/services/buffet` | Buffet & banquet equipment | `buffet equipment hotel Oman` |
| `/services/kitchen` | Commercial kitchen equipment | `commercial kitchen equipment Oman` |
| `/services/linen` | Linen & amenities | `hotel linen supplier Middle East` |
| `/services/furniture` | Furniture & lighting | `hotel furniture supplier Oman` |
| `/partners` | All brand partners overview | `hotel brands distributor Oman` |
| `/partners/[brand]` | Individual brand pages (top 10 first) | `[brand] distributor Oman` |
| `/clients` | Hotel portfolio with project descriptions | `hotel supplier portfolio` |
| `/blog` | Industry articles, guides, spotlights | Long-tail keywords |
| `/contact` | Full contact with per-country details | `contact hotel supplier Oman` |

---

## Part 5: Implementation Order

1. **Landing page** — design + build + deploy to GitHub Pages
2. **SEO foundation** — meta tags, schema, sitemap, GSC setup
3. **Google Business Profile** — claim both locations
4. **Multi-page expansion** — one page at a time, starting with About + Services
5. **Blog launch** — first 3-5 articles targeting long-tail keywords
6. **Arabic toggle** — translate landing page content first
7. **Backlink campaign** — directories, trade shows, brand partner links

---

*Ref: Problems addressed by this design — P1 through P15 (see 01-audit-current-site.md)*
