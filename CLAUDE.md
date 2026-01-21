# CLAUDE.md - Conversion Blueprints

> **AI Context Reference for Claude Code & AI-Assisted Development**

This file provides context for AI assistants (Claude, Cursor, Copilot, etc.) working with this repository.

---

## Repository Purpose

This is a **comprehensive, open-source knowledge base for building high-converting websites**. It contains:

- **160+ markdown documents** organized across library (knowledge base) and recipes (complete blueprints)
- **Evidence-based patterns** backed by research from Nielsen Norman Group, Baymard Institute, VWO, CXL, and other authoritative sources
- **Practical, actionable templates** for landing pages, product pages, conversion flows, and more

**Primary use case**: Provide AI coding assistants with conversion-aware context when building websites, SaaS products, landing pages, e-commerce sites, and marketing assets.

---

## Repository Structure

```
conversion-blueprints/
├── CLAUDE.md              # This file - AI context
├── README.md              # Project overview
├── library/               # Knowledge base (100+ guides)
│   ├── _index.md          # Library catalog & quick start
│   ├── frameworks/        # CRO methodologies (LIFT, MECLABS, AIDA, PAS, JTBD)
│   ├── research/          # Voice of customer, competitive analysis, personas
│   ├── testing/           # A/B testing, multivariate, heatmaps, user testing
│   ├── pages/             # Full page blueprints
│   │   ├── landing-page/  # Lead gen, product launch, event, waitlist
│   │   ├── homepage/      # Corporate, startup, portfolio
│   │   ├── product/       # E-commerce, SaaS, features
│   │   ├── content-hub/   # Blog, resource center, documentation
│   │   ├── contact/       # Contact forms, demo requests
│   │   ├── case-study/    # B2B case studies
│   │   └── interactive/   # Quizzes, calculators, configurators
│   ├── sections/          # Individual section patterns
│   │   ├── hero/          # Hero variants by page type
│   │   ├── cta/           # Call-to-action patterns
│   │   ├── social-proof/  # Testimonials, logos, reviews
│   │   ├── features/      # Feature presentation patterns
│   │   ├── pricing/       # Pricing table patterns
│   │   ├── faq/           # FAQ patterns
│   │   └── ...            # Stats, carousel, navigation, footer
│   ├── conversion/        # Core conversion patterns
│   │   ├── hero-patterns.md
│   │   ├── cta-patterns.md
│   │   ├── form-optimization.md
│   │   └── behavioral-economics.md
│   ├── content/           # Copywriting, objection handling, storytelling
│   ├── design-system/     # Visual hierarchy, typography, spacing, color
│   ├── industry/          # Vertical-specific guides (13 industries)
│   ├── analytics/         # Tracking, attribution, reporting
│   ├── seo/               # SEO for conversion
│   ├── accessibility/     # WCAG compliance, inclusive design
│   └── launch/            # Pre/post-launch checklists
│
└── recipes/               # Complete site blueprints by vertical
    ├── _index.md          # Recipe selection guide
    ├── saas-b2b/          # PLG.md, SALES-LED.md
    ├── ecommerce/         # DTC, marketplace patterns
    ├── agency/            # Creative, performance agencies
    ├── healthcare/        # Telehealth, medical practices
    ├── finance/           # Fintech B2B
    ├── real-estate/       # Residential, luxury
    ├── local-business/    # Restaurants, service providers
    ├── media/             # Newsletters, content platforms
    └── affiliate/         # Review sites, comparison sites
```

---

## Key Navigation Files

When working with this repo, start with these index files:

| File | Purpose |
|------|---------|
| `library/_index.md` | Complete library catalog with quick start paths |
| `recipes/_index.md` | Recipe selection guide by industry |
| `library/frameworks/_index.md` | CRO methodology comparison |
| `library/pages/_index.md` | All page type blueprints |
| `library/sections/_index.md` | All section patterns |
| `library/industry/_index.md` | Industry-specific guidance |

---

## How to Use This Repo in AI-Assisted Development

### For Building New Sites

```
# Prompt example:
"Build a SaaS homepage following the patterns in library/pages/homepage/startup.md
and the hero patterns in library/conversion/hero-patterns.md"
```

### For Optimizing Existing Sites

```
# Prompt example:
"Review my landing page against the checklist in library/pages/landing-page/lead-gen.md
and suggest improvements based on library/conversion/form-optimization.md"
```

### For Industry-Specific Guidance

```
# Prompt example:
"Apply the e-commerce best practices from library/industry/ecommerce.md
to my product page implementation"
```

### For Section Implementation

```
# Prompt example:
"Create a social proof section using the patterns from library/sections/social-proof/"
```

---

## Key Benchmarks (Reference)

### Conversion Rate Benchmarks

| Metric | Average | Good | Excellent | Source |
|--------|---------|------|-----------|--------|
| Landing Page CVR | 2.35% | 5.31% | 11.45%+ | Unbounce |
| E-commerce Product CVR | 1.88% | 3-5% | 8%+ | Various |
| SaaS Free Trial CVR | 1.1% | 3-5% | 10%+ | OpenView |
| Form Completion | 47% | 60% | 80%+ | Formstack |

### Optimization Impact

| Element | Typical Lift |
|---------|--------------|
| Headline changes | 10-30% |
| CTA optimization | 5-20% |
| Form field reduction | 10-30% |
| Social proof addition | 5-15% |
| Page speed improvement | 7% per second |

### User Behavior Data

| Insight | Data | Source |
|---------|------|--------|
| Above-fold attention | 80% of viewing time | Nielsen Norman Group |
| First impression decision | 50ms | Google Research |
| Mobile traffic share | 60%+ of web traffic | Statista |
| F-pattern reading | Dominant on text pages | Nielsen Norman Group |

---

## Document Standards

### Citation Format

All data claims should include sources. Format:
- Inline: "Landing pages convert at 2.35% on average ([Unbounce](https://unbounce.com/conversion-benchmark-report/))"
- Reference section at document end with full URLs

### Document Structure

Most guides follow this pattern:
1. **Overview/Purpose** - What and why
2. **Key Patterns/Frameworks** - The core content
3. **Data & Benchmarks** - Supporting evidence
4. **Implementation Checklist** - Actionable steps
5. **Sources** - Full citations

### Wireframe Format

ASCII wireframes use this style:
```
┌─────────────────────────────────────┐
│ SECTION NAME                        │
├─────────────────────────────────────┤
│ [Component description]             │
│ [Component description]             │
└─────────────────────────────────────┘
```

---

## Quality Standards

### What Makes a Good Document

1. **Sourced claims** - Every statistic has a citation
2. **Practical templates** - Copy-paste structures
3. **Visual wireframes** - ASCII diagrams showing layouts
4. **Checklists** - Implementation verification
5. **Cross-references** - Links to related documents

### Known Gaps to Address

When contributing or updating, prioritize:
- Adding sources to unsourced statistics
- Completing stub documents in recipes/
- Expanding SEO, accessibility, and content sections
- Adding more industry-specific benchmarks

---

## Authoritative Sources

This library prioritizes research from:

| Source | Domain | URL |
|--------|--------|-----|
| Nielsen Norman Group | UX Research | nngroup.com |
| Baymard Institute | E-commerce UX | baymard.com |
| CXL | Conversion Optimization | cxl.com |
| VWO | A/B Testing | vwo.com |
| Unbounce | Landing Pages | unbounce.com |
| HubSpot | Marketing | hubspot.com |
| Hotjar | Behavior Analytics | hotjar.com |
| MECLABS | Marketing Research | meclabs.com |

---

## Multi-Project Usage

This repo is designed to be:

1. **Cloned as AI context** - Add to your project's AI assistant context
2. **Referenced during development** - Browse when building sites
3. **Forked for customization** - Adapt to your specific needs
4. **Shared across teams** - Single source of truth for CRO practices

### Recommended Workflow

```bash
# Clone as submodule or reference
git clone https://github.com/martingeffrault/conversion-blueprints.git

# Reference in AI prompts
"Using conversion-blueprints/library/sections/hero/ as reference,
build a value proposition hero for my SaaS product"
```

---

## Contributing

When adding or updating content:

1. **Always cite sources** - No unsourced statistics
2. **Use consistent formatting** - Follow existing document structure
3. **Include practical examples** - Templates, wireframes, checklists
4. **Cross-reference related content** - Link to relevant documents
5. **Test recommendations** - Note if patterns are theoretical vs. tested

---

*This knowledge base is MIT licensed. Use freely for personal and commercial projects.*
