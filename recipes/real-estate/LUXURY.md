# Luxury Real Estate Recipe

> **Variant Focus**: High-end properties, luxury homes, estates
> **Examples**: Sotheby's International Realty, Christie's Real Estate, The Agency
> **Key Differentiator**: Visual storytelling, exclusivity, white-glove service
> **Revenue Model**: Commission on luxury transactions (higher price points)
> **Target**: High-net-worth individuals, international buyers, relocating executives

---

## How This Differs from Standard Residential

| Aspect | Standard Residential | Luxury Real Estate |
|--------|----------------------|-------------------|
| Hero | Search-focused | Visual/cinematic |
| Photography | Good photos | Architectural photography |
| Listings | Database grid | Curated galleries |
| Copy | Functional | Lifestyle-focused |
| Video | Optional | Essential (property films) |
| Agents | Directory | Featured experts |
| Branding | Professional | Aspirational |
| Privacy | Standard | Discrete listings option |

---

## Site Architecture

### Core Pages

```
/                       Homepage (visual showcase)
├── /properties/        Curated property collection
│   ├── /properties/for-sale/
│   ├── /properties/new-developments/
│   ├── /properties/rentals/
│   └── /properties/[id]/     Property showcase
├── /locations/         Destination guides
│   └── /locations/[area]/
├── /team/              Advisors/agents
│   └── /team/[name]/
├── /services/          White-glove services
├── /about/             Brand story
├── /journal/           Lifestyle content
└── /contact/           Inquiry
```

### Optional Pages

```
├── /lifestyle/         Lifestyle content sections
├── /market-insights/   Market reports
├── /new-developments/  Pre-construction projects
├── /private-listings/  Off-market properties
├── /international/     Global offices/network
└── /press/             Media coverage
```

---

## Homepage Structure

### Visual-First Approach

```
1. Hero
   └── Full-screen property video/image, minimal text

2. Featured Properties
   └── Curated selection (3-6 properties)

3. Locations/Destinations
   └── Markets we serve

4. Our Services
   └── What sets us apart

5. Team Showcase
   └── Featured advisors

6. Journal/Insights
   └── Lifestyle content preview

7. Brand Story
   └── Brief about section

8. Footer
   └── Global locations, contact
```

### Hero Pattern (Cinematic)

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│         [Full-screen video or hero image]                       │
│                                                                 │
│                                                                 │
│                                                                 │
│                                                                 │
│                                                                 │
│                         [Brand Name]                            │
│                    Exceptional Properties                       │
│                                                                 │
│                    [Explore Properties]                         │
│                                                                 │
│                            ↓                                    │
│                      Scroll to discover                         │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Alternative: Property Carousel Hero

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│         [Full-screen property image 1]                         │
│                                                                 │
│                                                                 │
│         $12,500,000                                             │
│         Oceanfront Estate | Malibu                              │
│         6 Bed · 8 Bath · 12,000 SF                             │
│                                                                 │
│         [View Property]                                         │
│                                                                 │
│  ○ ● ○ ○ ○                                        ← →          │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Property Presentation

### Luxury Property Card

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│         [Full-bleed property photograph]                        │
│                                                                 │
│                                                                 │
│                                                                 │
│                                                                 │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Oceanfront Estate                                              │
│  Malibu, California                                             │
│                                                                 │
│  $12,500,000                                                    │
│                                                                 │
│  6 Bedrooms · 8 Bathrooms · 12,000 SF                          │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Property Detail Page (Luxury Format)

```
1. Visual Hero
   └── Full-screen image/video with minimal overlay

2. Gallery
   └── Architectural photography, room-by-room

3. Overview
   └── Poetic property description

4. Property Film (if available)
   └── Cinematic property video

5. Features
   └── Luxury amenities, highlighted

6. Floor Plans
   └── Architectural drawings

7. Location
   └── Neighborhood lifestyle, map

8. Virtual Tour
   └── 3D walkthrough (Matterport)

9. Inquire
   └── Private viewing request

10. Similar Properties
    └── Related luxury listings

11. Advisor
    └── Listing advisor contact
```

### Property Description Style

**Standard (Avoid)**:
```
This 6-bedroom home has 8 bathrooms and 12,000 sq ft.
Features include a pool, ocean views, and modern kitchen.
```

**Luxury (Preferred)**:
```
Perched above the Pacific, this architectural masterpiece
offers an unparalleled coastal living experience. Floor-to-ceiling
glass frames endless ocean vistas, while the open floor plan
seamlessly connects indoor and outdoor entertaining spaces.
A true sanctuary where modern design meets natural beauty.
```

---

## Visual Standards

### Photography Requirements

| Element | Standard | Luxury |
|---------|----------|--------|
| Camera | DSLR | Medium format or professional DSLR |
| Lighting | Natural | Professional lighting setup |
| Editing | Basic | Architectural color grading |
| Staging | Furniture | Professional staging, lifestyle |
| Exteriors | Daylight | Golden hour, twilight shots |
| Aerials | Optional | Drone photography required |

### Video Requirements

- Property films (2-3 minutes)
- Cinematic quality
- Lifestyle storytelling
- Professional voiceover or music
- Drone footage
- 4K resolution

### Virtual Tours

- Matterport 3D tours
- High-quality photography base
- Floor plan integration
- Guided tour option

---

## Location/Destination Pages

### Destination Guide Structure

```
1. Hero
   └── Stunning location photography

2. Introduction
   └── What makes this place special

3. Lifestyle
   └── Culture, dining, activities

4. Featured Properties
   └── Available properties here

5. Market Insights
   └── Pricing, trends

6. Why Live Here
   └── Benefits, community

7. Our Local Experts
   └── Advisors specializing here

8. Inquire
   └── "Explore [Location] properties"
```

### Destination Hero Pattern

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│         [Stunning location photography]                         │
│                                                                 │
│                                                                 │
│                                                                 │
│                                                                 │
│                    [Location Name]                              │
│                                                                 │
│         "Where [unique characteristic]"                         │
│                                                                 │
│                  [View Properties]                              │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Team/Advisor Pages

### Advisor Profile (Luxury Format)

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│         [Professional portrait - editorial style]               │
│                                                                 │
│                                                                 │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Jane Smith                                                     │
│  Principal · Founding Partner                                   │
│                                                                 │
│  Specializing in architectural residences and                   │
│  oceanfront estates across Malibu and Pacific Palisades.       │
│                                                                 │
│  Over $500M in career sales                                    │
│                                                                 │
│  [Contact]  [View Properties]                                  │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Current Listings (6)                                          │
│                                                                 │
│  [Property Cards...]                                           │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Client Testimonials                                           │
│                                                                 │
│  "[Quote]" - Client Name                                       │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Services Page

### White-Glove Services

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Exceptional Service                                            │
│                                                                 │
│  ┌────────────────┐  ┌────────────────┐  ┌────────────────┐   │
│  │                │  │                │  │                │   │
│  │ Property       │  │ Buyer          │  │ Seller         │   │
│  │ Marketing      │  │ Advisory       │  │ Services       │   │
│  │                │  │                │  │                │   │
│  └────────────────┘  └────────────────┘  └────────────────┘   │
│                                                                 │
│  ┌────────────────┐  ┌────────────────┐  ┌────────────────┐   │
│  │                │  │                │  │                │   │
│  │ New            │  │ Relocation     │  │ International  │   │
│  │ Development    │  │ Services       │  │ Network        │   │
│  │                │  │                │  │                │   │
│  └────────────────┘  └────────────────┘  └────────────────┘   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Service Details

| Service | Description |
|---------|-------------|
| Property Marketing | Professional photography, video, staging |
| Buyer Advisory | Property search, negotiation, due diligence |
| Seller Services | Pricing strategy, marketing, showings |
| New Development | Pre-construction sales, project marketing |
| Relocation | Executive relocation, temporary housing |
| International | Global network, international buyers |
| Concierge | Move coordination, vendor referrals |
| Private Listings | Off-market properties, discrete sales |

---

## Lead Capture (Luxury Approach)

### Inquiry Form (Elegant)

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Schedule a Private Viewing                                     │
│                                                                 │
│  Name                                                           │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │                                                           │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
│  Email                              Phone                       │
│  ┌─────────────────────────────┐  ┌─────────────────────────┐  │
│  │                             │  │                         │  │
│  └─────────────────────────────┘  └─────────────────────────┘  │
│                                                                 │
│  I am interested in:                                           │
│  ○ Purchasing   ○ Renting   ○ Selling                         │
│                                                                 │
│  Preferred contact method:                                      │
│  ○ Phone   ○ Email   ○ Either                                 │
│                                                                 │
│  Message (optional)                                             │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │                                                           │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
│  [Request Information]                                         │
│                                                                 │
│  Your inquiry will be handled with complete discretion.        │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Privacy Considerations

- Discrete inquiry handling
- No public property addresses (on request)
- Private viewing by appointment only
- Non-disclosure options
- Qualified buyer verification

---

## Content Strategy

### Journal/Editorial Content

| Topic Type | Examples |
|------------|----------|
| Architecture | "Architectural Trends in Modern Estates" |
| Design | "Interior Design Insights" |
| Lifestyle | "Living in [Location]" |
| Market | "Q4 Luxury Market Report" |
| Properties | "Inside: [Property Address]" |

### Visual Content Priority

```
1. Property films (highest impact)
2. Aerial photography
3. Twilight/golden hour shots
4. Lifestyle photography
5. Market data visualization
```

---

## Technical Considerations

### Performance for High-Quality Media

- Image optimization (WebP, lazy loading)
- Video hosting (Vimeo Pro, YouTube)
- CDN for fast global delivery
- Progressive image loading
- Bandwidth-conscious mobile versions

### International Considerations

- Multi-currency display
- Multi-language support
- International phone formats
- Time zone handling
- Global contact options

---

## Implementation Checklist

### Foundation
- [ ] Premium design/branding
- [ ] Fast, secure hosting
- [ ] Mobile-responsive
- [ ] Video hosting solution

### Visual Content
- [ ] Professional photography standards
- [ ] Property films (top listings)
- [ ] Aerial/drone photography
- [ ] Virtual tours (Matterport)

### Pages
- [ ] Visual-first homepage
- [ ] Curated property galleries
- [ ] Destination/location guides
- [ ] Advisor profiles
- [ ] Services overview

### Functionality
- [ ] Elegant inquiry forms
- [ ] Property search (refined)
- [ ] Saved properties
- [ ] Privacy options

### Content
- [ ] Editorial blog/journal
- [ ] Market reports
- [ ] Lifestyle content
- [ ] Video library

---

## Sources

- [Sotheby's International Realty](https://www.sothebysrealty.com/) - Luxury reference
- [The Agency](https://www.theagencyre.com/) - Modern luxury approach
- [Douglas Elliman](https://www.elliman.com/) - Major market luxury
- [Luxury Portfolio International](https://www.luxuryportfolio.com/)
- [Institute for Luxury Home Marketing](https://www.luxuryhomemarketing.com/)
