# Information Architecture (IA) Patterns

> **Purpose**: Structure website content for findability and usability
> **Impact**: Good IA reduces bounce, increases conversions, improves SEO
> **Principle**: Users should find what they need in 3 clicks or less

---

## IA Fundamentals

### What is Information Architecture?

> "Information architecture is the practice of organizing, structuring, and labeling content to help users find information and complete tasks."
>
> *Source: [Usability.gov](https://www.usability.gov/what-and-why/information-architecture.html)*

### The Four Components

| Component | Definition | Example |
|-----------|------------|---------|
| **Organization** | How content is grouped | Categories, sections |
| **Labeling** | How content is named | Navigation labels, headings |
| **Navigation** | How users move around | Menus, breadcrumbs, links |
| **Search** | How users find specific content | Search functionality |

---

## Site Structure Patterns

### Hierarchical (Tree Structure)

```
                    Homepage
                        │
        ┌───────────────┼───────────────┐
        │               │               │
    Products        Services         About
        │               │               │
    ┌───┴───┐       ┌───┴───┐       ┌───┴───┐
  Cat A  Cat B   Serv 1  Serv 2   Team   Story
```

**Best for**: Most websites, clear parent-child relationships
**Depth**: Aim for 3-4 levels maximum

### Hub and Spoke

```
                    Homepage
                        │
    ┌───────┬───────┬───┴───┬───────┬───────┐
    │       │       │       │       │       │
  Page 1  Page 2  Page 3  Page 4  Page 5  Page 6
```

**Best for**: Landing pages, campaigns, simple sites
**Characteristic**: All pages same level, linked from hub

### Matrix/Network

```
  Topic A ←───→ Topic B
      ↑  ╲   ╱  ↑
      │   ╲ ╱   │
      │    ╳    │
      │   ╱ ╲   │
      ↓  ╱   ╲  ↓
  Topic C ←───→ Topic D
```

**Best for**: Complex relationships, knowledge bases, wikis
**Note**: Requires strong search and navigation

### Sequential/Linear

```
Step 1 → Step 2 → Step 3 → Step 4 → Complete
```

**Best for**: Checkout flows, onboarding, tutorials

---

## Content Grouping Strategies

### By Topic/Category

| Example | When to Use |
|---------|-------------|
| Products → Electronics → Phones | E-commerce |
| Services → Marketing → SEO | Service business |
| Articles → Tech → AI | Media/blog |

### By Audience

| Example | When to Use |
|---------|-------------|
| For Developers / For Designers | Developer tools |
| For Small Business / For Enterprise | B2B SaaS |
| Parents / Teachers / Students | Education |

### By Task/Intent

| Example | When to Use |
|---------|-------------|
| Learn / Build / Deploy | Developer docs |
| Get Started / Manage / Troubleshoot | Support portal |
| Browse / Compare / Buy | E-commerce |

### By Format

| Example | When to Use |
|---------|-------------|
| Articles / Videos / Podcasts | Media company |
| Templates / Guides / Tools | Resource library |
| Case Studies / Webinars / eBooks | Content marketing |

---

## URL Structure Best Practices

### URL Hierarchy

```
https://example.com/category/subcategory/page-name/
        ↑                                     ↑
    Domain                               Trailing slash
                    ↑
             Path reflects hierarchy
```

### URL Guidelines

| Good | Bad | Why |
|------|-----|-----|
| `/products/laptops/` | `/p/cat-123/` | Readable, SEO-friendly |
| `/blog/seo-guide/` | `/blog?id=456` | Clean URLs rank better |
| `/services/web-design/` | `/services/webdesign.html` | No file extensions |
| `/about/team/` | `/About/TEAM/` | Lowercase only |

### URL Patterns by Content Type

| Content Type | Pattern | Example |
|--------------|---------|---------|
| Blog post | `/blog/[post-slug]/` | `/blog/seo-best-practices/` |
| Product | `/products/[category]/[product]/` | `/products/shoes/running-pro/` |
| Service | `/services/[service-name]/` | `/services/web-development/` |
| Landing page | `/[keyword]/` | `/enterprise-seo-services/` |
| Tool | `/tools/[tool-name]/` | `/tools/roi-calculator/` |
| Help article | `/help/[topic]/[article]/` | `/help/billing/refunds/` |

---

## Navigation Planning

### Primary Navigation Rules

> "The ideal primary navigation has 5-7 items. More than that causes decision fatigue."
>
> *Source: [Nielsen Norman Group](https://www.nngroup.com/articles/navigation-menu-design/)*

| Item Count | Impact |
|------------|--------|
| 3-5 items | Optimal, easy to scan |
| 6-7 items | Acceptable |
| 8+ items | Too many, consider grouping |

### Navigation Label Best Practices

| Good Labels | Bad Labels | Why |
|-------------|------------|-----|
| Products | Our Solutions | Clear, direct |
| Pricing | Investment | Industry standard |
| Blog | Insights Hub | Users expect "Blog" |
| Contact | Get in Touch | Familiar pattern |
| About | Our Story | "About" is standard |

### Mega Menu Planning

```
PRODUCTS ▼
───────────────────────────────────────────────────────────

BY CATEGORY           BY USE CASE           RESOURCES
───────────           ───────────           ─────────
• Analytics           • For Marketing       • Documentation
• Automation          • For Sales           • API Reference
• Integration         • For Support         • Case Studies
• Reporting           • For Engineering     • Webinars

[Featured: New AI Analytics Platform - Learn More →]

───────────────────────────────────────────────────────────
```

**Mega menu guidelines**:
- 3-4 columns maximum
- Clear column headers
- Include featured content
- Link to category pages

---

## Content Hierarchy

### Page-Level Hierarchy

```
H1: Page Title (one per page)
    │
    ├── H2: Main Section 1
    │       │
    │       ├── H3: Subsection 1.1
    │       └── H3: Subsection 1.2
    │
    ├── H2: Main Section 2
    │       │
    │       ├── H3: Subsection 2.1
    │       │       │
    │       │       └── H4: Detail 2.1.1
    │       │
    │       └── H3: Subsection 2.2
    │
    └── H2: Main Section 3
```

### Heading Rules

| Rule | Example |
|------|---------|
| One H1 per page | Page title only |
| Don't skip levels | H2 → H3, not H2 → H4 |
| Descriptive, not generic | "Pricing Plans" not "Details" |
| Include keywords naturally | SEO benefit |

---

## Site Map Templates

### Corporate/B2B SaaS

```
Homepage
├── Products
│   ├── Product A
│   ├── Product B
│   └── All Products
├── Solutions
│   ├── By Industry
│   │   ├── Healthcare
│   │   ├── Finance
│   │   └── Retail
│   └── By Use Case
│       ├── Marketing
│       ├── Sales
│       └── Support
├── Pricing
├── Resources
│   ├── Blog
│   ├── Case Studies
│   ├── Webinars
│   ├── Documentation
│   └── API
├── Company
│   ├── About
│   ├── Team
│   ├── Careers
│   ├── Press
│   └── Contact
└── Legal
    ├── Privacy
    ├── Terms
    └── Security
```

### E-Commerce

```
Homepage
├── Shop
│   ├── Category 1
│   │   ├── Subcategory 1.1
│   │   └── Subcategory 1.2
│   ├── Category 2
│   ├── New Arrivals
│   ├── Sale
│   └── All Products
├── Collections
│   ├── Summer Collection
│   └── Best Sellers
├── About
│   ├── Our Story
│   ├── Sustainability
│   └── Blog
├── Help
│   ├── Shipping
│   ├── Returns
│   ├── Size Guide
│   ├── FAQ
│   └── Contact
├── Account
│   ├── Orders
│   ├── Wishlist
│   └── Settings
└── Legal
    ├── Privacy
    └── Terms
```

### Content/Media Site

```
Homepage
├── Topics
│   ├── Tech
│   │   ├── AI
│   │   ├── Software
│   │   └── Hardware
│   ├── Business
│   ├── Science
│   └── Culture
├── Formats
│   ├── Articles
│   ├── Videos
│   ├── Podcasts
│   └── Newsletters
├── About
│   ├── Team
│   ├── Editorial Policy
│   └── Contact
└── Subscribe
```

### Affiliate/Review Site

```
Homepage
├── Categories
│   ├── Category 1
│   │   ├── Best [Product Type]
│   │   ├── [Product] Reviews
│   │   └── [Product A] vs [Product B]
│   └── Category 2
├── Guides
│   ├── How to Choose [Product]
│   └── [Product] Buying Guide
├── Tools
│   ├── Comparison Tool
│   └── Quiz/Finder
├── About
│   ├── Our Team
│   ├── Methodology
│   └── Contact
└── Legal
    ├── Privacy
    ├── Terms
    └── Affiliate Disclosure
```

---

## Internal Linking Strategy

### Link Types

| Type | Purpose | Example |
|------|---------|---------|
| **Contextual** | Relevant in-text links | "Learn more about [SEO basics](/seo-guide/)" |
| **Navigation** | Move between sections | Header, footer, sidebar |
| **Related** | Show similar content | "Related articles" section |
| **Breadcrumb** | Show location | Home > Products > Laptops |
| **Call-to-action** | Drive conversions | "Get started" buttons |

### Link Distribution

```
Homepage
    │
    ├─── Links to ──→ Category pages (high authority)
    │
Category Page
    │
    ├─── Links to ──→ Product/article pages
    │
    └─── Links to ──→ Related categories

Article/Product Page
    │
    ├─── Links to ──→ Related articles/products
    │
    └─── Links to ──→ Category (via breadcrumb)
```

### Internal Linking Best Practices

| Do | Don't |
|----|-------|
| Use descriptive anchor text | Use "click here" |
| Link to relevant pages | Link randomly |
| Keep links updated | Leave broken links |
| Link deep pages from high-traffic pages | Only link to homepage |
| Use breadcrumbs | Hide user's location |

---

## Taxonomy & Tagging

### Category vs Tag

| Categories | Tags |
|------------|------|
| Hierarchical | Flat |
| Broad groupings | Specific attributes |
| Few per item | Many per item |
| Part of URL | Usually not in URL |
| Example: "Electronics" | Example: "Wireless, Bluetooth" |

### Taxonomy Planning

```
Category Structure:
└── Electronics
    ├── Phones
    │   ├── Smartphones
    │   └── Feature Phones
    ├── Computers
    │   ├── Laptops
    │   └── Desktops
    └── Audio
        ├── Headphones
        └── Speakers

Tag Examples:
- Wireless
- Under $100
- Best Seller
- New Arrival
- Editor's Pick
```

### Taxonomy Best Practices

| Practice | Reason |
|----------|--------|
| Start broad, refine later | Don't over-categorize initially |
| Limit depth to 3 levels | Beyond that, users get lost |
| Use clear, consistent naming | Helps users and SEO |
| Avoid overlapping categories | Creates confusion |
| Plan for growth | Categories should scale |

---

## IA Testing Methods

### Card Sorting

> "Card sorting is a method used to help design or evaluate the information architecture of a site."
>
> *Source: [Usability.gov](https://www.usability.gov/how-to-and-tools/methods/card-sorting.html)*

**Types**:
- **Open**: Users create and name categories
- **Closed**: Users sort into predefined categories
- **Hybrid**: Mix of both

### Tree Testing

Test if users can find items in your proposed structure:

1. Present navigation structure (no visual design)
2. Give users tasks: "Find the return policy"
3. Track success rate and path taken
4. Iterate based on results

### First-Click Testing

- Users see a page and a task
- Record where they click first
- Success correlates with first click accuracy

---

## Common IA Mistakes

| Mistake | Problem | Solution |
|---------|---------|----------|
| Too deep | Users get lost | Flatten to 3-4 levels |
| Jargon labels | Users confused | Use common terminology |
| Organization by org chart | Doesn't match user mental model | Organize by user needs |
| Too many categories | Decision paralysis | Consolidate |
| Inconsistent structure | Unpredictable | Apply same patterns |
| No search | Can't find specific items | Add search for 100+ pages |

---

## Sources

- [Nielsen Norman Group - IA Fundamentals](https://www.nngroup.com/articles/ia-vs-navigation/)
- [Usability.gov - Information Architecture](https://www.usability.gov/what-and-why/information-architecture.html)
- [A List Apart - Complete Beginner's Guide to IA](https://alistapart.com/article/thecompletebeginnersguidetoia/)
- [Rosenfeld Media - Information Architecture for the Web](https://rosenfeldmedia.com/books/information-architecture-for-the-world-wide-web/)
- [Content Design London - IA Principles](https://contentdesign.london/)
