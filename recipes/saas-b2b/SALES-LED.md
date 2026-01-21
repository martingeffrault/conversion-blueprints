# SaaS B2B: Sales-Led Architecture

> **Model**: Enterprise sales, demo-driven, high-touch conversion
> **Examples**: Salesforce, Workday, ServiceNow, HubSpot Enterprise, Marketo
> **Characteristics**: Complex products, long sales cycles, high ACV

---

## Key Differences vs Product-Led

| Aspect | Sales-Led | Product-Led |
|--------|-----------|-------------|
| Primary CTA | "Book a Demo" / "Talk to Sales" | "Start Free" |
| Pricing | Custom / "Contact us" | Transparent, self-serve |
| Conversion | Sales team closes | Self-serve in-product |
| Homepage focus | Build trust, capture leads | Show product, instant signup |
| Content | ROI calculators, case studies | Templates, tutorials |
| Sales cycle | Weeks to months | Minutes to days |

---

## Site Architecture

### Core Pages

```
/                           Homepage (credibility-focused)
├── /platform/              Platform overview
│   └── /platform/[module]/ Individual modules/products
├── /solutions/             Solutions by use case/industry
│   ├── /solutions/[use-case]/
│   └── /solutions/[industry]/
├── /customers/             Customer success stories
│   └── /customers/[case-study]/
├── /resources/             Content hub
│   ├── /resources/guides/
│   ├── /resources/whitepapers/
│   ├── /resources/webinars/
│   └── /resources/reports/
├── /blog/                  Thought leadership
├── /about/                 Company credibility
│   ├── /about/leadership/
│   ├── /about/careers/
│   └── /about/partners/
└── /contact/               Contact options
```

### Conversion Pages

```
├── /demo/                  Demo request (primary CTA)
├── /pricing/               Pricing overview (may require contact)
├── /free-trial/            Guided trial (optional)
├── /roi-calculator/        Business case tool
└── /contact-sales/         Sales contact form
```

### Trust & Compliance

```
├── /security/              Security & compliance
├── /trust/                 Trust center
├── /privacy/
├── /terms/
└── /sla/                   Service level agreements
```

---

## Homepage Structure (Sales-Led)

```
┌─────────────────────────────────────────────────────────────────┐
│ [Logo]   Platform ▼  Solutions ▼  Customers  Resources  Pricing │
│                                                   [Book a Demo] │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│              The Enterprise Platform for                        │
│              [Outcome/Category]                                 │
│                                                                 │
│              [2-3 sentence value prop emphasizing               │
│               enterprise-grade, security, scale]                │
│                                                                 │
│              [Book a Demo]    [Watch Overview]                  │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Trusted by industry leaders                                    │
│                                                                 │
│  [Fortune 500 Logo] [Logo] [Logo] [Logo] [Logo] [Logo]         │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Why Leaders Choose [Product]                                   │
│                                                                 │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐             │
│  │ Enterprise  │  │ Proven      │  │ Dedicated   │             │
│  │ Security    │  │ at Scale    │  │ Support     │             │
│  │             │  │             │  │             │             │
│  │ SOC2, GDPR, │  │ Used by 500+│  │ 24/7 with   │             │
│  │ HIPAA ready │  │ enterprises │  │ named CSM   │             │
│  └─────────────┘  └─────────────┘  └─────────────┘             │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Complete Platform                                              │
│                                                                 │
│  [Module 1]    [Module 2]    [Module 3]    [Module 4]          │
│  [Icon]        [Icon]        [Icon]        [Icon]              │
│  Description   Description   Description   Description         │
│  [Learn more]  [Learn more]  [Learn more]  [Learn more]        │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Solutions for Your Industry                                    │
│                                                                 │
│  [Financial Services] [Healthcare] [Retail] [Manufacturing]    │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Customer Success Story                                         │
│                                                                 │
│  ┌──────────────────────────────────────────────────────────┐  │
│  │                                                          │  │
│  │  "Quote about transformation and ROI achieved"           │  │
│  │                                                          │  │
│  │  — Executive Name, Title, [Company Logo]                 │  │
│  │                                                          │  │
│  │  +40% efficiency  │  $2M saved  │  6 month ROI          │  │
│  │                                                          │  │
│  │  [Read Full Story]                                       │  │
│  │                                                          │  │
│  └──────────────────────────────────────────────────────────┘  │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  The Results Speak for Themselves                               │
│                                                                 │
│     500+          $50B+          99.99%         4.8/5          │
│     Enterprise    Revenue        Uptime         G2 Rating      │
│     Customers     Managed        Guaranteed                    │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Recognition & Certifications                                   │
│                                                                 │
│  [Gartner Leader] [G2 Leader] [SOC2] [GDPR] [ISO 27001]        │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Latest Resources                                               │
│                                                                 │
│  [Whitepaper]    [Case Study]    [Webinar]                     │
│  [Title]         [Title]         [Title]                       │
│  [Download]      [Read]          [Watch]                       │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│              See [Product] in Action                            │
│                                                                 │
│              Get a personalized demo tailored to                │
│              your business needs.                               │
│                                                                 │
│              [Book Your Demo]                                   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Key Sales-Led Elements

### 1. Multi-Touch Lead Capture

Multiple conversion points for different buyer stages:

| Stage | Offer | Form Fields |
|-------|-------|-------------|
| Early | Whitepaper, guide | Email only |
| Mid | Webinar, ROI calculator | Email, company, role |
| Late | Demo, pricing | Full qualification form |

### 2. Solution-Based Navigation

Organize by buyer need, not product features:

```
Solutions →
├── By Use Case
│   ├── Sales Automation
│   ├── Customer Service
│   └── Marketing Operations
│
└── By Industry
    ├── Financial Services
    ├── Healthcare
    └── Retail
```

### 3. Case Studies with ROI

Enterprise buyers need proof of ROI:

```
┌─────────────────────────────────────────┐
│ [Customer Logo]                         │
│                                         │
│ How [Customer] Achieved [Outcome]       │
│                                         │
│ Challenge → Solution → Results          │
│                                         │
│ +40% efficiency | $2M saved | 6mo ROI  │
│                                         │
│ [Read Case Study] [Watch Video]         │
└─────────────────────────────────────────┘
```

### 4. Trust Center

Enterprise-grade security page:

| Section | Content |
|---------|---------|
| Security | Architecture, encryption, access controls |
| Compliance | SOC2, GDPR, HIPAA, ISO certifications |
| Privacy | Data handling, DPA template |
| Reliability | Uptime SLA, disaster recovery |
| Penetration tests | Third-party audit reports |

---

## SEO Considerations for Sales-Led

### Different SEO Strategy

Sales-led SaaS often has **lower SEO priority** for commercial pages because:
- Buyers often know the brand (branded search)
- Long sales cycles mean attribution is complex
- Competitor comparisons can be risky for enterprise

### Where SEO Matters

| Page Type | SEO Value | Strategy |
|-----------|-----------|----------|
| Blog | High | Thought leadership, top-of-funnel |
| Resources | High | Gated but indexed guides |
| Solutions pages | Medium | Industry/use case keywords |
| Homepage | Medium | Brand + category |
| Product pages | Low | Often too technical |
| Pricing | Low | Usually "custom pricing" |

### Content Marketing Focus

Sales-led benefits more from:
- **Original research** (State of [Industry] reports)
- **Expert content** (Executive interviews, podcasts)
- **Analyst relations** (Gartner, Forrester mentions)
- **Industry events** (Webinars, conference talks)

---

## Lead Qualification

### Form Strategy

**Demo request form** (high intent):
```
- Work email* (validates company)
- Company name*
- Job title*
- Company size*
- Primary challenge/use case*
- Timeline (optional)
- Additional context (optional)
```

**Whitepaper form** (low intent):
```
- Work email*
- (Progressive profiling adds more later)
```

### Lead Scoring Signals

| Signal | Weight |
|--------|--------|
| Company size (enterprise) | High |
| Job title (decision maker) | High |
| Demo request | High |
| Multiple page views | Medium |
| Pricing page visit | Medium |
| Whitepaper download | Low |

---

## Conversion Metrics (Sales-Led)

| Metric | Benchmark | Notes |
|--------|-----------|-------|
| MQL to SQL | 15-25% | Marketing qualified to sales qualified |
| SQL to opportunity | 30-40% | Sales accepts as real opportunity |
| Opportunity to close | 20-30% | Closed won rate |
| Sales cycle length | 3-9 months | Varies by ACV |
| CAC payback | 12-18 months | Time to recover acquisition cost |

---

## Sources

- [Gartner - B2B Buying Journey](https://www.gartner.com/en/sales/insights/b2b-buying-journey)
- [Forrester - B2B Marketing](https://www.forrester.com/b2b-marketing/)
- [HubSpot - Enterprise Sales](https://blog.hubspot.com/sales)
- [SaaStr - Enterprise SaaS benchmarks](https://www.saastr.com/)
- [OpenView - SaaS Benchmarks](https://openviewpartners.com/product-benchmarks/)
