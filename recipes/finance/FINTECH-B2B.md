# Fintech B2B Recipe

> **For**: Payment processors, banking-as-a-service, financial infrastructure, enterprise financial software
> **Key Challenges**: Technical credibility, security/compliance, complex integrations, enterprise sales
> **Reference Sites**: Stripe, Plaid, Marqeta, Adyen, Column, Modern Treasury

---

## Site Architecture

```
/                           → Homepage
/products/                  → Products hub
├── /payments/              → Payment processing
├── /banking/               → Banking infrastructure
├── /treasury/              → Treasury management
├── /[product]/             → Individual products
/solutions/                 → Solutions by vertical
├── /saas/                  → SaaS platforms
├── /marketplaces/          → Marketplaces
├── /ecommerce/             → E-commerce
├── /fintech/               → Fintech companies
├── /enterprise/            → Enterprise
/developers/                → Developer hub
├── /docs/                  → API documentation
├── /reference/             → API reference
├── /guides/                → Integration guides
├── /sdks/                  → SDKs & libraries
├── /changelog/             → API changelog
/pricing/                   → Pricing page
/customers/                 → Case studies hub
├── /[customer]/            → Individual studies
/resources/                 → Resources hub
├── /blog/                  → Engineering blog
├── /guides/                → Whitepapers
├── /webinars/              → Events
/company/                   → Company hub
├── /about/                 → About us
├── /careers/               → Careers
├── /press/                 → Press room
├── /security/              → Security center
/contact/                   → Contact sales
/login/                     → Dashboard
/signup/                    → Get started
```

---

## Homepage Blueprint

### Section Order (Stripe-Style)

```
1. Hero
   └── Technical value proposition
   └── Code snippet preview (optional)
   └── Primary: Start building / Get Started
   └── Secondary: Contact sales

2. Customer Logos
   └── High-profile logos
   └── "Powers X% of internet commerce" or similar

3. Product Overview
   └── Product cards with icons
   └── Technical benefits
   └── Links to individual product pages

4. Code / Integration Preview
   └── Code snippets showing simplicity
   └── "Get started in minutes" messaging
   └── Language/framework tabs

5. Solutions by Use Case
   └── Industry/use case cards
   └── Specific outcomes
   └── Links to solution pages

6. Case Studies Preview
   └── 2-3 headline case studies
   └── Metrics/results
   └── Company logos

7. Developer Experience
   └── Documentation preview
   └── SDKs available
   └── Developer testimonials

8. Security & Compliance
   └── Certification badges
   └── Compliance coverage
   └── Link to security center

9. Pricing Preview
   └── Starting pricing or "Pay as you go"
   └── Link to full pricing

10. CTA Section
    └── Start building (self-serve)
    └── Talk to sales (enterprise)
```

### Hero Pattern (Technical Product)

```
┌────────────────────────────────────────────────────────────────┐
│ HEADER: Logo | Products | Solutions | Developers | Pricing | Login │
├────────────────────────────────────────────────────────────────┤
│                                                                │
│  Financial infrastructure                                      │
│  for the internet                                              │
│                                                                │
│  Millions of companies use [Company] to accept payments,      │
│  send payouts, and manage their businesses online.            │
│                                                                │
│  [Start now →]  [Contact sales]                               │
│                                                                │
│  ┌────────────────────────────────────────────────┐          │
│  │ // Accept a payment in minutes                 │          │
│  │                                                │          │
│  │ const payment = await company.payments.create({│          │
│  │   amount: 2000,                               │          │
│  │   currency: 'usd',                            │          │
│  │   source: 'tok_visa',                         │          │
│  │ });                                           │          │
│  │                                                │          │
│  │ [Node] [Python] [Ruby] [Go] [Java]            │          │
│  └────────────────────────────────────────────────┘          │
│                                                                │
├────────────────────────────────────────────────────────────────┤
│ [Amazon] [Shopify] [Lyft] [Zoom] [Slack] +thousands more      │
└────────────────────────────────────────────────────────────────┘
```

---

## Key Page Patterns

### Product Page

**Structure for technical products**:

```
┌────────────────────────────────────────────────────────────────┐
│ [Payments]                                                     │
│                                                                │
│ Accept payments globally                                       │
│                                                                │
│ A fully integrated suite of payments products that let you    │
│ accept credit cards, mobile wallets, and local payment        │
│ methods from customers anywhere in the world.                 │
│                                                                │
│ [Get started]  [View docs →]                                  │
├────────────────────────────────────────────────────────────────┤
│ ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐       │
│ │ 135+     │  │ 99.99%   │  │ 195+     │  │ 3.5B     │       │
│ │ Currencies│  │ Uptime   │  │ Countries│  │ API calls│       │
│ └──────────┘  └──────────┘  └──────────┘  └──────────┘       │
├────────────────────────────────────────────────────────────────┤
│ Key Capabilities                                               │
│                                                                │
│ ├── Online payments                                           │
│ │   └── Cards, wallets, bank transfers                       │
│ ├── Invoicing                                                 │
│ │   └── Hosted invoices with payment links                   │
│ ├── Subscriptions                                             │
│ │   └── Recurring billing automation                         │
│ └── Fraud prevention                                          │
│     └── ML-powered risk assessment                           │
├────────────────────────────────────────────────────────────────┤
│ Technical Deep Dive                                            │
│                                                                │
│ [Code examples] [Architecture diagrams] [Integration flow]    │
├────────────────────────────────────────────────────────────────┤
│ Customer Stories                                               │
│ "We reduced checkout abandonment by 25%" — [Customer]         │
├────────────────────────────────────────────────────────────────┤
│ Pricing                                                        │
│ 2.9% + 30¢ per successful card charge                        │
│ [See all pricing →]                                           │
├────────────────────────────────────────────────────────────────┤
│ Related Products                                               │
│ [Billing] [Radar] [Connect]                                   │
└────────────────────────────────────────────────────────────────┘
```

### Developer Documentation Hub

```
┌────────────────────────────────────────────────────────────────┐
│ DEVELOPERS                                                     │
├────────────────────────────────────────────────────────────────┤
│                                                                │
│ Build with [Company]                                           │
│                                                                │
│ ┌──────────────┐  ┌──────────────┐  ┌──────────────┐         │
│ │ 📚 Docs     │  │ 🔧 API       │  │ 📦 SDKs     │         │
│ │ Start here  │  │ Reference    │  │ Libraries   │         │
│ └──────────────┘  └──────────────┘  └──────────────┘         │
│                                                                │
│ Quick Start Guides:                                           │
│ [Accept a payment] [Set up webhooks] [Test mode] [Go live]    │
│                                                                │
├────────────────────────────────────────────────────────────────┤
│ Popular Tutorials                                              │
│                                                                │
│ • Build a checkout page (15 min)                              │
│ • Add subscription billing (20 min)                           │
│ • Handle webhooks (10 min)                                    │
│ • Integrate with React (15 min)                               │
│                                                                │
├────────────────────────────────────────────────────────────────┤
│ Available SDKs                                                 │
│                                                                │
│ [Node.js] [Python] [Ruby] [Go] [PHP] [Java] [.NET] [iOS]     │
│                                                                │
├────────────────────────────────────────────────────────────────┤
│ Developer Resources                                            │
│                                                                │
│ • API Status: [status.company.com]                            │
│ • Changelog: [Recent updates]                                 │
│ • Support: [Discord] [GitHub] [Stack Overflow]               │
│                                                                │
└────────────────────────────────────────────────────────────────┘
```

### Pricing Page (Usage-Based)

```
┌────────────────────────────────────────────────────────────────┐
│ Simple, transparent pricing                                    │
│                                                                │
│ Pay only for what you use. No setup fees, no monthly fees.   │
├────────────────────────────────────────────────────────────────┤
│                                                                │
│ INTEGRATED                                                     │
│ ────────────────────────────────────                          │
│ For platforms and marketplaces                                │
│                                                                │
│ 2.9% + 30¢                                                    │
│ per successful card charge                                    │
│                                                                │
│ + 0.5% for international cards                                │
│ + 1% if currency conversion required                          │
│                                                                │
│ Includes:                                                      │
│ ✓ Accept all major cards                                      │
│ ✓ Mobile wallets (Apple Pay, Google Pay)                     │
│ ✓ Fraud protection                                            │
│ ✓ 24/7 support                                                │
│                                                                │
│ [Get started]                                                  │
│                                                                │
├────────────────────────────────────────────────────────────────┤
│                                                                │
│ CUSTOMIZED                                                     │
│ ────────────────────────────────────                          │
│ For large or unique business models                           │
│                                                                │
│ Volume discounts                                               │
│ Custom integration support                                     │
│ Dedicated account management                                   │
│ SLA guarantees                                                 │
│                                                                │
│ [Contact sales]                                                │
│                                                                │
├────────────────────────────────────────────────────────────────┤
│ All prices shown in USD. See full pricing for all products.  │
│                                                                │
│ Additional products:                                          │
│ • Billing: 0.5% of recurring revenue                          │
│ • Connect: 0.25% + per-payout fees                           │
│ • Radar: $0.02 per screened transaction                      │
│                                                                │
│ [See detailed pricing →]                                      │
└────────────────────────────────────────────────────────────────┘
```

---

## Security & Compliance Section

Critical for fintech B2B — buyers need assurance.

### Security Center Page

```
┌────────────────────────────────────────────────────────────────┐
│ Security at [Company]                                          │
│                                                                │
│ Built with security at the core                               │
├────────────────────────────────────────────────────────────────┤
│                                                                │
│ Certifications & Compliance:                                   │
│                                                                │
│ ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐ │
│ │ PCI DSS │ │ SOC 2   │ │ SOC 1   │ │ GDPR    │ │ ISO     │ │
│ │ Level 1 │ │ Type II │ │ Type II │ │ Ready   │ │ 27001   │ │
│ └─────────┘ └─────────┘ └─────────┘ └─────────┘ └─────────┘ │
│                                                                │
├────────────────────────────────────────────────────────────────┤
│ How we protect your data:                                      │
│                                                                │
│ 🔐 Encryption                                                  │
│    All data encrypted at rest (AES-256) and in transit (TLS) │
│                                                                │
│ 🔒 Access Control                                              │
│    Role-based access, MFA required for all employees          │
│                                                                │
│ 🛡️ Infrastructure                                             │
│    SOC 2 certified data centers, regular penetration testing  │
│                                                                │
│ 📊 Monitoring                                                  │
│    24/7 security monitoring and incident response             │
│                                                                │
├────────────────────────────────────────────────────────────────┤
│ Security Resources                                             │
│                                                                │
│ [Download SOC 2 Report] [View Security Whitepaper]           │
│ [Bug Bounty Program] [Responsible Disclosure]                 │
│                                                                │
├────────────────────────────────────────────────────────────────┤
│ Questions about security?                                      │
│ Contact our security team: security@company.com               │
└────────────────────────────────────────────────────────────────┘
```

---

## Case Study Format

### B2B Case Study Structure

```
┌────────────────────────────────────────────────────────────────┐
│ [Company Logo]                                                 │
│                                                                │
│ How [Customer] increased conversion by 25%                    │
│ with [Company] Payments                                        │
│                                                                │
│ Industry: E-commerce                                          │
│ Products: Payments, Billing, Connect                          │
│                                                                │
├────────────────────────────────────────────────────────────────┤
│ THE CHALLENGE                                                  │
│ ──────────────────────────────────────────────                │
│ [2-3 paragraphs on their problem]                             │
│                                                                │
├────────────────────────────────────────────────────────────────┤
│ THE SOLUTION                                                   │
│ ──────────────────────────────────────────────                │
│ [How they implemented your product]                           │
│                                                                │
├────────────────────────────────────────────────────────────────┤
│ THE RESULTS                                                    │
│ ──────────────────────────────────────────────                │
│ ┌───────────────┐ ┌───────────────┐ ┌───────────────┐        │
│ │ 25%           │ │ 2 weeks       │ │ $2M           │        │
│ │ conversion    │ │ to            │ │ annual        │        │
│ │ increase      │ │ integrate     │ │ savings       │        │
│ └───────────────┘ └───────────────┘ └───────────────┘        │
│                                                                │
│ [Full case study details...]                                  │
│                                                                │
├────────────────────────────────────────────────────────────────┤
│ "Quote from customer about the experience"                    │
│ — Name, Title at Company                                      │
│                                                                │
├────────────────────────────────────────────────────────────────┤
│ Ready to get similar results?                                 │
│ [Get started] [Contact sales]                                 │
└────────────────────────────────────────────────────────────────┘
```

---

## Developer Experience Patterns

### API Reference Structure

```
/developers/docs/
├── Getting Started
│   ├── Quick start
│   ├── Authentication
│   ├── Test mode
│   └── Going live
├── Core Concepts
│   ├── API overview
│   ├── Idempotency
│   ├── Pagination
│   └── Error handling
├── Guides
│   ├── Accept a payment
│   ├── Refunds
│   ├── Subscriptions
│   └── Webhooks
├── API Reference
│   ├── [Resource 1]
│   ├── [Resource 2]
│   └── ...
└── Resources
    ├── SDKs
    ├── Changelog
    └── Support
```

### Code Sample Pattern

```
┌────────────────────────────────────────────────────────────────┐
│ Accept a payment                                               │
│                                                                │
│ [Node.js ▼] [Python] [Ruby] [Go] [curl]                       │
├────────────────────────────────────────────────────────────────┤
│                                                                │
│  1  const company = require('company');                       │
│  2                                                             │
│  3  const paymentIntent = await company.paymentIntents.create({│
│  4    amount: 2000,                                           │
│  5    currency: 'usd',                                        │
│  6    payment_method_types: ['card'],                         │
│  7  });                                                        │
│  8                                                             │
│  9  // Returns the client secret for frontend confirmation    │
│ 10  return paymentIntent.client_secret;                       │
│                                                                │
│ [Copy code] [Run in test mode]                                │
├────────────────────────────────────────────────────────────────┤
│ Response:                                                      │
│ {                                                             │
│   "id": "pi_1234567890",                                      │
│   "object": "payment_intent",                                 │
│   "amount": 2000,                                             │
│   "status": "requires_payment_method"                         │
│ }                                                             │
└────────────────────────────────────────────────────────────────┘
```

---

## Enterprise Sales Patterns

### Contact Sales Flow

```
Interest                    Qualify                     Engage
    │                          │                          │
    ▼                          ▼                          ▼
Request demo             Form completion            Sales outreach
Contact sales            Lead enrichment            Demo scheduling
                         Volume qualification

FORM FIELDS:                                        NEXT STEPS:
• Company name                                      • SDR qualification
• Work email                                        • Demo scheduling
• Company size                                      • Technical discovery
• Volume estimate
• Use case
```

### Enterprise vs Self-Serve Path

```
┌─────────────────────────────────────────────────────────────────┐
│ Get started with [Company]                                      │
│                                                                 │
│ ┌──────────────────────────┐  ┌──────────────────────────┐    │
│ │                          │  │                          │    │
│ │ START BUILDING           │  │ TALK TO SALES            │    │
│ │                          │  │                          │    │
│ │ Create an account and    │  │ For custom pricing,      │    │
│ │ start integrating in     │  │ volume discounts, and    │    │
│ │ minutes. Free to start.  │  │ enterprise support.      │    │
│ │                          │  │                          │    │
│ │ [Create account →]       │  │ [Contact sales →]        │    │
│ │                          │  │                          │    │
│ └──────────────────────────┘  └──────────────────────────┘    │
│                                                                 │
│ Not sure which is right?                                       │
│ See our [pricing page] or [chat with us].                     │
└─────────────────────────────────────────────────────────────────┘
```

---

## Metrics to Track

| Metric | Target | Notes |
|--------|--------|-------|
| Developer signups | Track volume | Self-serve funnel |
| Time to first API call | <30 min | Developer experience |
| Documentation engagement | Track paths | Content optimization |
| Demo requests | Conversion rate | Enterprise funnel |
| MQL to SQL | >30% | Lead quality |
| Integration completion | >60% | Product stickiness |
| Developer NPS | >50 | Experience satisfaction |
| Docs search (no results) | <5% | Content gaps |

---

## Reference Sites

### Payments Infrastructure
- **Stripe** — The standard for developer experience
- **Adyen** — Enterprise payments
- **Plaid** — Financial data

### Banking Infrastructure
- **Column** — Bank infrastructure
- **Modern Treasury** — Payment operations
- **Unit** — Banking-as-a-service

### Enterprise Financial
- **Brex** — Corporate cards
- **Ramp** — Spend management
- **Mercury** — Startup banking

---

*See also: [Finance Recipe](./SITE.md) | [B2B Enterprise Patterns](../../library/industry/b2b-enterprise.md) | [Pricing Patterns](../../library/conversion/pricing-patterns.md)*
