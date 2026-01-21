# SaaS B2B Website Recipe

> **Business Type**: Software as a Service, selling to businesses
> **Primary Goals**: Drive free trials, demo requests, and paid conversions
> **Reference Sites**: Stripe, Linear, Notion, Slack, HubSpot, Intercom

---

## Choose Your Variant

SaaS B2B sites fall into two main go-to-market strategies. Choose the one that matches your business:

| Variant | Best For | Primary CTA | See Details |
|---------|----------|-------------|-------------|
| **[Product-Led Growth (PLG)](PLG.md)** | Self-serve, low ACV (<$1K/yr), freemium | "Start Free" | [PLG.md](PLG.md) |
| **[Sales-Led](SALES-LED.md)** | Enterprise, high ACV (>$10K/yr), complex sales | "Book a Demo" | [SALES-LED.md](SALES-LED.md) |

Many companies use a **hybrid approach** (PLG for SMB, Sales-Led for Enterprise). The architecture below covers common elements.

---

## Site Architecture

### Core Pages (Must Have)

```
/                       Homepage
├── /features/          Features overview (or individual feature pages)
├── /pricing/           Pricing & plans
├── /demo/              Book a demo (high-touch sales)
├── /signup/            Free trial signup (self-serve)
├── /login/             Customer login
└── /contact/           Contact page
```

### Trust & Conversion Pages

```
├── /customers/         Customer stories hub
│   └── /customers/[company]/   Individual case studies
├── /about/             Company story
├── /blog/              Content hub
│   └── /blog/[post]/           Individual posts
└── /resources/         Guides, ebooks, webinars
    └── /resources/[resource]/  Individual resources
```

### Product Pages (For Complex Products)

```
├── /solutions/         Use case pages
│   ├── /solutions/marketing/   For marketing teams
│   ├── /solutions/sales/       For sales teams
│   └── /solutions/enterprise/  For enterprise
├── /integrations/      Integration directory
│   └── /integrations/[app]/    Individual integrations
└── /security/          Security & compliance
```

### Utility Pages

```
├── /terms/             Terms of service
├── /privacy/           Privacy policy
├── /status/            System status
├── /changelog/         Product updates
└── /help/              Help center / Documentation
```

---

## Page Hierarchy Diagram

```
                    ┌─────────────┐
                    │  HOMEPAGE   │
                    └──────┬──────┘
                           │
        ┌──────────────────┼──────────────────┐
        │                  │                  │
   ┌────▼────┐       ┌─────▼─────┐      ┌─────▼─────┐
   │ PRODUCT │       │   TRUST   │      │ CONVERT   │
   └────┬────┘       └─────┬─────┘      └─────┬─────┘
        │                  │                  │
   ┌────┼────┐        ┌────┼────┐        ┌────┼────┐
   │    │    │        │    │    │        │    │    │
Features  Solutions  Customers  About   Pricing  Demo
   │         │          │         │         │      │
Integrations │      Case Studies  Blog     Signup  Contact
             │          │         │
         Use Cases   Resources  Careers
```

---

## Recommended Page Structures

### Homepage
See: [pages/homepage.md](pages/homepage.md)

**Framework**: StoryBrand + Social Proof Heavy
**Sections**:
1. Hero with value prop + dual CTAs
2. Logo cloud (trusted by)
3. Key benefits (3-4)
4. How it works (3 steps)
5. Feature highlights
6. Testimonials
7. Pricing teaser (optional)
8. Final CTA

### Pricing Page
See: [pages/pricing.md](pages/pricing.md)

**Framework**: 4Ps (Promise, Picture, Proof, Push)
**Sections**:
1. Hero with pricing promise
2. Pricing tiers (3 typically)
3. Feature comparison table
4. FAQ
5. Testimonials
6. CTA with guarantee

### Features Page
See: [pages/features.md](pages/features.md)

**Framework**: Benefits-focused with proof
**Sections**:
1. Hero with features overview
2. Individual feature sections
3. Integration highlights
4. Testimonials specific to features
5. CTA

### Demo/Trial Page
See: [pages/demo.md](pages/demo.md)

**Framework**: PAS (light) + Social Proof
**Sections**:
1. Hero with form
2. What to expect
3. Trust indicators
4. Testimonials
5. FAQ

---

## Key User Journeys

See: [journeys.md](journeys.md)

### Journey 1: Self-Serve Trial
```
[Ad/Search] → Homepage → Features → Pricing → Signup → Onboarding
```

### Journey 2: Demo Request
```
[Ad/Search] → Homepage → Case Study → Demo Page → Sales Call
```

### Journey 3: Content to Trial
```
[Blog Post] → Resources → Homepage → Pricing → Signup
```

### Journey 4: Comparison Shopper
```
[Search] → Homepage → Features → Pricing → Case Studies → Signup
```

---

## Navigation Structure

### Primary Navigation
```
Products | Solutions | Pricing | Customers | Resources | [Login] [CTA]
```

### Mega Menu Example (Products)
```
PRODUCTS                  SOLUTIONS            RESOURCES
────────                  ─────────            ─────────
Product A                 For Marketing        Blog
  Description             For Sales            Help Center
Product B                 For Support          Guides
  Description             For Enterprise       Webinars
                                               Case Studies
```

### Footer Navigation
```
PRODUCT          COMPANY         RESOURCES        LEGAL
────────         ───────         ─────────        ─────
Features         About           Blog             Privacy
Pricing          Careers         Help Center      Terms
Integrations     Press           Status           Security
What's New       Contact         Changelog        GDPR
```

---

## CTA Strategy

### Primary CTAs (High Commitment)
- "Start Free Trial"
- "Book a Demo"
- "Get Started Free"

### Secondary CTAs (Low Commitment)
- "See How It Works"
- "View Pricing"
- "Read Case Study"
- "Watch Demo Video"

### CTA Placement
- Hero: Primary + Secondary
- After feature sections: Contextual CTA
- End of page: Primary CTA block
- Sticky header: Primary CTA (optional)

---

## Trust Elements

### Types of Proof Needed

| Proof Type | Placement | Purpose |
|------------|-----------|---------|
| **Logos** | After hero, footer | Instant credibility |
| **Stats** | Homepage, pricing | Scale validation |
| **Testimonials** | Throughout | Specific results |
| **Case Studies** | Dedicated pages, embedded | Deep proof |
| **Badges** | Footer, pricing | Security/compliance |
| **Reviews** | Homepage, pricing | Third-party validation |

### Trust Hierarchy
1. Recognizable logos
2. Specific results (numbers)
3. Named testimonials with photos
4. Full case studies
5. Third-party reviews (G2, Capterra)

---

## Conversion Points

### Primary Conversions
1. Free trial signup
2. Demo request
3. Contact form submission

### Micro-Conversions
1. Newsletter signup
2. Resource download
3. Webinar registration
4. Blog subscription

### Tracking Points
- Page views by source
- CTA click-through rates
- Form start vs. completion
- Trial-to-paid conversion

---

## Mobile Considerations

- Hamburger menu for navigation
- Sticky CTA in header
- Simplified feature sections
- Touch-friendly pricing toggles
- Click-to-call on contact info

---

## SEO Pages

### High-Intent Keywords
- `/features/[feature-name]/` — Feature-specific pages
- `/solutions/[use-case]/` — Use case pages
- `/vs/[competitor]/` — Comparison pages
- `/integrations/[app]/` — Integration pages

### Content Keywords
- `/blog/[topic]/` — Thought leadership
- `/resources/[guide]/` — Lead magnets
- `/glossary/[term]/` — Definitional content

---

## Reference Sites to Study

| Company | Strength | Study For |
|---------|----------|-----------|
| **Stripe** | Clarity, docs, trust | Overall structure |
| **Linear** | Minimalism, product focus | Design system |
| **Notion** | Simplicity, demos | Onboarding flow |
| **Slack** | Social proof, use cases | Enterprise positioning |
| **HubSpot** | Content, SEO | Full funnel |
| **Intercom** | Messaging, positioning | Value communication |

---

## Implementation Checklist

### Foundation
- [ ] Core pages created (home, features, pricing, demo)
- [ ] Navigation implemented
- [ ] CTAs placed throughout
- [ ] Basic tracking in place

### Trust
- [ ] Logo cloud with 5+ logos
- [ ] At least 3 testimonials
- [ ] 1+ case study
- [ ] Security badges if applicable

### Conversion
- [ ] Trial signup flow working
- [ ] Demo request form live
- [ ] Contact form functional
- [ ] Email capture for content

### Content
- [ ] Blog with 5+ posts
- [ ] 1+ lead magnet resource
- [ ] FAQ on key pages
- [ ] Help documentation

---

*See individual page files in `pages/` for detailed blueprints of each page type.*
