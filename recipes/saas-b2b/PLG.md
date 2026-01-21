# SaaS B2B: Product-Led Growth (PLG) Architecture

> **Model**: Self-serve acquisition, free trial/freemium, in-product conversion
> **Examples**: Notion, Slack, Figma, Calendly, Loom, Airtable
> **Characteristics**: Low friction signup, viral loops, usage-based pricing

---

## Key Differences vs Sales-Led

| Aspect | Product-Led | Sales-Led |
|--------|-------------|-----------|
| Primary CTA | "Start Free" / "Try Now" | "Book a Demo" / "Contact Sales" |
| Pricing | Transparent, self-serve | Hidden or "Contact us" |
| Conversion | In-product | Sales team |
| Homepage focus | Value prop + instant signup | Credibility + lead capture |
| Content | Help docs, templates, tutorials | Case studies, whitepapers |

---

## Site Architecture

### Core Pages

```
/                           Homepage (signup-focused)
├── /pricing/               Transparent pricing page
├── /features/              Feature overview
│   └── /features/[feature]/ Individual feature pages
├── /templates/             Template gallery (if applicable)
├── /integrations/          Integration directory
├── /customers/             Customer stories (lighter than case studies)
├── /about/                 Company story
├── /blog/                  SEO + thought leadership
├── /changelog/             Product updates (transparency)
└── /help/ or /docs/        Self-serve documentation
```

### Conversion Pages

```
├── /signup/                Free signup flow
├── /login/                 Existing user login
├── /demo/                  Optional demo for enterprise
└── /enterprise/            Enterprise tier landing page
```

### Legal

```
├── /privacy/
├── /terms/
├── /security/              Security practices (important for B2B)
└── /gdpr/ or /compliance/  Compliance info
```

---

## Homepage Structure (PLG)

```
┌─────────────────────────────────────────────────────────────────┐
│ [Logo]      Features  Pricing  Customers  Blog     [Login]      │
│                                                    [Start Free] │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│              The [category] tool that                           │
│              teams actually love                                │
│                                                                 │
│              [Brief value prop - 1 sentence]                    │
│                                                                 │
│              [Email         ] [Start Free →]                    │
│              No credit card required                            │
│                                                                 │
│              [Product Screenshot / Demo GIF]                    │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Trusted by teams at                                            │
│  [Logo] [Logo] [Logo] [Logo] [Logo] [Logo]                     │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  See how it works                                               │
│  [Product Demo Video or Interactive Preview]                    │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Why teams switch to [Product]                                  │
│                                                                 │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐             │
│  │ Fast setup  │  │ Intuitive   │  │ Affordable  │             │
│  │ 2 min to    │  │ No training │  │ Free for    │             │
│  │ first value │  │ needed      │  │ small teams │             │
│  └─────────────┘  └─────────────┘  └─────────────┘             │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Features for every workflow                                    │
│                                                                 │
│  [Feature cards with product screenshots]                       │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  "Quote from happy customer"                                    │
│  — Name, Company                                                │
│                                                                 │
│  [More stories →]                                               │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Integrates with your stack                                     │
│                                                                 │
│  [Integration logos grid]                                       │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Simple, transparent pricing                                    │
│                                                                 │
│  [Free]        [Pro]         [Team]                            │
│  $0/month      $12/month     $29/seat/mo                       │
│  [Get started] [Start trial] [Start trial]                     │
│                                                                 │
│  [Compare all plans →]                                          │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│              Ready to get started?                              │
│              [Email         ] [Start Free →]                    │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Key PLG Elements

### 1. Instant Value Path

Users should experience value within minutes:

```
Signup → Onboarding (minimal) → First Win → Habit → Upgrade
```

- Signup: Email-only or SSO (no forms)
- Onboarding: Interactive, not documentation
- First Win: Guide to key "aha moment"
- Habit: Daily/weekly use triggers
- Upgrade: In-product, usage-based prompts

### 2. Viral Loops Built-In

| Loop Type | Mechanism |
|-----------|-----------|
| **Invite** | "Invite teammate" to collaborate |
| **Share** | Shareable outputs (links, embeds) |
| **Badge** | "Made with [Product]" on outputs |
| **Social** | Share achievements, templates |

### 3. Transparent Pricing

| Element | Best Practice |
|---------|---------------|
| Free tier | Generous enough for real use |
| Clear limits | What triggers upgrade |
| No "contact us" | Self-serve purchase |
| Monthly/annual toggle | Show annual savings |

### 4. In-Product Education

Replace gated content with:
- Help docs accessible without login
- Templates library (ungated)
- Video tutorials embedded
- Community forum

---

## SEO Considerations for PLG

### High-Value Pages to Optimize

| Page Type | Target Keywords | SEO Priority |
|-----------|-----------------|--------------|
| Homepage | Brand + category | High |
| Features | "[Feature] software" | High |
| Templates | "[Use case] template" | High |
| Integrations | "[Tool] + [Tool] integration" | High |
| Comparisons | "[Competitor] alternative" | High |
| Blog | Long-tail informational | High |

### PLG-Specific SEO Patterns

**Template galleries** drive significant organic traffic:
```
/templates/
├── /templates/marketing/
├── /templates/project-management/
└── /templates/[specific-use-case]/
```

**Integration pages** capture bottom-funnel searches:
```
/integrations/slack/
/integrations/google-drive/
```

**Comparison pages** (ethical approach):
```
/compare/[competitor]/
/alternatives/[competitor]/
```

---

## Conversion Metrics (PLG)

| Metric | Benchmark | Top Performers |
|--------|-----------|----------------|
| Signup rate | 2-5% | 8%+ |
| Activation rate | 20-40% | 60%+ |
| Free-to-paid | 2-5% | 10%+ |
| Time to first value | <10 min | <2 min |
| Viral coefficient | 0.3-0.5 | 1.0+ |

---

## Sources

- [OpenView - Product-Led Growth Benchmarks](https://openviewpartners.com/product-benchmarks/)
- [ProductLed - PLG Playbook](https://productled.com/)
- [Lenny's Newsletter - PLG research](https://www.lennysnewsletter.com/)
- [First Round Review - PLG case studies](https://review.firstround.com/)
