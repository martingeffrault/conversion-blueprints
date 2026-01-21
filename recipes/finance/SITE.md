# Finance & Fintech Website Recipe

> **For**: Banks, credit unions, fintech apps, investment platforms, insurance, lending
> **Key Challenges**: Security perception, regulatory compliance, complex product explanation, trust building
> **Reference Sites**: Stripe, Mercury, Wise, Robinhood, Chime, Lemonade

---

## Site Architecture

### Consumer Finance (B2C)

```
/                           → Homepage
/personal/                  → Personal banking hub
├── /checking/              → Checking accounts
├── /savings/               → Savings accounts
├── /credit-cards/          → Credit card offerings
├── /loans/                 → Personal loans
├── /mortgage/              → Mortgage products
/investing/                 → Investment products
├── /brokerage/             → Trading accounts
├── /retirement/            → IRAs, 401k
├── /robo-advisor/          → Managed investing
/insurance/                 → Insurance products (if applicable)
/tools/                     → Financial tools hub
├── /calculator-loan/       → Loan calculator
├── /calculator-mortgage/   → Mortgage calculator
├── /budget-planner/        → Budgeting tool
/learn/                     → Financial education
├── /[topic]/               → Educational articles
/pricing/                   → Fees & rates
/security/                  → Security center
/about/                     → About the company
/help/                      → Help center
/login/                     → Account login
/get-started/               → Account opening
```

### Fintech / B2B Finance

```
/                           → Homepage (value prop + demo CTA)
/product/                   → Product hub
├── /[feature]/             → Feature pages
/solutions/                 → Solutions by use case
├── /[use-case]/            → Use case pages
/pricing/                   → Pricing plans
/developers/                → Developer docs (if API product)
├── /docs/                  → API documentation
├── /guides/                → Integration guides
/customers/                 → Case studies
├── /[customer]/            → Individual case studies
/resources/                 → Resource hub
├── /blog/                  → Blog
├── /guides/                → Downloadable guides
├── /webinars/              → Webinars
/company/                   → Company info
├── /about/                 → About
├── /careers/               → Careers
├── /press/                 → Press & news
/contact/                   → Contact sales
/login/                     → Dashboard login
/signup/                    → Create account
```

---

## Homepage Blueprint

### Consumer Finance Homepage

```
1. Hero
   └── Value proposition (simplicity, savings, better rates)
   └── Primary CTA: "Open Account" or "Get Started"
   └── Trust: FDIC insured, security badges

2. Products Overview
   └── Product cards (checking, savings, investing)
   └── Quick comparison of benefits
   └── "Best for" labels

3. Why Us (Differentiators)
   └── 3-4 key benefits vs traditional banks
   └── Feature comparison
   └── No hidden fees messaging

4. Trust Section
   └── Security certifications
   └── Regulatory compliance (FDIC, SEC, etc.)
   └── Company credibility

5. Social Proof
   └── Customer count
   └── App store ratings
   └── Testimonials
   └── Press mentions

6. Mobile App Showcase
   └── App screenshots
   └── Key features
   └── Download links

7. Rates & Benefits
   └── APY rates (if competitive)
   └── Fee comparison
   └── Rewards/cashback

8. Financial Tools
   └── Calculator previews
   └── Educational content teasers

9. CTA Section
   └── Account opening CTA
   └── Time to open ("5 minutes")
   └── What you'll need

10. Footer
    └── Regulatory disclosures
    └── Legal links
    └── Contact information
```

### Fintech B2B Homepage

```
1. Hero
   └── Clear value proposition
   └── Primary: Demo/Contact Sales
   └── Secondary: View pricing
   └── Credibility: Customer logos

2. Product Features
   └── Key capabilities
   └── Visual demonstrations
   └── Integration logos

3. How It Works
   └── Process visualization
   └── Integration simplicity
   └── Time-to-value messaging

4. Use Cases / Solutions
   └── Industry or use case cards
   └── Specific outcomes

5. Customer Proof
   └── Case studies with metrics
   └── Logo cloud
   └── Testimonial quotes

6. Security & Compliance
   └── Security certifications
   └── Compliance badges
   └── Audit information

7. Pricing Preview
   └── Plan overview or "Custom pricing"
   └── Link to full pricing page

8. Resources
   └── Developer docs preview
   └── Integration guides
   └── Blog/content highlights

9. CTA Section
   └── Demo request
   └── Talk to sales
   └── Self-serve signup (if available)
```

---

## Key Page Patterns

### Product Page (Consumer Finance)

**Structure for checking/savings/credit card pages**:

```
┌─────────────────────────────────────────────────────────────┐
│ HEADER with Product Navigation Submenu                      │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  [Product Badge: "No Monthly Fees"]                        │
│                                                             │
│  The Checking Account                                       │
│  That Works for You                                         │
│                                                             │
│  Earn 4.00% APY with no monthly fees, no minimums,         │
│  and instant transfers.                                     │
│                                                             │
│  [Open Account - It's Free]  [Learn More ↓]                │
│                                                             │
├─────────────────────────────────────────────────────────────┤
│ Key Benefits Grid (4 items)                                 │
│ • No monthly fees    • Free ATM network                    │
│ • Instant transfers  • FDIC insured                        │
├─────────────────────────────────────────────────────────────┤
│ Feature Deep Dive (expandable sections)                     │
│ ├── Earning interest                                       │
│ ├── ATM access                                             │
│ ├── Mobile banking                                         │
│ └── Direct deposit                                         │
├─────────────────────────────────────────────────────────────┤
│ Comparison Table                                            │
│ [Us] vs [Big Bank A] vs [Big Bank B]                       │
├─────────────────────────────────────────────────────────────┤
│ FAQ                                                         │
├─────────────────────────────────────────────────────────────┤
│ CTA: Ready to open? [Get Started] Takes 5 minutes          │
├─────────────────────────────────────────────────────────────┤
│ DISCLOSURES (Required legal text)                          │
└─────────────────────────────────────────────────────────────┘
```

### Calculator / Tool Page

Financial calculators drive significant SEO traffic.

```
┌─────────────────────────────────────────────────────────────┐
│ Mortgage Calculator                                         │
│                                                             │
│ See how much house you can afford                          │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  ┌─────────────────────┐  ┌──────────────────────────┐     │
│  │ INPUTS              │  │ RESULTS                   │     │
│  │                     │  │                          │     │
│  │ Home Price:         │  │ Monthly Payment:         │     │
│  │ [$400,000    ]      │  │ $2,147/mo               │     │
│  │                     │  │                          │     │
│  │ Down Payment:       │  │ ┌──────────────────────┐│     │
│  │ [20%] [$80,000]     │  │ │ Principal: $1,547   ││     │
│  │                     │  │ │ Interest:  $450     ││     │
│  │ Interest Rate:      │  │ │ Taxes:     $100     ││     │
│  │ [6.5%        ]      │  │ │ Insurance: $50      ││     │
│  │                     │  │ └──────────────────────┘│     │
│  │ Loan Term:          │  │                          │     │
│  │ (30yr) (15yr)       │  │ [Amortization Chart]    │     │
│  │                     │  │                          │     │
│  └─────────────────────┘  └──────────────────────────┘     │
│                                                             │
│  [Get Pre-Approved] See your real rate                     │
│                                                             │
├─────────────────────────────────────────────────────────────┤
│ How This Calculator Works (Educational content)            │
├─────────────────────────────────────────────────────────────┤
│ Related Tools: [Refinance Calculator] [Affordability]      │
└─────────────────────────────────────────────────────────────┘
```

### Security Center Page

Critical for finance — dedicated page builds trust.

```
┌─────────────────────────────────────────────────────────────┐
│ Your Security is Our Priority                               │
│                                                             │
│ Bank-grade security to protect your money                  │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│ How We Protect You:                                        │
│                                                             │
│ ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐           │
│ │ 🔐      │ │ 🛡️      │ │ 📱      │ │ 👁️      │           │
│ │ 256-bit │ │ FDIC    │ │ 2-Factor│ │ 24/7    │           │
│ │ Encrypt │ │ Insured │ │ Auth    │ │ Monitor │           │
│ └─────────┘ └─────────┘ └─────────┘ └─────────┘           │
│                                                             │
│ Certifications & Compliance:                               │
│ [SOC 2 Type II] [PCI DSS] [FDIC Member] [SIPC Protected]  │
│                                                             │
│ ─────────────────────────────────────────────────────────  │
│                                                             │
│ Security Features:                                          │
│ ├── Biometric login                                        │
│ ├── Instant card lock                                      │
│ ├── Transaction alerts                                     │
│ ├── Fraud protection                                       │
│ └── Zero liability guarantee                               │
│                                                             │
│ ─────────────────────────────────────────────────────────  │
│                                                             │
│ Security Tips (Educational)                                 │
│ FAQ (Security-related questions)                           │
│                                                             │
│ Report Suspicious Activity: [Contact Security Team]        │
└─────────────────────────────────────────────────────────────┘
```

---

## Trust & Compliance Patterns

### Required Trust Elements

| Element | Placement | Notes |
|---------|-----------|-------|
| FDIC/NCUA insurance | Header, footer, product pages | Required disclosure |
| Security certifications | Security page, footer | SOC 2, PCI DSS |
| Regulatory registrations | Footer, legal pages | SEC, FINRA, state licenses |
| Encryption badges | Forms, security page | 256-bit SSL |
| Member logos | Footer | FDIC, SIPC, etc. |

### Disclosure Requirements

Financial sites have strict disclosure requirements:

**APY Disclosures**:
```
*Annual Percentage Yield (APY) accurate as of [date].
APY may change at any time before or after account opening.
Fees may reduce earnings.
```

**Investment Disclosures**:
```
*Investing involves risk, including possible loss of principal.
Past performance does not guarantee future results.
See our [Disclosures] page for important information.
```

**Rate Comparisons**:
```
*Comparison based on [source/methodology].
Rates shown are for [specific product].
Your rate may vary based on creditworthiness.
```

### Trust Badge Placement

```
┌────────────────────────────────────────────────────────────┐
│ Footer Trust Bar                                           │
├────────────────────────────────────────────────────────────┤
│                                                            │
│ [🏦 FDIC]  [🔒 256-bit]  [🛡️ SOC 2]  [⭐ BBB A+]          │
│  Insured    Encryption    Certified    Rated              │
│                                                            │
│ Member FDIC. Equal Housing Lender. NMLS #[number]         │
│                                                            │
└────────────────────────────────────────────────────────────┘
```

---

## Account Opening Flow

### Conversion Funnel

```
INTEREST                    QUALIFY                    CONVERT
    │                          │                          │
    ▼                          ▼                          ▼
Product page              Eligibility check           Application
CTA click                 Quick questions             Full form
                          Rate quote                  Funding

OPTIMIZE:                 OPTIMIZE:                  OPTIMIZE:
• Clear value prop       • Short qualifier          • Progressive form
• Trust signals          • Soft credit check        • Save & continue
• Social proof           • Personalized rate        • Clear timeline
```

### Application Form Design

**Progressive Disclosure** (multi-step):

```
Step 1: Basic Info        Step 2: Identity          Step 3: Funding
├── Name                  ├── SSN (last 4)          ├── Initial deposit
├── Email                 ├── Date of birth         ├── Link bank account
├── Phone                 ├── Address               ├── Or deposit check
└── [Continue]            └── [Continue]            └── [Open Account]

Progress: [███░░░░░░] 2 of 3
```

**Trust Elements in Forms**:
- Security badges near sensitive fields
- "Why we need this" explanations
- Privacy assurance
- Save progress option

---

## Copywriting for Finance

### Language Principles

| Instead of | Use |
|------------|-----|
| "Application" | "Get started" |
| "Submit" | "Continue" or "Open account" |
| "Requirements" | "What you'll need" |
| "Terms and conditions" | "The details" (but still link to full T&C) |
| "Annual Percentage Yield" | "APY" with tooltip explanation |

### Headlines by Product Type

**Checking Account**:
- "Banking that puts you first"
- "The checking account that pays you"
- "No fees. No minimums. No kidding."

**Savings Account**:
- "Earn more on every dollar"
- "A savings account that actually saves"
- "Watch your money grow"

**Credit Card**:
- "Rewards on your terms"
- "The card that works as hard as you do"
- "Earn unlimited [X]% cash back"

**Investment Platform**:
- "Investing made simple"
- "Start building wealth today"
- "Invest with confidence"

---

## Mobile Experience

### Banking App Emphasis

```
┌────────────────────────────────────────────────────────────┐
│ Manage Your Money on the Go                                │
│                                                            │
│ ┌────────────────────────────────────────┐                │
│ │     [App Screenshot - Dashboard]        │                │
│ │                                        │                │
│ │     $12,456.78                        │                │
│ │     Available Balance                 │                │
│ │                                        │                │
│ │     [Transfer] [Deposit] [Pay]        │                │
│ └────────────────────────────────────────┘                │
│                                                            │
│ ⭐⭐⭐⭐⭐ 4.9 on App Store                                │
│                                                            │
│ [App Store]  [Google Play]                                │
│                                                            │
│ Key Features:                                             │
│ • Instant transfers                                       │
│ • Mobile check deposit                                    │
│ • Face ID / fingerprint login                            │
│ • Real-time notifications                                │
└────────────────────────────────────────────────────────────┘
```

### Mobile-First Considerations

| Feature | Implementation |
|---------|----------------|
| Quick actions | Prominent transfer/pay buttons |
| Biometric | Face ID/Touch ID login |
| Alerts | Push notification opt-in |
| Chat support | In-app messaging |
| Card controls | Instant lock/unlock |

---

## SEO Strategy

### High-Value Keywords

| Keyword Type | Examples | Content Type |
|--------------|----------|--------------|
| Product | "high yield savings account" | Product pages |
| Calculator | "mortgage calculator" | Tool pages |
| Rates | "CD rates today" | Rate tables (updated regularly) |
| Comparison | "[product] vs [competitor]" | Comparison pages |
| Educational | "how to build credit" | Blog/learn section |
| Local | "[product] in [state]" | Location pages |

### Content Pillars

1. **Product Content**: Account/product pages
2. **Tool Content**: Calculators, comparisons
3. **Educational Content**: Financial literacy
4. **News/Updates**: Rate changes, product updates

---

## Variants

### Neobank / Challenger Bank

**Emphasis on**:
- Mobile-first design
- Simplicity vs traditional banks
- No/low fees messaging
- Speed (instant everything)
- Modern, consumer-friendly language

**Examples**: Chime, Varo, Current

### Investment Platform

**Emphasis on**:
- Getting started ease
- Educational content
- Risk communication
- Performance visualization
- Social/community features

**Examples**: Robinhood, Wealthfront, Betterment

### Insurance (Insurtech)

**Emphasis on**:
- Quote speed
- Price transparency
- Claims simplicity
- Policy clarity
- Digital-first service

**Examples**: Lemonade, Root, Hippo

### Lending Platform

**Emphasis on**:
- Rate transparency
- Qualification process
- Speed to funding
- Use case flexibility
- Payment terms clarity

**Examples**: SoFi, Upstart, LendingClub

---

## Metrics to Track

| Metric | Target | Notes |
|--------|--------|-------|
| Account open rate | 15-25% | From product page to completion |
| Application start rate | 40%+ | Click "Get Started" |
| Application completion | 60%+ | Finish once started |
| Calculator engagement | 3+ minutes | Time on tool pages |
| Mobile app downloads | Track vs web signups | App-first metrics |
| Funded accounts | 80%+ | Actually deposited money |
| Time to first transaction | <24 hours | Engagement speed |

---

## Reference Sites

### Neobanks
- **Chime** — Consumer-friendly banking
- **Mercury** — Startup banking
- **Wise** — International transfers
- **Revolut** — Multi-currency

### Investment
- **Robinhood** — Commission-free trading
- **Wealthfront** — Robo-advisor
- **Betterment** — Goal-based investing
- **Public** — Social investing

### Lending
- **SoFi** — Multi-product fintech
- **Upstart** — AI lending
- **Rocket Mortgage** — Digital mortgage

### Insurance
- **Lemonade** — Renter's/home insurance
- **Root** — Auto insurance
- **Oscar** — Health insurance

### B2B Fintech
- **Stripe** — Payments infrastructure
- **Plaid** — Financial data
- **Brex** — Corporate cards

---

*See also: [Finance Industry Patterns](../../library/industry/finance.md) | [Trust Elements](../../library/components/trust-elements.md) | [Form Optimization](../../library/conversion/form-optimization.md)*
