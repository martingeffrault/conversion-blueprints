# Deep Product Review Site Recipe

> **Variant Focus**: In-depth product testing, hands-on reviews, expert analysis
> **Examples**: Wirecutter, RTINGS, Sleep Foundation, Headphones.com, DxOMark
> **Key Differentiator**: Testing methodology, data-driven reviews, expert authority
> **Revenue Model**: Affiliate commissions (Amazon, direct), display ads
> **E-E-A-T Priority**: Critical (Google scrutinizes review sites heavily)

---

## How This Differs from Comparison Site

| Aspect | Review Site | Comparison/Tool Site |
|--------|-------------|---------------------|
| Content depth | Deep, long-form | Broader, tool-focused |
| Testing | Hands-on, proprietary | Aggregated data |
| Expertise | Expert reviewers | Data analysis |
| Monetization | Affiliate + ads | Affiliate + tools |
| Trust signals | Methodology, labs | Database completeness |
| Updates | Regular testing | Continuous data updates |

---

## Site Architecture

### Core Pages

```
/                           Homepage (authority hub)
├── /[category]/            Category hubs
│   └── /[category]/best-[product]/   Best X roundups
│   └── /[category]/[product]-review/ Individual reviews
│   └── /[category]/[a]-vs-[b]/       Head-to-head comparisons
├── /buying-guides/         Educational content
│   └── /buying-guides/[topic]/
├── /methodology/           How we test (critical for E-E-A-T)
├── /about/                 Team, experts, credentials
├── /contact/               Contact page
└── /[legal]/               Privacy, terms, affiliate disclosure
```

### Content Hierarchy

```
                        ┌─────────────┐
                        │  HOMEPAGE   │
                        └──────┬──────┘
                               │
          ┌────────────────────┼────────────────────┐
          │                    │                    │
     ┌────▼────┐          ┌────▼────┐          ┌────▼────┐
     │CATEGORY │          │CATEGORY │          │ BUYING  │
     │  HUB    │          │  HUB    │          │ GUIDES  │
     └────┬────┘          └────┬────┘          └────┬────┘
          │                    │                    │
    ┌─────┼─────┐        ┌─────┼─────┐        ┌─────┴─────┐
    │     │     │        │     │     │        │           │
Best X  Review  VS    Best X  Review  VS   How to    What is
                                           Choose     [Topic]
```

---

## E-E-A-T: The Foundation

> "Google's helpful content system and product review updates have made E-E-A-T signals essential for affiliate sites. Sites without demonstrable expertise struggle to rank."
>
> *Pattern from: [Google Search Central - Product Reviews](https://developers.google.com/search/docs/specialty/ecommerce/product-reviews)*

### Experience (Hands-On Testing)

**Must demonstrate**:
- Physical testing of products
- Original photos (not manufacturer stock)
- Video reviews showing usage
- Long-term testing notes

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Original photo of product being tested in lab/home]           │
│                                                                 │
│  We tested this product for 3 months in our lab and in         │
│  real-world conditions.                                         │
│                                                                 │
│  Testing performed by: [Expert Name], [Credentials]             │
│  Last tested: [Date]                                            │
│  Total test hours: [X] hours                                    │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Expertise (Qualified Reviewers)

**Show credentials**:
- Author bylines with qualifications
- Expert reviewer input
- Industry experience
- Relevant education/certifications

### Authoritativeness (Recognized Source)

**Build through**:
- Methodology page (detailed)
- Press coverage and citations
- Industry awards
- Expert advisory board

### Trustworthiness (Honest Reviews)

**Demonstrate**:
- Clear affiliate disclosure
- Negative reviews published
- Update history shown
- Corrections/updates noted

---

## Methodology Page (Critical)

> "Sleep Foundation's research methodology page breaks down how their lab team tests mattresses. This level of transparency is now table stakes for ranking."
>
> *Reference: [Sleep Foundation Methodology](https://www.sleepfoundation.org/research-methodology)*

### Methodology Page Structure

```
1. Overview
   └── How and why we test

2. Testing Process
   └── Step-by-step methodology

3. Scoring Criteria
   └── How we rate products

4. Our Team
   └── Who performs testing, their credentials

5. Equipment & Lab
   └── Testing environment, tools used

6. Update Policy
   └── How often we retest

7. Editorial Independence
   └── How we avoid bias
```

### Methodology Page Example

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  How We Test [Products]                                         │
│                                                                 │
│  Our [X]-step testing process ensures every review is           │
│  thorough, unbiased, and helpful.                               │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Our Testing Process                                            │
│                                                                 │
│  ┌─────┐    ┌─────┐    ┌─────┐    ┌─────┐    ┌─────┐           │
│  │  1  │ →  │  2  │ →  │  3  │ →  │  4  │ →  │  5  │           │
│  └─────┘    └─────┘    └─────┘    └─────┘    └─────┘           │
│                                                                 │
│  Research   Acquire   Test      Analyze    Publish              │
│  Market     Products  In-Lab    Data       Review               │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  What We Measure                                                │
│                                                                 │
│  [Category-specific criteria with explanations]                 │
│                                                                 │
│  • Criterion 1: [Explanation, how we measure]                   │
│  • Criterion 2: [Explanation, how we measure]                   │
│  • Criterion 3: [Explanation, how we measure]                   │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Our Testing Equipment                                          │
│                                                                 │
│  [Photos of lab, equipment, testing setup]                      │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Meet Our Testers                                               │
│                                                                 │
│  [Expert photos, credentials, experience]                       │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Review Article Structure

### Individual Product Review

```
1. Hero
   └── Product name, rating, quick verdict, main image

2. At a Glance
   └── Pros/cons, key specs, price, where to buy

3. Our Testing
   └── How we tested, what we measured

4. Performance
   └── Detailed breakdown by category

5. Comparisons
   └── How it stacks up to alternatives

6. Who It's For
   └── Ideal user profile

7. Verdict
   └── Final thoughts, rating breakdown

8. Where to Buy
   └── Affiliate links with price comparison

9. FAQ
   └── Common questions

10. Related Reviews
    └── Similar products tested
```

### Review Page Layout

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Product Name] Review                                          │
│                                                                 │
│  ⭐⭐⭐⭐⭐ 9.2/10                                                │
│                                                                 │
│  "The best [product type] we've tested for most people."        │
│                                                                 │
│  Written by [Expert] | Tested [Date] | Updated [Date]           │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌─────────────────────────────┐  ┌────────────────────────┐   │
│  │                             │  │                        │   │
│  │  [Product Image - Original] │  │  QUICK VERDICT         │   │
│  │                             │  │                        │   │
│  │                             │  │  ✓ Pro 1               │   │
│  │                             │  │  ✓ Pro 2               │   │
│  │                             │  │  ✓ Pro 3               │   │
│  │                             │  │  ✗ Con 1               │   │
│  │                             │  │  ✗ Con 2               │   │
│  │                             │  │                        │   │
│  │                             │  │  Price: $XXX           │   │
│  │                             │  │                        │   │
│  │                             │  │  [Check Price →]       │   │
│  │                             │  │                        │   │
│  └─────────────────────────────┘  └────────────────────────┘   │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Scores by Category                                             │
│                                                                 │
│  Performance     ████████████░░  8.5                            │
│  Build Quality   █████████████░  9.0                            │
│  Value           ██████████████  9.5                            │
│  Features        ███████████░░░  8.0                            │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  [Table of Contents]                                            │
│                                                                 │
│  1. How We Tested                                               │
│  2. Performance Analysis                                        │
│  3. Comparisons                                                 │
│  4. Who Should Buy                                              │
│  5. Verdict                                                     │
│  6. Where to Buy                                                │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  [Long-form content with original images, test data,            │
│   measurements, charts, and detailed analysis]                  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## "Best X" Roundup Structure

The primary monetization content.

### Roundup Article Flow

```
1. Title
   └── "The [X] Best [Products] of [Year]"

2. Quick Picks (TOP - Critical)
   └── Winner, runner-up, budget, best for [use case]

3. Why Trust Us
   └── Credentials, testing methodology brief

4. Comparison Table
   └── All products with key specs and ratings

5. Detailed Reviews
   └── Each product with testing notes

6. Buying Guide
   └── What to look for

7. How We Tested
   └── Methodology for this category

8. FAQ
   └── Common questions

9. Methodology Link
   └── Link to full methodology page
```

### Quick Picks Section (Critical)

> "Your first links are usually the most lucrative. State the best product right there in the intro."
>
> *Source: [Ahrefs - Wirecutter Case Study](https://ahrefs.com/blog/wirecutter-seo-case-study/)*

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Our Top Picks                                                  │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ 🏆 BEST OVERALL                                         │   │
│  │                                                         │   │
│  │  ┌──────────┐  [Product Name]                          │   │
│  │  │ [Image]  │  ⭐⭐⭐⭐⭐ 9.2/10                           │   │
│  │  └──────────┘                                          │   │
│  │                                                         │   │
│  │  Why we picked it: [2-3 sentences on why it's best]    │   │
│  │                                                         │   │
│  │  ✓ Best overall performance                            │   │
│  │  ✓ Excellent build quality                             │   │
│  │  ✗ Premium price                                       │   │
│  │                                                         │   │
│  │  [Check Price at Amazon] [Check at Retailer]           │   │
│  │                                                         │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ 💰 BEST VALUE                                           │   │
│  │  ...                                                    │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ ⚡ BEST FOR [USE CASE]                                  │   │
│  │  ...                                                    │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Author Pages & Bylines

### Author Byline (On Every Article)

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Avatar]  Written by [Name]                                    │
│            [Title/Credentials]                                  │
│            Tested: [Date] | Updated: [Date]                     │
│                                                                 │
│  Reviewed by [Expert Name], [Credentials]                       │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Author Page Structure

Dedicated author pages help with E-E-A-T:

```
/author/[name]/

1. Bio
   └── Credentials, experience, expertise areas

2. Why Trust This Expert
   └── Education, certifications, industry experience

3. Published Reviews
   └── All articles by this author

4. Social/Professional Links
   └── LinkedIn, Twitter, publications
```

---

## Category Hub Structure

### Hub Page Elements

```
1. Hero
   └── Category name, description, expert quote

2. Quick Picks
   └── Top 3 recommendations

3. All Reviews
   └── Full list of tested products

4. Buying Guide
   └── What to look for in this category

5. FAQ
   └── Common category questions

6. Related Categories
   └── Adjacent categories
```

---

## Content Freshness

### Update Signals

> "Showing when content was last updated and tested is now essential for review content. Google's product review updates penalize stale content."

**Display prominently**:
- Last tested date
- Last updated date
- Update changelog (optional)

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  📅 This article was last updated on [Date]                     │
│                                                                 │
│  Update log:                                                    │
│  • [Date]: Added [New Product] after testing                    │
│  • [Date]: Retested [Product] after firmware update             │
│  • [Date]: Updated prices and availability                      │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Schema Markup

### Required Schema

| Schema Type | Use Case |
|-------------|----------|
| `Product` | Individual products |
| `Review` | Review content |
| `AggregateRating` | Overall ratings |
| `Person` (author) | E-E-A-T signals |
| `Organization` | Site authority |
| `ItemList` | Best X roundups |
| `HowTo` (if applicable) | Guides, tutorials |

### Review Schema Example

```json
{
  "@type": "Product",
  "name": "Product Name",
  "review": {
    "@type": "Review",
    "author": {
      "@type": "Person",
      "name": "Reviewer Name"
    },
    "reviewRating": {
      "@type": "Rating",
      "ratingValue": "9.2",
      "bestRating": "10"
    },
    "reviewBody": "Review summary..."
  }
}
```

---

## Implementation Checklist

### Foundation
- [ ] Methodology page complete
- [ ] Author pages with credentials
- [ ] Affiliate disclosure prominent
- [ ] About page with team

### Content
- [ ] Original product photography
- [ ] Detailed testing data
- [ ] Pros/cons on every review
- [ ] Regular content updates

### Trust Signals
- [ ] Author bylines on all content
- [ ] Testing dates displayed
- [ ] Update logs where relevant
- [ ] Expert reviewer input

### Technical
- [ ] Review schema markup
- [ ] Image optimization
- [ ] Fast page load
- [ ] Mobile-friendly

---

## Sources

- [Google - Product Review Update Guidelines](https://developers.google.com/search/docs/specialty/ecommerce/product-reviews)
- [Wirecutter](https://www.nytimes.com/wirecutter/) - Reference for structure and methodology
- [RTINGS](https://www.rtings.com/) - Reference for testing methodology
- [Sleep Foundation](https://www.sleepfoundation.org/) - Reference for E-E-A-T implementation
- [Ahrefs - Wirecutter SEO Case Study](https://ahrefs.com/blog/wirecutter-seo-case-study/)
- [Affilimate - Product Review Templates](https://affilimate.com/blog/product-review-template/)
