# Recipes: Complete Website Blueprints

> **Purpose**: Recipes are curated combinations of page blueprints, optimized for specific business types. Use them as starting points for new projects.

---

## How Recipes Work

A recipe provides:
1. **Site architecture** — Which pages you need
2. **Page structures** — Section order for each page
3. **User journeys** — How visitors flow through the site
4. **Framework recommendations** — Which copywriting frameworks to use
5. **Reference examples** — Real-world sites to study

---

## Available Recipes

### B2B / SaaS

| Recipe | Description | Use When |
|--------|-------------|----------|
| [saas-b2b/](saas-b2b/) | Full SaaS website | Selling software to businesses |

### E-commerce

| Recipe | Description | Use When |
|--------|-------------|----------|
| [ecommerce/](ecommerce/) | Online store | Selling physical or digital products |

### Content / Publishing

| Recipe | Description | Use When |
|--------|-------------|----------|
| [affiliate/](affiliate/) | Review/comparison site | Affiliate marketing, product reviews |

### Services

| Recipe | Description | Use When |
|--------|-------------|----------|
| [agency/](agency/) | Agency/portfolio site | Selling services, showcasing work |
| [local-business/](local-business/) | Local service business | Location-based services |

### Industry-Specific

| Recipe | Description | Use When |
|--------|-------------|----------|
| [real-estate/](real-estate/) | Real estate website | Property listings, agents |
| [healthcare/](healthcare/) | Healthcare & medical | Medical practices, telehealth |
| [finance/](finance/) | Finance & fintech | Banks, fintech, lending, insurance |
| [media/](media/) | Media & publishing | News, blogs, newsletters |

---

## Recipe Selection Guide

### What Are You Building?

```
START: What's your business model?
│
├─► Selling software (SaaS)
│   └─► saas-b2b/
│
├─► Selling products
│   ├─► Physical products → ecommerce/
│   └─► Digital products → ecommerce/ or saas-b2b/
│
├─► Monetizing content
│   ├─► Affiliate revenue → affiliate/
│   ├─► Ads/subscriptions → media/
│   └─► Newsletter business → media/NEWSLETTER.md
│
├─► Selling services
│   ├─► B2B services → agency/
│   └─► Local services → local-business/
│
├─► Financial services
│   ├─► Consumer banking → finance/
│   ├─► B2B fintech → finance/FINTECH-B2B.md
│   └─► Lending/insurance → finance/
│
├─► Healthcare
│   ├─► Medical practice → healthcare/
│   └─► Telehealth platform → healthcare/TELEHEALTH.md
│
└─► Other industry-specific
    └─► Real estate → real-estate/
```

---

## Recipe Structure

Each recipe folder contains:

```
recipes/[business-type]/
├── SITE.md              # Overall site architecture
├── pages/
│   ├── homepage.md      # Homepage blueprint
│   ├── product.md       # Product/service page (if applicable)
│   ├── pricing.md       # Pricing page (if applicable)
│   └── [other-pages].md # Other pages specific to this type
├── journeys.md          # Key user journeys
└── references.md        # Sites to study
```

---

## How to Use a Recipe

### Step 1: Review Site Architecture
Read `SITE.md` to understand the complete site structure.

### Step 2: Understand User Journeys
Read `journeys.md` to see how visitors should flow through your site.

### Step 3: Build Pages
Use the individual page blueprints in `pages/` as templates.

### Step 4: Study References
Look at `references.md` for real-world inspiration.

### Step 5: Customize
Adapt the recipe to your specific brand, audience, and offerings.

---

## Recipes vs. Library

| Recipes | Library |
|---------|---------|
| Complete solutions | Building blocks |
| Business-specific | Universal patterns |
| Prescriptive | Educational |
| "Follow this structure" | "Choose what you need" |

**Use recipes when**: You want a proven starting point
**Use library when**: You need to understand options or build custom pages

---

## Customization Guidelines

Recipes are starting points, not rigid rules. Customize based on:

1. **Audience sophistication** — More aware audiences need less education
2. **Price point** — Higher prices need longer, more detailed pages
3. **Competition** — Differentiate from what competitors are doing
4. **Brand voice** — Adapt tone and style to your brand
5. **Offer complexity** — Simpler offers need simpler pages

---

## Contributing New Recipes

When creating a new recipe:

1. Include all standard files (SITE.md, pages/, journeys.md, references.md)
2. Reference library blueprints where applicable
3. Include 3-5 real-world reference sites
4. Document key conversion points
5. Note any industry-specific considerations

---

*See individual recipe folders for complete business-specific blueprints.*
