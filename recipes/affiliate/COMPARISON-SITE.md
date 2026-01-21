# Comparison & Tool Site Recipe

> **Variant Focus**: Interactive tools, data comparisons, decision-making aids
> **Examples**: PC Part Picker, NerdWallet, Bankrate, Compare the Market, Finder
> **Key Differentiator**: Interactive tools, comprehensive data, comparison functionality
> **Revenue Model**: Affiliate commissions, lead generation, premium features
> **SEO Focus**: High-volume transactional queries, tool-based content

---

## How This Differs from Review Site

| Aspect | Review Site | Comparison/Tool Site |
|--------|-------------|---------------------|
| Primary content | Long-form reviews | Tools, calculators, tables |
| Data source | Hands-on testing | Aggregated/updated data |
| User intent | "Which is best?" | "Compare these options" |
| Interaction | Read articles | Use tools, filter, compare |
| Updates | Periodic testing | Real-time or frequent |
| Scale | Selective products | Comprehensive database |

---

## Site Architecture

### Core Pages

```
/                           Homepage (tool/search focused)
├── /[category]/            Category landing pages
│   └── /[category]/[product]/  Product profile pages
├── /compare/               Comparison tool
│   └── /compare/[a]-vs-[b]/    Generated comparison pages
├── /calculator/            Calculators hub
│   └── /calculator/[type]/     Individual calculators
├── /best/                  Curated recommendations
│   └── /best/[product-type]/
├── /guides/                Educational content
├── /about/                 About, methodology
└── /[legal]/               Privacy, terms, disclosure
```

### Tool-Centric Architecture

```
                        ┌─────────────┐
                        │  HOMEPAGE   │
                        └──────┬──────┘
                               │
     ┌─────────────────────────┼─────────────────────────┐
     │                         │                         │
┌────▼────┐              ┌────▼────┐              ┌────▼────┐
│ COMPARE │              │CALCULATE│              │ BROWSE  │
│  TOOL   │              │  TOOLS  │              │PRODUCTS │
└────┬────┘              └────┬────┘              └────┬────┘
     │                        │                        │
┌────┴────┐              ┌────┴────┐              ┌────┴────┐
│ A vs B  │              │ Budget  │              │Category │
│ pages   │              │ ROI     │              │ Hubs    │
└─────────┘              │ Savings │              └────┬────┘
                         └─────────┘                   │
                                                  ┌────┴────┐
                                                  │ Product │
                                                  │ Pages   │
                                                  └─────────┘
```

---

## Homepage: Tool-First

### Pattern 1: Search/Compare First

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Logo]   Products ▼   Compare   Calculators   Guides  [Login] │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│            Compare [Products] in Seconds                        │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │                                                         │   │
│  │  [Search or select product 1]  vs  [Search product 2]  │   │
│  │                                                         │   │
│  │                    [Compare Now]                        │   │
│  │                                                         │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  Popular comparisons:                                           │
│  [A vs B] [C vs D] [E vs F] [G vs H]                           │
│                                                                 │
│  ─────────────────────────────────────────────────────────────  │
│                                                                 │
│  [X] products in database    Updated [frequency]                │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Pattern 2: Calculator-First (Finance)

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│          Find the Best [Product] for Your Needs                 │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │                                                         │   │
│  │  How much are you looking to [action]?                  │   │
│  │                                                         │   │
│  │  [ $_________________ ]                                 │   │
│  │                                                         │   │
│  │  What's your timeline?                                  │   │
│  │                                                         │   │
│  │  [1 year ▼]                                             │   │
│  │                                                         │   │
│  │  [Show Me Options]                                      │   │
│  │                                                         │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  Or explore by category:                                        │
│  [Category 1] [Category 2] [Category 3] [Category 4]           │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Comparison Tool

### Interactive Comparison Builder

The core value proposition:

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Compare [Products]                                             │
│                                                                 │
│  ┌───────────────┐  ┌───────────────┐  ┌───────────────┐       │
│  │  [Product 1]  │  │  [Product 2]  │  │  + Add       │       │
│  │  [Change ×]   │  │  [Change ×]   │  │    Product   │       │
│  └───────────────┘  └───────────────┘  └───────────────┘       │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Quick Summary                                                  │
│                                                                 │
│                    Product 1      Product 2                     │
│  ─────────────────────────────────────────────────────────────  │
│  Price              $XXX           $XXX                        │
│  Overall Score      8.5/10         7.9/10                      │
│  Best For           [Use case]     [Use case]                  │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Detailed Comparison                                            │
│                                                                 │
│  [All] [Performance] [Features] [Value] [Specs]                │
│                                                                 │
│                    Product 1      Product 2       Winner       │
│  ─────────────────────────────────────────────────────────────  │
│  Spec 1             Value          Value          ✓            │
│  Spec 2             Value          Value               ✓       │
│  Spec 3             Value          Value          ✓            │
│  ...                                                            │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Verdict                                                        │
│                                                                 │
│  [Product 1] is better for [use case].                         │
│  [Product 2] is better for [use case].                         │
│                                                                 │
│  [View Product 1 Details]  [View Product 2 Details]            │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Auto-Generated Comparison Pages

For SEO, generate static comparison pages:

**URL pattern**: `/compare/[product-a]-vs-[product-b]/`

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Product A] vs [Product B]: Which Is Better in [Year]?        │
│                                                                 │
│  Written by [Author] | Updated [Date]                           │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Quick Answer                                                   │
│                                                                 │
│  [Product A] is better for [use case]. [Product B] is better   │
│  for [use case]. Here's the full breakdown.                    │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  [Interactive comparison table - same as tool]                  │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Detailed Analysis                                              │
│                                                                 │
│  [Category-by-category breakdown with explanations]             │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  FAQ                                                            │
│                                                                 │
│  Q: Is [A] better than [B] for [use case]?                     │
│  A: ...                                                         │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Related Comparisons                                            │
│                                                                 │
│  [A vs C] [A vs D] [B vs C] [B vs D]                           │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Calculators & Tools

### Calculator Types by Vertical

| Vertical | Calculator Types |
|----------|-----------------|
| **Finance** | Loan, mortgage, savings, ROI, budget |
| **Tech** | Build calculator, compatibility checker |
| **Insurance** | Quote estimator, coverage calculator |
| **Travel** | Cost estimator, trip planner |
| **Health** | BMI, calorie, dosage calculators |

### Calculator Page Structure

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Calculator Name] Calculator                                   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │                                                         │   │
│  │  [Interactive calculator interface]                     │   │
│  │                                                         │   │
│  │  Input 1: [___________]                                │   │
│  │  Input 2: [___________]                                │   │
│  │  Input 3: [___________]                                │   │
│  │                                                         │   │
│  │  [Calculate]                                            │   │
│  │                                                         │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Results                                                        │
│                                                                 │
│  [Dynamic results display with charts/visualizations]           │
│                                                                 │
│  Based on your inputs, we recommend:                            │
│  [Product recommendations based on calculation]                 │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  How This Calculator Works                                      │
│                                                                 │
│  [SEO content explaining methodology, formula, use cases]       │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  FAQ                                                            │
│                                                                 │
│  [Common questions about the calculation/topic]                 │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Product Database Pages

### Product Profile Page

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Product Name]                                                 │
│                                                                 │
│  ┌───────────────────────────────┐  ┌────────────────────────┐ │
│  │                               │  │                        │ │
│  │  [Product Image]              │  │  Price: $XXX           │ │
│  │                               │  │                        │ │
│  │                               │  │  Score: 8.5/10         │ │
│  │                               │  │                        │ │
│  │                               │  │  [Compare]             │ │
│  │                               │  │  [Check Price →]       │ │
│  └───────────────────────────────┘  └────────────────────────┘ │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  [Overview] [Specs] [Comparisons] [Alternatives] [Reviews]      │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Overview                                                       │
│                                                                 │
│  [Brief description of the product]                             │
│                                                                 │
│  Pros                          Cons                             │
│  ✓ Pro 1                       ✗ Con 1                         │
│  ✓ Pro 2                       ✗ Con 2                         │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Full Specifications                                            │
│                                                                 │
│  [Complete spec table]                                          │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Compare With                                                   │
│                                                                 │
│  [Product A] [Product B] [Product C]                           │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Similar Products                                               │
│                                                                 │
│  [Grid of alternatives in same category/price range]            │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Category/Browse Pages

### Filterable Product List

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Category Name]                                                │
│                                                                 │
│  [X] products in this category                                  │
│                                                                 │
├───────────────┬─────────────────────────────────────────────────┤
│               │                                                 │
│  FILTERS      │  Sort: [Popularity ▼]   [Grid] [List]          │
│               │                                                 │
│  Price        │  ┌─────────┐ ┌─────────┐ ┌─────────┐           │
│  [$__]-[$__]  │  │Product 1│ │Product 2│ │Product 3│           │
│               │  │         │ │         │ │         │           │
│  [Apply]      │  │ $XXX    │ │ $XXX    │ │ $XXX    │           │
│               │  │ 8.5/10  │ │ 7.9/10  │ │ 8.2/10  │           │
│  Brand        │  │[Compare]│ │[Compare]│ │[Compare]│           │
│  ☐ Brand A    │  └─────────┘ └─────────┘ └─────────┘           │
│  ☐ Brand B    │                                                 │
│  ☐ Brand C    │  ┌─────────┐ ┌─────────┐ ┌─────────┐           │
│               │  │Product 4│ │Product 5│ │Product 6│           │
│  Rating       │  │ ...     │ │ ...     │ │ ...     │           │
│  ☐ 9+ only    │  └─────────┘ └─────────┘ └─────────┘           │
│  ☐ 8+ only    │                                                 │
│               │  [Load More]                                    │
│  Features     │                                                 │
│  ☐ Feature 1  │                                                 │
│  ☐ Feature 2  │                                                 │
│               │                                                 │
└───────────────┴─────────────────────────────────────────────────┘
```

---

## SEO Strategy

### Programmatic SEO

Comparison sites excel at programmatic SEO:

| Page Type | Template | Scale |
|-----------|----------|-------|
| Product pages | 1 template | 1000s of pages |
| Comparison pages | 1 template | 1000s of pages |
| Category pages | 1 template | 10s-100s of pages |
| Calculator results | Dynamic | Infinite variations |

### Target Keywords

| Priority | Keyword Pattern | Example |
|----------|-----------------|---------|
| 1 | [A] vs [B] | "iPhone 15 vs Samsung S24" |
| 2 | best [product] [year] | "best laptop 2024" |
| 3 | [product] calculator | "mortgage calculator" |
| 4 | [category] comparison | "credit card comparison" |
| 5 | [product] specs | "MacBook Pro specs" |

### Internal Linking Strategy

- Product pages → comparison pages
- Comparison pages → product pages
- Category pages → all products in category
- Calculators → related products
- Related comparisons on every page

---

## Data & Updates

### Data Freshness

> "Comparison sites live or die by data accuracy. Stale prices or specs destroy trust."

**Update frequency**:
- Prices: Daily or real-time API
- Specs: When products update
- New products: Within days of release
- Discontinued: Mark as discontinued

### Data Sources

| Data Type | Sources |
|-----------|---------|
| Prices | Affiliate APIs, scraping, manual |
| Specs | Manufacturer data, manual entry |
| Reviews | Aggregated, original testing |
| Availability | Affiliate APIs |

---

## Monetization

### Affiliate Integration

| Placement | Type | Notes |
|-----------|------|-------|
| Product pages | Check price buttons | Multiple retailers |
| Comparison tool | Winner CTAs | Contextual |
| Calculator results | Recommendations | Based on calculation |
| Article content | Inline links | Natural mentions |

### Lead Generation (Finance)

For finance comparison sites:

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Based on your inputs, here are your top matches:               │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ [Provider Logo]  Provider Name                          │   │
│  │                                                         │   │
│  │ APR: X.XX%   Monthly: $XXX                             │   │
│  │                                                         │   │
│  │ [Check Eligibility →]  (Lead gen form)                  │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Technical Considerations

### Performance

- Fast filtering (client-side or AJAX)
- Efficient database queries
- CDN for static assets
- Lazy loading for large lists

### API Integration

- Price APIs for real-time data
- Affiliate network APIs
- Product data APIs (if available)

### Schema Markup

| Schema Type | Use Case |
|-------------|----------|
| `Product` | Product pages |
| `ItemList` | Category pages |
| `FAQPage` | FAQ sections |
| `HowTo` | Calculator explanations |
| `SoftwareApplication` | For apps/tools |

---

## Implementation Checklist

### Core Tools
- [ ] Comparison tool functional
- [ ] Calculator(s) working
- [ ] Product database populated
- [ ] Search working

### Content
- [ ] Category pages created
- [ ] Auto-generated VS pages
- [ ] Educational guides
- [ ] FAQ content

### Data
- [ ] Price update system
- [ ] Spec verification process
- [ ] New product workflow
- [ ] Data accuracy checks

### Monetization
- [ ] Affiliate links integrated
- [ ] Multiple retailers where possible
- [ ] Lead gen forms (if applicable)
- [ ] Tracking implemented

---

## Sources

- [PC Part Picker](https://pcpartpicker.com/) - Reference for build/comparison tools
- [NerdWallet](https://www.nerdwallet.com/) - Reference for finance comparison
- [Finder](https://www.finder.com/) - Reference for multi-vertical comparison
- [Bankrate](https://www.bankrate.com/) - Reference for calculator-first approach
- [Compare the Market](https://www.comparethemarket.com/) - Reference for UK comparison model
- [Search Engine Journal - Programmatic SEO](https://www.searchenginejournal.com/programmatic-seo/)
