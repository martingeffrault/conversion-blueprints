# Real Estate Website Recipe

> **Business Type**: Real estate agency, property portal, broker website
> **Primary Goals**: Generate leads, showcase properties, connect buyers/sellers
> **Revenue Model**: Commissions, listing fees, lead sales
> **Reference Sites**: Zillow, Redfin, Realtor.com, Compass, Century 21, local agencies

---

## Site Architecture

### Core Pages (Must Have)

```
/                           Homepage (search-focused)
├── /properties/            All property listings
│   ├── /properties/sale/   Properties for sale
│   ├── /properties/rent/   Properties for rent
│   └── /properties/[slug]/ Individual property pages
├── /search/                Property search (with filters)
├── /map/                   Map-based search view
├── /agents/                Agent directory
│   └── /agents/[slug]/     Individual agent profiles
├── /about/                 About the agency
├── /contact/               Contact page
└── /estimation/            Property valuation tool
```

### Content Pages

```
├── /neighborhoods/         Area guides
│   └── /neighborhoods/[area]/
├── /guides/               Buyer/seller guides
│   ├── /guides/buying/    Buying guide
│   ├── /guides/selling/   Selling guide
│   └── /guides/renting/   Renting guide
├── /blog/                 Market insights, news
│   └── /blog/[post]/
└── /mortgage-calculator/  Financial tools
```

### Account Pages (if applicable)

```
├── /account/
│   ├── /account/favorites/    Saved properties
│   ├── /account/searches/     Saved searches
│   ├── /account/alerts/       Property alerts
│   └── /account/messages/     Agent messages
```

### Legal Pages

```
├── /legal/
│   ├── /privacy/
│   ├── /terms/
│   └── /fair-housing/     Fair housing statement
```

---

## Page Hierarchy Diagram

```
                        ┌─────────────┐
                        │  HOMEPAGE   │
                        │  (Search)   │
                        └──────┬──────┘
                               │
      ┌────────────────────────┼────────────────────────┐
      │                        │                        │
 ┌────▼────┐             ┌────▼────┐             ┌────▼────┐
 │LISTINGS │             │  AREAS  │             │ AGENTS  │
 └────┬────┘             └────┬────┘             └────┬────┘
      │                       │                       │
 ┌────┼────┐             ┌────┼────┐             ┌────┼────┐
 │    │    │             │    │    │             │    │    │
Sale Rent Search     Neighborhood  Agent       Agent  Agent
                       Guides     Listings     Profile Contact
      │
      └───────┐
              │
        Property Page
              │
        ┌─────┼─────┐
        │     │     │
    Gallery Details Contact
```

---

## Homepage Structure

The homepage should be search-centric—help visitors find properties fast.

### Recommended Section Order

```
1. Header
   └── Logo, navigation, phone, agent login

2. Hero Search
   └── Prominent search bar with filters

3. Featured Properties
   └── Premium/new listings (6-12 properties)

4. Search by Type
   └── Sale, Rent, New Development

5. Neighborhoods/Areas
   └── Popular area cards with property counts

6. Why Choose Us
   └── Trust signals, experience, results

7. Agent Spotlight
   └── Featured agents with stats

8. Market Insights (optional)
   └── Recent blog posts or market data

9. Testimonials
   └── Client success stories

10. CTA
    └── Valuation, contact, newsletter

11. Footer
    └── Areas served, contact, legal
```

### Homepage Hero (Search-Focused)

> "An exceptional user experience is at the heart of modern web design. For real estate platforms, it means clean design, intuitive navigation, clear calls-to-action, and user-friendly interfaces."
>
> *Source: [Property Web Masters](https://www.propertywebmasters.com/news/best-real-estate-website-design-best-practices-for-2024/)*

```
┌─────────────────────────────────────────────────────────────────┐
│ [Logo]   Buy  Rent  Sell  Areas  Agents  About   📞 555-1234    │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│            [High-quality background image]                      │
│                                                                 │
│              Find Your Dream Home                               │
│                                                                 │
│   ┌─────────────────────────────────────────────────────────┐  │
│   │  [Buy ▼]  [Location        ]  [Type ▼]  [🔍 Search]     │  │
│   └─────────────────────────────────────────────────────────┘  │
│                                                                 │
│   Quick links: Paris • Lyon • Marseille • Bordeaux              │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Property Search Experience

### Search Bar Components

> "Strategically showcasing property listings with advanced search options, filters and personalised recommendations add value to the user experience, catering to their specific needs and preferences."
>
> *Source: [Property Web Masters](https://www.propertywebmasters.com/news/best-real-estate-website-design-best-practices-for-2024/)*

**Essential search fields:**

| Field | Type | Notes |
|-------|------|-------|
| **Transaction type** | Toggle/tabs | Buy, Rent, (Sold) |
| **Location** | Autocomplete | City, neighborhood, postal code |
| **Property type** | Dropdown | House, Apartment, Land, etc. |
| **Min/Max price** | Range sliders or inputs | |
| **Bedrooms** | Buttons/dropdown | Any, 1, 2, 3, 4+ |

**Advanced filters (expandable):**

| Field | Type |
|-------|------|
| Min/Max area | Range |
| Bathrooms | Dropdown |
| Parking | Checkbox |
| Year built | Range |
| Features | Multi-select (pool, garden, etc.) |
| Energy rating | Multi-select |

### Search Results Page

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Modify Search] ← Sticky search bar                            │
│                                                                 │
│  125 properties in Paris                [Sort: Newest ▼]        │
│                                                                 │
│  Active Filters: [3+ beds ×] [€500K-1M ×] [Clear all]          │
│                                                                 │
│  [List View] [Grid View] [Map View]                             │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐ │
│  │                 │  │                 │  │                 │ │
│  │ [Property Card] │  │ [Property Card] │  │ [Property Card] │ │
│  │                 │  │                 │  │                 │ │
│  └─────────────────┘  └─────────────────┘  └─────────────────┘ │
│                                                                 │
│  [Pagination or Load More]                                      │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Map-Based Search

> "Dynamic maps have gone beyond mere basic location information. These interactive maps are embedded with live data such as schools, shopping centers, hospitals and even traffic conditions."
>
> *Source: [Web Design Inspiration](https://www.webdesign-inspiration.com/article/innovative-web-design-trends-for-real-estate-websites-in-2024/)*

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  ┌────────────────────────┐  ┌──────────────────────────────┐  │
│  │                        │  │                              │  │
│  │   Results List         │  │      Interactive Map         │  │
│  │   (scrollable)         │  │                              │  │
│  │                        │  │      [Property Markers]      │  │
│  │   [Property Card]      │  │                              │  │
│  │   [Property Card]      │  │      POIs: Schools, Transit  │  │
│  │   [Property Card]      │  │      Neighborhood boundaries │  │
│  │   [Property Card]      │  │                              │  │
│  │   ...                  │  │                              │  │
│  │                        │  │                              │  │
│  └────────────────────────┘  └──────────────────────────────┘  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Map features to include:**
- Property markers with price labels
- Cluster markers for dense areas
- Marker click → Mini property card
- Draw-to-search (draw area on map)
- Points of interest (schools, transit, shops)
- Neighborhood boundaries

---

## Property Page Structure

The property page is the conversion point—make it complete and compelling.

### Essential Sections

```
1. Breadcrumbs
   └── Home > Paris > 16th > This Property

2. Gallery
   └── Large images, thumbnails, fullscreen, virtual tour

3. Key Info
   └── Price, beds, baths, area, type

4. Quick Actions
   └── Contact agent, save, share, schedule visit

5. Description
   └── Property description, features highlights

6. Features & Amenities
   └── Organized list of features

7. Energy Rating (DPE/GES)
   └── Official energy labels

8. Location
   └── Map, neighborhood info, nearby amenities

9. Agent Info
   └── Agent card, contact form

10. Similar Properties
    └── Related listings

11. Recently Viewed
    └── User's browsing history
```

### Property Page Layout

> "Optimising property listings involves using high-quality images, accurate descriptions, and virtual tours where possible to showcase the listings in the best light."
>
> *Source: [Property Web Masters](https://www.propertywebmasters.com/news/best-real-estate-website-design-best-practices-for-2024/)*

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Home > Paris > 16th > Beautiful Apartment...                   │
│                                                                 │
│  ┌──────────────────────────────────────────────────────────┐  │
│  │                                                          │  │
│  │              [Main Image Gallery]                        │  │
│  │                                                          │  │
│  │  [thumb] [thumb] [thumb] [+12]  [🎬 Virtual Tour]       │  │
│  │                                                          │  │
│  └──────────────────────────────────────────────────────────┘  │
│                                                                 │
│  ┌─────────────────────────────┐  ┌──────────────────────────┐ │
│  │                             │  │                          │ │
│  │  Beautiful Apartment        │  │  € 850,000               │ │
│  │  Paris 16th                 │  │  ────────                │ │
│  │                             │  │  € 8,500/m²              │ │
│  │  🛏 3 beds  🚿 2 baths      │  │                          │ │
│  │  📐 100m²  🏢 5th floor     │  │  [♡ Save] [↗ Share]      │ │
│  │                             │  │                          │ │
│  │  Ref: PAR-2024-1234         │  │  [📞 Contact Agent]      │ │
│  │                             │  │  [📅 Schedule Visit]     │ │
│  └─────────────────────────────┘  └──────────────────────────┘ │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Description                                                    │
│  ───────────                                                    │
│                                                                 │
│  Stunning apartment in the heart of Paris 16th...               │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Features                                                       │
│  ────────                                                       │
│                                                                 │
│  ✓ Balcony      ✓ Parking    ✓ Cellar     ✓ Elevator          │
│  ✓ Concierge    ✓ Parquet    ✓ Fireplace  ✓ AC                │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Energy Rating                                                  │
│  ─────────────                                                  │
│                                                                 │
│  DPE: [==C===] 125 kWh/m²/year                                 │
│  GES: [==B===] 18 kgCO₂/m²/year                                │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Location                                                       │
│  ────────                                                       │
│                                                                 │
│  [Interactive Map]                                              │
│                                                                 │
│  Nearby: Metro (2min) • Schools • Shops • Park                  │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌────────────────────────────┐  ┌─────────────────────────┐   │
│  │                            │  │                         │   │
│  │  Your Agent                │  │  Contact Form           │   │
│  │                            │  │                         │   │
│  │  [Photo]                   │  │  Name                   │   │
│  │  Marie Dupont              │  │  [____________]         │   │
│  │  Senior Agent              │  │                         │   │
│  │                            │  │  Email                  │   │
│  │  ★★★★★ 48 reviews         │  │  [____________]         │   │
│  │                            │  │                         │   │
│  │  📞 01 23 45 67 89        │  │  Phone                  │   │
│  │  📧 marie@agency.com      │  │  [____________]         │   │
│  │                            │  │                         │   │
│  │  [View Profile]            │  │  Message                │   │
│  │                            │  │  [____________]         │   │
│  │                            │  │                         │   │
│  │                            │  │  [Request Info]         │   │
│  │                            │  │                         │   │
│  └────────────────────────────┘  └─────────────────────────┘   │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Similar Properties                                             │
│                                                                 │
│  [Property] [Property] [Property] [Property]                    │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Property Gallery Best Practices

> "Property images should be at least 1200 pixels wide and properly compressed for web use. Virtual tours have become increasingly important, with listings featuring them receiving significantly more views."
>
> *Source: [Housing Wire](https://www.housingwire.com/articles/real-estate-website-design/)*

**Gallery features:**
- Large main image (hero size)
- Thumbnail navigation
- Full-screen mode
- Virtual tour button (prominent)
- Video walkthrough if available
- Photo count indicator
- Lazy loading for performance
- Keyboard navigation

### Property Card Design

```
┌─────────────────────────────────────┐
│ [Property Image]           [♡]     │
│                           EXCLU    │
│                                    │
│ € 450,000                          │
│ Beautiful 3BR in Lyon              │
│                                    │
│ 🛏 3  🚿 2  📐 85m²                │
│                                    │
│ Lyon 6th • Apartment               │
│                                    │
│ [View Property]                    │
│                                    │
└────────────────────────────────────┘
```

**Card elements:**
- High-quality image (4:3 or 3:2 ratio)
- Favorite button (heart icon)
- Badges (New, Exclusive, Price Drop)
- Price (prominently displayed)
- Title/Address (truncated if needed)
- Key specs (beds, baths, area)
- Location and type
- Optional: Agent info, price/m²

---

## Agent Pages

### Agent Directory

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Our Agents                                                     │
│                                                                 │
│  [Search by name or area]                                       │
│                                                                 │
│  Filter by: [All Areas ▼] [Specialty ▼]                        │
│                                                                 │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐             │
│  │ [Photo]     │  │ [Photo]     │  │ [Photo]     │             │
│  │ Marie D.    │  │ Jean P.     │  │ Sophie M.   │             │
│  │ Paris       │  │ Lyon        │  │ Bordeaux    │             │
│  │ ★★★★★ (48) │  │ ★★★★☆ (32) │  │ ★★★★★ (56) │             │
│  │ 12 listings │  │ 8 listings  │  │ 15 listings │             │
│  │ [Contact]   │  │ [Contact]   │  │ [Contact]   │             │
│  └─────────────┘  └─────────────┘  └─────────────┘             │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Agent Profile Page

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  ┌─────────────────────┐  ┌──────────────────────────────────┐ │
│  │                     │  │                                  │ │
│  │    [Agent Photo]    │  │  Marie Dupont                    │ │
│  │                     │  │  Senior Real Estate Agent        │ │
│  │                     │  │                                  │ │
│  │                     │  │  ★★★★★ 4.9/5 (48 reviews)       │ │
│  │                     │  │                                  │ │
│  │                     │  │  Specialties: Paris 16th, 17th   │ │
│  │                     │  │  Languages: FR, EN, ES           │ │
│  │                     │  │                                  │ │
│  │                     │  │  📞 01 23 45 67 89               │ │
│  │                     │  │  📧 marie@agency.com             │ │
│  │                     │  │                                  │ │
│  │                     │  │  [Contact Marie]                 │ │
│  │                     │  │                                  │ │
│  └─────────────────────┘  └──────────────────────────────────┘ │
│                                                                 │
│  About Marie                                                    │
│  ───────────                                                    │
│  Bio text about experience, approach, and expertise...          │
│                                                                 │
│  Stats                                                          │
│  ─────                                                          │
│  [120+] Properties sold | [15] Years experience | [98%] Client  │
│                           satisfaction                          │
│                                                                 │
│  Marie's Active Listings (12)                                   │
│  ────────────────────────────                                   │
│                                                                 │
│  [Property Cards Grid]                                          │
│                                                                 │
│  Client Reviews                                                 │
│  ──────────────                                                 │
│                                                                 │
│  [Review testimonials]                                          │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Lead Generation Elements

### Contact Forms

> "Implementing quick enquiry forms, live chat support and integrative mapping features enhances user engagement and encourages proactive communication."
>
> *Source: [Property Web Masters](https://www.propertywebmasters.com/news/best-real-estate-website-design-best-practices-for-2024/)*

**Property inquiry form (minimal):**
- Name*
- Email*
- Phone*
- Message (pre-filled with property reference)
- Preferred contact method
- Best time to call

**Valuation request form:**
- Property address*
- Property type*
- Approximate size*
- Contact info*
- When looking to sell

### Call-to-Action Placement

| Location | CTA Type |
|----------|----------|
| Header | Phone number, prominent |
| Hero | Search bar + "Or call us" |
| Property page | Contact agent, schedule visit |
| Sticky footer (mobile) | Call + Inquiry buttons |
| After search results | "Can't find what you need?" |
| Exit intent | Valuation offer popup |

---

## Mobile Considerations

> "Since property searches are predominantly done on mobile devices, adopting a mobile-first design has become essential for real estate websites in 2024."
>
> *Source: [Dream X Web](https://www.dreamxweb.com/blog/real-estate-web-design-trends-a-necessity-or-just-a-fad/)*

**Mobile essentials:**
- Click-to-call phone numbers
- Simplified search (expandable filters)
- Swipeable property galleries
- Sticky bottom bar (Call | Save | Share)
- GPS-based "Properties near me"
- Touch-friendly filters and buttons
- Collapsible property details

### Mobile Property Card

```
┌─────────────────────────┐
│ [Full-width Image]  [♡] │
│                    EXCLU│
│                         │
│ € 450,000               │
│ Beautiful 3BR in Lyon   │
│ 🛏 3  🚿 2  📐 85m²     │
│ Lyon 6th                │
│                         │
│ [Call] [Inquiry]        │
│                         │
└─────────────────────────┘
```

### Mobile Navigation

```
┌─────────────────────────┐
│ [☰] [Logo]  [🔍] [📞]  │
└─────────────────────────┘

Bottom Nav:
┌─────────────────────────┐
│ [🏠] [🔍] [♡] [👤]     │
│ Home Search Saved Account│
└─────────────────────────┘
```

---

## Trust & Credibility

### Trust Elements for Real Estate

| Element | Placement |
|---------|-----------|
| **Agency credentials** | Footer, About page |
| **Agent certifications** | Agent profiles |
| **Client testimonials** | Homepage, Agent pages |
| **Properties sold count** | Homepage stats |
| **Years in business** | About, footer |
| **Professional memberships** | Footer |
| **Press coverage** | About page |
| **Awards/recognition** | Homepage, About |

### Social Proof

- Number of properties listed
- Number of successful transactions
- Client satisfaction percentage
- Time on market (if impressive)
- Price achievement vs. asking

---

## SEO Considerations

### Key Page Types to Optimize

| Page Type | Target Keywords |
|-----------|-----------------|
| Homepage | "[city] real estate agency" |
| Category | "apartments for sale [city]" |
| Area pages | "[neighborhood] real estate" |
| Property pages | "[address]" (long-tail) |
| Guides | "how to buy house [city]" |

### Schema Markup

- `RealEstateListing` for properties
- `LocalBusiness` for agency
- `Person` for agents
- `Review` for testimonials
- `BreadcrumbList` for navigation
- `FAQPage` for guides

### URL Structure

```
/properties/sale/paris/
/properties/sale/paris/apartment/
/properties/sale/paris/3-beds/
/properties/ref-PAR-2024-1234/
/neighborhoods/paris-16/
/agents/marie-dupont/
```

---

## Performance

### Image Optimization

> "Property images should be at least 1200 pixels wide and properly compressed for web use. Tools like TinyPNG can reduce file size without noticeably affecting quality."
>
> *Source: [Housing Wire](https://www.housingwire.com/articles/real-estate-website-design/)*

- WebP format with JPEG fallback
- Multiple sizes for responsive images
- Lazy loading for gallery thumbnails
- Placeholder/blur-up while loading
- CDN for property images

### Search Performance

- Server-side filtering for large datasets
- Debounced autocomplete
- Cache common searches
- Progressive loading of results

---

## Key User Journeys

### Journey 1: Buyer Search

```
Homepage → Search → Results → Property Page → Contact Agent → Lead
```

### Journey 2: Direct Property

```
External Link/Ad → Property Page → View Gallery → Contact → Lead
```

### Journey 3: Seller Valuation

```
Homepage → Valuation CTA → Form → Lead → Agent Contact
```

### Journey 4: Agent Lookup

```
Homepage → Agents → Agent Profile → View Listings → Contact
```

---

## Implementation Checklist

### Foundation
- [ ] Homepage with prominent search
- [ ] Property listing pages
- [ ] Property detail pages
- [ ] Agent pages
- [ ] Contact/About pages

### Search
- [ ] Basic search (location, type, price)
- [ ] Advanced filters
- [ ] Map-based search
- [ ] Saved searches (if account system)

### Property Pages
- [ ] Full-featured gallery
- [ ] Virtual tour integration
- [ ] Key specs display
- [ ] Energy rating display
- [ ] Contact form

### Lead Generation
- [ ] Inquiry forms on properties
- [ ] Valuation tool/form
- [ ] Agent contact forms
- [ ] Click-to-call integration

### Mobile
- [ ] Responsive design
- [ ] Click-to-call
- [ ] Mobile-friendly search
- [ ] Touch-optimized gallery

### SEO
- [ ] Schema markup
- [ ] Optimized URLs
- [ ] Meta tags per page
- [ ] Sitemap with properties

### Performance
- [ ] Optimized images
- [ ] Fast search
- [ ] Caching strategy
- [ ] CDN for media

---

## Sources

- [Property Web Masters - Best Practices for 2024](https://www.propertywebmasters.com/news/best-real-estate-website-design-best-practices-for-2024/)
- [Housing Wire - Real Estate Website Design](https://www.housingwire.com/articles/real-estate-website-design/)
- [Web Design Inspiration - Trends for 2024](https://www.webdesign-inspiration.com/article/innovative-web-design-trends-for-real-estate-websites-in-2024/)
- [Dream X Web - Real Estate Web Design Trends](https://www.dreamxweb.com/blog/real-estate-web-design-trends-a-necessity-or-just-a-fad/)
- [AgentFire - Real Estate Website Design Best Practices](https://agentfire.com/blog/real-estate-website-design-best-practices/)
