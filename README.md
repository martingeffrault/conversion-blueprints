# Conversion Blueprints

A comprehensive, open-source library of conversion-focused website patterns, frameworks, and templates. Every recommendation backed by data, research, and industry benchmarks.

---

## What This Is

This repository contains two main resources:

### /library — The Knowledge Base

100+ guides covering everything you need to build websites that convert:

- **Page Blueprints** — Full structures for landing pages, product pages, homepages
- **Section Patterns** — Hero, CTA, social proof, pricing, FAQ templates
- **CRO Frameworks** — LIFT, MECLABS, AIDA, and other methodologies
- **Research Methods** — Voice of customer, competitive analysis, user testing
- **Industry Guides** — E-commerce, SaaS, healthcare, finance specifics
- **Testing Playbooks** — A/B testing, multivariate, heatmap analysis

### /recipes — Ready-to-Use Site Blueprints

Complete website recipes by industry vertical:

- **SaaS B2B** — PLG and sales-led playbooks
- **E-commerce** — DTC brands, marketplaces
- **Agency** — Creative and performance agencies
- **Healthcare** — Telehealth, medical practices
- **Finance** — Fintech B2B platforms
- **Real Estate** — Residential, luxury properties
- **Local Business** — Restaurants, service providers
- **Media** — Newsletters, content platforms
- **Affiliate** — Review sites, comparison sites

Each recipe includes page hierarchy, section assembly, and conversion strategies.

---

## Who It's For

- **Founders and marketers** building landing pages and websites
- **Product teams** optimizing conversion flows
- **Developers** implementing CRO best practices
- **Agencies** creating client deliverables
- **AI-assisted development** — clone this repo to give your AI tools conversion context

---

## Quick Start

### Browse Online

- [Library Index](library/_index.md) — Patterns, frameworks, and guides
- [Recipes Index](recipes/_index.md) — Complete site blueprints by industry

### Clone for AI Context

```bash
git clone https://github.com/martingeffrault/conversion-blueprints.git
```

Use this as a reference folder for AI coding assistants (Cursor, Claude, Copilot) to get conversion-aware recommendations.

### Download as Reference

Download the ZIP and keep it as a local reference library.

---

## Repository Structure

```
conversion-blueprints/
├── .claude/                # Claude Code integration
│   ├── commands/           # Custom slash commands
│   └── settings.json       # Claude Code config
├── CLAUDE.md               # AI context reference
├── library/                # Knowledge base
│   ├── frameworks/         # CRO methodologies (LIFT, MECLABS, PAS, AIDA)
│   ├── research/           # Customer research, competitive analysis
│   ├── testing/            # A/B testing, multivariate, heatmaps
│   ├── pages/              # Full page blueprints
│   │   ├── landing-page/
│   │   ├── homepage/
│   │   ├── product/
│   │   └── ...
│   ├── sections/           # Individual section patterns
│   │   ├── hero/
│   │   ├── cta/
│   │   ├── social-proof/
│   │   └── ...
│   ├── conversion/         # Core conversion patterns
│   ├── content/            # Copywriting, objection handling
│   ├── design-system/      # Visual hierarchy, typography
│   ├── industry/           # Vertical-specific guides
│   ├── analytics/          # Tracking, attribution
│   ├── seo/                # SEO for conversion
│   ├── accessibility/      # WCAG compliance
│   └── launch/             # Pre/post-launch checklists
│
└── recipes/                # Complete site blueprints
    ├── saas-b2b/           # PLG, sales-led
    ├── ecommerce/          # DTC, marketplace
    ├── agency/             # Creative, performance
    ├── healthcare/         # Telehealth
    ├── finance/            # Fintech B2B
    ├── real-estate/        # Residential, luxury
    ├── local-business/     # Restaurant, services
    ├── media/              # Newsletter
    └── affiliate/          # Review, comparison
```

---

## Key Benchmarks Included

| Metric | Average | Top Performers | Source |
|--------|---------|----------------|--------|
| Landing Page CVR | 6.6% | 11.4%+ | [Unbounce Q4 2024](https://unbounce.com/average-conversion-rates-landing-pages/) |
| E-commerce Product CVR | 2-3% | 4-6%+ | [Shopify](https://www.shopify.com/blog/ecommerce-conversion-rate) |
| SaaS Free Trial Signup | 2-5% | 10%+ | [First Page Sage](https://firstpagesage.com/seo-blog/saas-free-trial-conversion-rate-benchmarks/) |
| Trial to Paid CVR | 18-25% | 40%+ | [Userpilot](https://userpilot.com/blog/saas-average-conversion-rate/) |
| Form Completion | 45-66% | 75%+ | [Zuko](https://www.zuko.io/benchmarking/industry-benchmarking) |

| Optimization | Typical Impact | Source |
|--------------|----------------|--------|
| Headline changes | 10-30% lift | Industry testing data |
| CTA optimization | 5-20% lift | Industry testing data |
| Form field reduction | Up to 120% lift | [HubSpot](https://blog.hubspot.com/marketing/form-length) |
| Page speed (+1s delay) | -7% conversions | [Akamai/Cloudflare](https://www.cloudflare.com/learning/performance/more/website-performance-conversion-rates/) |

---

## Use Cases

### As AI Context

Add this repo to your AI coding assistant's context:

```
"Build the homepage following conversion-blueprints/recipes/saas-b2b/PLG.md"
"For the hero section, use patterns from conversion-blueprints/library/sections/hero/"
```

### As a Reference Library

When building a new site:

1. Pick a recipe from `recipes/` matching your vertical
2. Reference section patterns from `library/sections/`
3. Apply frameworks from `library/frameworks/`
4. Validate against benchmarks in `library/industry/`

### As a Team Resource

Share with your team as a single source of truth for conversion best practices.

---

## Claude Code Integration

This repo includes built-in commands for [Claude Code](https://claude.ai/code) users.

### Available Commands

| Command | Description | Example |
|---------|-------------|---------|
| `/audit-page` | Audit a page against best practices | `/audit-page landing-page https://example.com` |
| `/benchmark` | Get conversion benchmarks | `/benchmark saas` |
| `/checklist` | Generate a build checklist | `/checklist pricing ecommerce` |
| `/pattern` | Explain a conversion pattern | `/pattern hero` |

### Quick Start

```bash
# Clone the repo
git clone https://github.com/martingeffrault/conversion-blueprints.git
cd conversion-blueprints

# Commands are auto-available in Claude Code
/benchmark trial-to-paid
/checklist homepage saas
```

See [.claude/README.md](.claude/README.md) for full documentation.

---

## Sources

This library synthesizes research from:

- Nielsen Norman Group
- Baymard Institute
- Unbounce Conversion Benchmark Report
- VWO, Hotjar, CXL research
- Marketing Experiments / MECLABS
- Google Web Vitals documentation
- WCAG accessibility guidelines

Individual guides cite their specific sources.

---

## Contributing

Found an error? Have data to add? Contributions welcome.

- Open an issue for errors or suggestions
- Submit a PR for new content or corrections
- Share case studies or benchmarks

---

## License

MIT License. Use freely for personal and commercial projects.

---

Built for people who want their websites to actually convert.
