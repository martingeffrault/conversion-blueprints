# Residential Real Estate Agency Recipe

> **Variant Focus**: Traditional residential real estate agencies and brokerages
> **Examples**: Keller Williams, RE/MAX, Coldwell Banker, local brokerages
> **Key Differentiator**: Agent-centric, listings database, local market expertise
> **Revenue Model**: Commission on sales/rentals
> **Target**: Home buyers, sellers, renters in local market

---

## How This Differs from Generic Real Estate

| Aspect | Generic Real Estate | Residential Agency |
|--------|---------------------|-------------------|
| Focus | Properties only | Agents + properties |
| Trust | Listings quality | Agent reputation |
| Conversion | Property inquiries | Agent assignment + inquiries |
| Content | Property details | Market insights + guides |
| SEO | Property searches | Location + agent searches |

---

## Site Architecture

### Core Pages

```
/                       Homepage (search + featured listings)
├── /properties/        Property search/listings
│   ├── /properties/for-sale/
│   ├── /properties/for-rent/
│   └── /properties/[id]/     Individual listing
├── /agents/            Agent directory
│   └── /agents/[name]/       Agent profiles
├── /neighborhoods/     Neighborhood guides
│   └── /neighborhoods/[area]/
├── /sell/              Sellers landing page
├── /buy/               Buyers landing page
├── /rent/              Renters landing page
├── /about/             Agency story, values
├── /contact/           Contact + office locations
└── /blog/              Market updates, guides
```

### Optional Pages

```
├── /valuation/         Free home valuation tool
├── /mortgage/          Mortgage calculator/info
├── /sold/              Recently sold properties
├── /testimonials/      Client success stories
├── /careers/           Recruitment for agents
└── /commercial/        Commercial properties (if applicable)
```

---

## Homepage Structure

### Recommended Sections

```
1. Hero
   └── Search bar prominent, featured listings

2. Quick Search
   └── Buy / Rent / Sell toggles with filters

3. Featured Listings
   └── Premium/featured properties

4. Why Choose Us
   └── Agency differentiators

5. Neighborhoods
   └── Area guides with quick links

6. Our Agents
   └── Featured agent profiles

7. Testimonials
   └── Client success stories

8. Market Insights
   └── Recent blog posts/market data

9. CTA Section
   └── "Ready to find your home?"

10. Footer
    └── Office locations, contact, social
```

### Hero Pattern with Search

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│         [Background: Local cityscape or home]                   │
│                                                                 │
│         Find Your Perfect Home in [City/Region]                │
│                                                                 │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │ [Buy ▼] [City, ZIP, or Address___________] [🔍 Search]    │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
│  Popular: [Downtown] [Suburbs] [Waterfront] [New Construction] │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Property Listings

### Property Card Pattern

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Property Image Gallery]                         [♡] [Share]  │
│                                                                 │
│  [NEW]  [OPEN HOUSE]                                           │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  $425,000                                                       │
│  123 Main Street, City, State 12345                            │
│                                                                 │
│  🛏️ 3 beds  🛁 2 baths  📐 1,850 sqft  🏡 Single Family       │
│                                                                 │
│  Listed by: Jane Smith, ABC Realty                             │
│                                                                 │
│  [View Details]                    [Schedule Tour]             │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Property Search Filters

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  FILTERS                                                        │
│                                                                 │
│  Location                          Property Type               │
│  ┌─────────────────────────┐      ┌─────────────────────────┐  │
│  │ City, ZIP, Neighborhood │      │ All Types             ▼ │  │
│  └─────────────────────────┘      └─────────────────────────┘  │
│                                                                 │
│  Price Range                       Bedrooms                     │
│  ┌──────────┐  ┌──────────┐       [Any] [1+] [2+] [3+] [4+]   │
│  │ Min    ▼ │  │ Max    ▼ │                                    │
│  └──────────┘  └──────────┘       Bathrooms                    │
│                                   [Any] [1+] [2+] [3+]         │
│  [More Filters ▼]                                              │
│                                                                 │
│  [Clear All]                              [Apply Filters]      │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Property Detail Page Structure

```
1. Gallery
   └── Photo gallery/slideshow, virtual tour link

2. Key Details
   └── Price, beds, baths, sqft, lot size

3. Property Description
   └── Full description, features

4. Features & Amenities
   └── Categorized list of features

5. Location & Map
   └── Map, nearby amenities, commute times

6. Agent Contact
   └── Listing agent card with contact options

7. Mortgage Calculator
   └── Estimated monthly payment

8. Similar Properties
   └── Related listings

9. Contact Form
   └── Schedule showing, ask question
```

---

## Agent Directory

### Agent Profile Page Structure

```
1. Hero
   └── Photo, name, title, contact buttons

2. About
   └── Bio, experience, specialties

3. Credentials
   └── Licenses, certifications, awards

4. Active Listings
   └── Current properties for sale/rent

5. Sold Properties
   └── Recent transactions (if public)

6. Client Reviews
   └── Testimonials from past clients

7. Market Expertise
   └── Areas/neighborhoods served

8. Contact Form
   └── Direct contact to agent
```

### Agent Card Pattern

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  ┌──────────────────┐                                          │
│  │                  │  Jane Smith                               │
│  │  [Agent Photo]   │  Senior Sales Associate                   │
│  │                  │                                          │
│  └──────────────────┘  ★★★★★ 4.9 (127 reviews)                │
│                                                                 │
│  Specialties: Luxury Homes, First-Time Buyers                  │
│  Areas: Downtown, Suburbs                                       │
│                                                                 │
│  📧 jane@agency.com   📞 (555) 123-4567                        │
│                                                                 │
│  [View Profile]                [Contact Agent]                 │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Seller & Buyer Landing Pages

### Seller Page Structure

```
1. Hero
   └── "Sell Your Home" + CTA for valuation

2. Market Stats
   └── Average sale price, days on market, appreciation

3. Our Process
   └── Steps to selling with your agency

4. What We Offer
   └── Marketing, staging, photography, etc.

5. Pricing Strategy
   └── How we price homes

6. Testimonials
   └── Seller success stories

7. Free Valuation CTA
   └── "What's your home worth?"

8. Contact Form
   └── Consultation request
```

### Seller Page Hero Pattern

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│         Ready to Sell Your Home?                               │
│                                                                 │
│         Get a free home valuation and expert guidance          │
│         from our top-rated agents.                             │
│                                                                 │
│         [Get Your Free Valuation]                              │
│                                                                 │
│         ✓ No obligation  ✓ Results in 24 hours                 │
│                                                                 │
│         Average Days on Market: 21                              │
│         Homes Sold This Year: 150+                             │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Buyer Page Structure

```
1. Hero
   └── "Find Your Dream Home" + search

2. Why Buy With Us
   └── Buyer representation benefits

3. Buying Process
   └── Steps from search to close

4. Neighborhood Guides
   └── Featured areas to consider

5. First-Time Buyers
   └── Resources for new buyers

6. Mortgage Resources
   └── Calculator, lender partners

7. Search CTA
   └── "Start your home search"

8. Agent Matching
   └── Get paired with a buyer's agent
```

---

## Neighborhood Guides

### Neighborhood Page Structure

```
1. Hero
   └── Area name, hero image, quick stats

2. Overview
   └── Description of the neighborhood

3. Market Stats
   └── Avg price, inventory, trends

4. Featured Listings
   └── Active listings in this area

5. Schools
   └── School ratings, districts

6. Amenities
   └── Parks, restaurants, shopping

7. Commute
   └── Transportation, drive times

8. Agent Experts
   └── Agents who specialize here

9. CTA
   └── "Explore homes in [Neighborhood]"
```

### Neighborhood Hero Pattern

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│         [Neighborhood background image]                         │
│                                                                 │
│         Living in [Neighborhood Name]                          │
│                                                                 │
│         $450K          15 min          A+                       │
│         Median Price   to Downtown     Schools                  │
│                                                                 │
│         [View Homes]                                           │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Lead Capture Forms

### Property Inquiry Form

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Interested in This Property?                                   │
│                                                                 │
│  Name *                                                         │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │                                                           │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
│  Email *                          Phone *                       │
│  ┌─────────────────────────────┐ ┌─────────────────────────┐  │
│  │                             │ │                         │  │
│  └─────────────────────────────┘ └─────────────────────────┘  │
│                                                                 │
│  How can we help?                                               │
│  [Schedule a Showing]  [Request Info]  [Ask a Question]        │
│                                                                 │
│  Message                                                        │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │                                                           │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
│  [Send Inquiry]                                                │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Home Valuation Form

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  What's Your Home Worth?                                       │
│                                                                 │
│  Get a free, no-obligation market analysis                     │
│                                                                 │
│  Property Address *                                             │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │                                                           │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
│  City *              State *         ZIP *                      │
│  ┌──────────────┐  ┌──────────────┐ ┌───────────────────────┐  │
│  │              │  │              │ │                       │  │
│  └──────────────┘  └──────────────┘ └───────────────────────┘  │
│                                                                 │
│  Name *                            Phone *                      │
│  ┌─────────────────────────────┐  ┌─────────────────────────┐  │
│  │                             │  │                         │  │
│  └─────────────────────────────┘  └─────────────────────────┘  │
│                                                                 │
│  Email *                                                        │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │                                                           │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
│  [Get My Free Valuation]                                       │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Local SEO Strategy

### Key Page Types for SEO

| Page Type | Target Keywords |
|-----------|-----------------|
| Homepage | "[agency] real estate [city]" |
| Listings | "homes for sale in [city]" |
| Neighborhoods | "homes for sale in [neighborhood]" |
| Agent profiles | "[agent name] realtor [city]" |
| Buyer guides | "buying a home in [city]" |
| Seller guides | "selling a home in [city]" |

### Schema Markup

```json
{
  "@type": "RealEstateAgent",
  "name": "ABC Realty",
  "areaServed": [...],
  "makesOffer": {
    "@type": "Offer",
    "itemOffered": {
      "@type": "Service",
      "name": "Residential Real Estate"
    }
  }
}
```

For individual listings:
```json
{
  "@type": "Product",
  "name": "123 Main Street",
  "offers": {
    "@type": "Offer",
    "price": "425000",
    "priceCurrency": "USD"
  }
}
```

---

## IDX Integration

### What is IDX?

IDX (Internet Data Exchange) allows brokerages to display MLS listings on their websites.

### IDX Providers

| Provider | Features |
|----------|----------|
| IDX Broker | Full-featured, customizable |
| Showcase IDX | WordPress plugin |
| iHomeFinder | Optima leads |
| Realtyna | WPL plugin |

### IDX Best Practices

- Ensure mobile-responsive listing display
- Customize search experience
- Capture leads on every listing
- Optimize listing pages for SEO
- Include neighborhood context

---

## Implementation Checklist

### Foundation
- [ ] IDX integration set up
- [ ] Mobile-responsive design
- [ ] SSL certificate
- [ ] Fast page speed

### Content
- [ ] Homepage with search
- [ ] Property listings (via IDX)
- [ ] Agent directory
- [ ] Neighborhood guides (top 5-10)
- [ ] Buyer/seller pages

### Functionality
- [ ] Property search working
- [ ] Lead capture forms
- [ ] Agent contact integration
- [ ] Saved searches (if applicable)
- [ ] Email alerts

### SEO
- [ ] RealEstateAgent schema
- [ ] Product schema on listings
- [ ] Neighborhood pages optimized
- [ ] Google Business Profile
- [ ] Local keywords targeted

---

## Sources

- [National Association of Realtors - Technology](https://www.nar.realtor/technology)
- [Placester - Real Estate Website Best Practices](https://placester.com/)
- [Real Geeks - IDX & Lead Generation](https://www.realgeeks.com/)
- [Zillow - Agent Marketing Guide](https://www.zillow.com/agent-resources/)
