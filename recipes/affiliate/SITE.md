# Affiliate / Review Website Recipe

> **Business Type**: Product reviews, comparisons, affiliate marketing
> **Primary Goals**: Drive clicks to affiliate links, build authority, rank for buying intent keywords
> **Revenue Model**: Affiliate commissions, display ads, sponsored content
> **Reference Sites**: Wirecutter, NerdWallet, RTINGS, Sleep Foundation, PC Part Picker

---

## Site Architecture

### Core Pages (Must Have)

```
/                       Homepage (hub for all content)
├── /[category]/        Category hub pages
│   └── /[category]/[article]/   Individual review/comparison articles
├── /about/             About + methodology
├── /contact/           Contact page
└── /[legal]/           Privacy, terms, affiliate disclosure
```

### Content Pages

```
├── /best-[product]/              "Best X" roundup articles
├── /[product]-review/            Individual product reviews
├── /[product-a]-vs-[product-b]/  Head-to-head comparisons
├── /[topic]-guide/               Buying guides (educational)
└── /[category]/                  Category landing pages
```

### Trust Pages

```
├── /about/             Team, mission, story
├── /methodology/       How you test/review (critical for E-E-A-T)
├── /editorial-policy/  Review standards
└── /affiliate-disclosure/  FTC compliance
```

---

## Page Hierarchy Diagram

```
                        ┌─────────────┐
                        │  HOMEPAGE   │
                        └──────┬──────┘
                               │
          ┌────────────────────┼────────────────────┐
          │                    │                    │
     ┌────▼────┐          ┌────▼────┐          ┌────▼────┐
     │CATEGORY │          │CATEGORY │          │CATEGORY │
     │  HUB    │          │  HUB    │          │  HUB    │
     └────┬────┘          └────┬────┘          └────┬────┘
          │                    │                    │
    ┌─────┼─────┐        ┌─────┼─────┐        ┌─────┼─────┐
    │     │     │        │     │     │        │     │     │
 Best X  VS   Review   Best X  VS   Review   Best X  VS   Review
```

---

## Content Types (By Intent)

### High Buying Intent (Monetize)

| Type | URL Pattern | Example | Purpose |
|------|-------------|---------|---------|
| **Best X Roundup** | `/best-[product]/` | `/best-wireless-earbuds/` | Primary revenue driver |
| **Comparison (VS)** | `/[a]-vs-[b]/` | `/airpods-pro-vs-sony-wf/` | Decision-stage visitors |
| **Single Review** | `/[product]-review/` | `/airpods-pro-review/` | Brand searches |
| **Best X for Y** | `/best-[product]-for-[audience]/` | `/best-earbuds-for-running/` | Niche segments |

### Medium Intent (Educate → Convert)

| Type | URL Pattern | Example | Purpose |
|------|-------------|---------|---------|
| **Buying Guide** | `/how-to-choose-[product]/` | `/how-to-choose-earbuds/` | Educate, build trust |
| **Category Hub** | `/[category]/` | `/headphones/` | Internal linking, navigation |
| **Listicle** | `/[number]-best-[product]/` | `/10-best-budget-earbuds/` | SEO, social shares |

### Low Intent (Traffic → Nurture)

| Type | URL Pattern | Example | Purpose |
|------|-------------|---------|---------|
| **Educational** | `/what-is-[topic]/` | `/what-is-active-noise-cancelling/` | Top of funnel |
| **Problem/Solution** | `/[problem]/` | `/earbuds-keep-falling-out/` | Problem-aware visitors |

---

## Homepage Structure

The homepage serves as a navigation hub and authority signal.

### Recommended Sections

```
1. Hero
   └── Value prop, trust signals, search

2. Featured Categories
   └── Visual category navigation

3. Latest/Featured Reviews
   └── Recent high-value content

4. Popular Comparisons
   └── "Best X" article cards

5. Trust Section
   └── Methodology, team, credentials

6. Newsletter Signup
   └── Email capture

7. Footer
   └── Categories, legal, social
```

### Homepage Hero Options

**Option A: Search-Focused**
```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│          Find the Best [Product Category] for You               │
│                                                                 │
│       We test 100+ products so you don't have to.               │
│                                                                 │
│       [Search: What are you looking for?___________🔍]          │
│                                                                 │
│       Popular: Headphones | Laptops | Cameras | Monitors        │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Option B: Category-Focused**
```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│          Expert Reviews. Honest Recommendations.                │
│                                                                 │
│   ┌──────────┐  ┌──────────┐  ┌──────────┐  ┌──────────┐       │
│   │ [Image]  │  │ [Image]  │  │ [Image]  │  │ [Image]  │       │
│   │Headphones│  │ Laptops  │  │ Cameras  │  │ Monitors │       │
│   └──────────┘  └──────────┘  └──────────┘  └──────────┘       │
│                                                                 │
│   Trusted by 2M+ readers | 500+ products tested                 │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Category Hub Structure

Category hubs are critical for SEO and navigation.

### Sections

```
1. Hero
   └── Category name, description, key stats

2. Quick Picks
   └── Top 3 recommendations with anchor links

3. Comparison Table
   └── All reviewed products side-by-side

4. Featured Articles
   └── Best X, buying guide, key comparisons

5. All Articles
   └── Complete list of category content

6. FAQ
   └── Common category questions
```

---

## Comparison Article Structure (Wirecutter Model)

This is the core monetization content. Structure is critical.

### Article Flow

```
1. Title + Meta
   └── "The [Number] Best [Products] of [Year]"

2. Quick Picks Summary (TOP OF PAGE - CRITICAL)
   └── Winner, runner-up, budget pick with affiliate links

3. Methodology/Credibility
   └── How you tested, expert input, credentials

4. Comparison Table
   └── All products with key specs

5. Detailed Reviews
   └── Individual product sections with pros/cons

6. Buying Guide
   └── What to look for, how to choose

7. FAQ
   └── Common questions

8. Final Verdict
   └── Summary + CTAs
```

### Quick Picks Section (Critical for Conversions)

> "These summaries are a staple of Wirecutter's reviews. Before losing any readers to the Back button, they are intentional about establishing authority, introducing the reviewers, and giving you the 'quick take' of which product they think is best and why."
>
> *Source: [Affilimate](https://affilimate.com/blog/product-review-template/)*

```
## Our Top Picks

┌─────────────────────────────────────────────────────────────────┐
│ 🏆 BEST OVERALL                                                 │
│                                                                 │
│ [Product Image]  Product Name                                   │
│                  ⭐⭐⭐⭐⭐ 4.8/5                                   │
│                                                                 │
│                  Brief 2-3 sentence summary of why it's best.   │
│                  Key standout feature mentioned.                │
│                                                                 │
│                  [Check Price at Amazon →]                      │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│ 💰 BEST VALUE                                                   │
│                                                                 │
│ [Product Image]  Product Name                                   │
│                  ...                                            │
└─────────────────────────────────────────────────────────────────┘
```

### First Links Convert Best

> "Your first links are usually the most lucrative. They clearly state the best product right there in the intro. This is critical, since many people are lazy and just want to buy 'the best' without reading."
>
> *Source: [Ahrefs - Wirecutter Case Study](https://ahrefs.com/blog/wirecutter-seo-case-study/)*

---

## Trust & E-E-A-T Elements

Critical for affiliate sites post-Google's helpful content updates.

### Methodology Page

> "Sleep Foundation's research methodology page breaks down how their lab team tests mattresses. Each product gets lab scores across multiple criteria, a summary of who it's best for, and clear pros/cons."
>
> *Source: [Tetra Marketing](https://www.tetramarketing.io/p/site-analysis-wirecutter)*

**Include**:
- Testing process
- Evaluation criteria
- Expert involvement
- Update frequency

### Author Bylines

Show who wrote the review and their credentials.

```
Written by [Name], [Title/Credentials]
Reviewed by [Expert Name], [Credentials]
Last updated: [Date]
```

### First-Person Experience

> "Writing from the first person, highlighting your personal experience, builds the most trust and rapport with your audience, and also sends signals to search engines that this is a real product review."
>
> *Source: [Lasso](https://getlasso.co/product-review-template/)*

---

## Navigation Structure

### Primary Navigation
```
[Logo]  Categories ▼  Guides  About  [Search 🔍]
```

### Mega Menu (Categories)
```
AUDIO                 COMPUTERS            HOME
──────                ─────────            ────
Headphones            Laptops              Mattresses
Earbuds               Monitors             Vacuums
Speakers              Keyboards            Coffee Makers
Soundbars             Mice                 Air Purifiers
```

### Footer
```
CATEGORIES       ABOUT           LEGAL
──────────       ─────           ─────
All Categories   Our Team        Affiliate Disclosure
Popular Reviews  Methodology     Privacy Policy
Latest Articles  Editorial Policy Terms of Service
                 Contact Us
```

---

## SEO Strategy

### Keyword Types (By Priority)

| Priority | Type | Example | Volume | Intent |
|----------|------|---------|--------|--------|
| 1 | Best X | "best wireless earbuds" | High | Transactional |
| 2 | Product Review | "airpods pro 2 review" | Medium | Commercial |
| 3 | VS Comparison | "airpods vs galaxy buds" | Medium | Commercial |
| 4 | Best X for Y | "best earbuds for small ears" | Low-Med | Transactional |
| 5 | How to Choose | "how to choose earbuds" | Medium | Informational |

### Internal Linking Strategy

- Category hub → All category articles
- Comparison articles → Individual reviews
- Individual reviews → Related comparisons
- Buying guides → Best X articles
- Cross-link between related categories

---

## Monetization Elements

### Affiliate Link Placement

| Location | Effectiveness | Notes |
|----------|--------------|-------|
| Quick picks (top) | Highest | First links convert best |
| Product headers | High | Easy to find |
| Comparison table | High | Side-by-side decision |
| Inline mentions | Medium | Natural placement |
| Final verdict | Medium | Post-read decision |

### Display Ads (If Applicable)
- Above fold: 1 max
- In-content: Every 3-4 paragraphs
- Sidebar: Sticky if desktop
- Don't overwhelm — trust first

### Affiliate Disclosure

FTC requires clear disclosure. Place:
- Near the top of affiliate content
- In a visible affiliate disclosure page
- Link in footer

---

## Reference Sites to Study

| Site | Strength | Study For |
|------|----------|-----------|
| **Wirecutter** | Structure, authority, SEO | Article format |
| **RTINGS** | Testing methodology, data | Technical reviews |
| **NerdWallet** | Comparison tools, UX | Finance reviews |
| **Sleep Foundation** | E-E-A-T, experts | Trust signals |
| **PC Part Picker** | Comparison tools | Price tracking |
| **Tom's Guide** | Volume, categories | Content breadth |

---

## Implementation Checklist

### Foundation
- [ ] Core pages (home, about, methodology, disclosure)
- [ ] Category structure defined
- [ ] Navigation implemented
- [ ] Search functionality

### Content
- [ ] 3+ "Best X" articles per category
- [ ] 1+ buying guide per category
- [ ] Author bios with credentials
- [ ] Methodology page complete

### Trust
- [ ] Affiliate disclosure on all pages
- [ ] Author bylines on all content
- [ ] Methodology explained
- [ ] Expert input where relevant

### Monetization
- [ ] Affiliate accounts set up (Amazon, etc.)
- [ ] Link tracking implemented
- [ ] Quick picks at top of articles
- [ ] Comparison tables with links

### SEO
- [ ] Keyword research complete
- [ ] Internal linking strategy
- [ ] Schema markup (Product, Review)
- [ ] Image optimization

---

*See individual page files in `pages/` for detailed article templates.*
