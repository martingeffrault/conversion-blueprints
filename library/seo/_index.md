# SEO for Conversion

> **Purpose**: Understand when and how to optimize pages for search while maintaining conversion focus
> **Philosophy**: Not every page needs SEO—focus resources where they drive business outcomes
> **Principle**: Rank for intent that converts, not just traffic

---

## SEO vs. CRO: Finding the Balance

SEO and CRO sometimes conflict. Understanding when to prioritize each is key to efficient resource allocation.

### When They Align

| Scenario | SEO + CRO Both Win |
|----------|-------------------|
| **Informational content** | Ranks well, builds trust, drives conversions |
| **Product pages** | Search visibility + conversion optimization |
| **Category pages** | Navigation SEO + user experience |
| **Long-form guides** | Authority building + lead generation |

### When They Conflict

| Scenario | Prioritize | Why |
|----------|------------|-----|
| **Landing pages from ads** | CRO | Traffic is paid; maximize conversion |
| **Checkout/cart pages** | CRO | No search intent; pure conversion |
| **Account/dashboard pages** | Neither | Internal utility only |
| **Highly competitive SERP** | CRO | May not rank anyway |

---

## SEO Library Contents

### [When to Optimize](when-to-optimize.md)

**The PSMART Framework for SEO Decisions**

| Question | If No → Skip SEO |
|----------|------------------|
| **P**urpose — Is organic traffic a goal? | Landing pages, checkout |
| **S**earchable — Do people search for this? | Niche processes |
| **M**atchable — Can we match intent well? | Ambiguous queries |
| **A**chievable — Can we realistically rank? | Extreme competition |
| **R**elevant — Does traffic drive goals? | Traffic without conversions |
| **T**rackable — Can we measure success? | No attribution |

Covers:
- Page types by SEO priority (high/medium/low/none)
- Resource allocation framework
- Common SEO mistakes for CRO-focused sites

---

## Quick Reference: SEO Priority by Page Type

### High Priority (Optimize Fully)

| Page Type | Target Keywords | SEO Focus |
|-----------|-----------------|-----------|
| Homepage | Brand + category | Authority, structure |
| Category/hub pages | "[category]" | Topic clusters |
| Blog/content | Long-tail questions | Informational intent |
| Comparison pages | "[A] vs [B]" | Decision stage |
| Product pages | "[product name]" | Transactional |
| Location pages | "[service] + [city]" | Local search |

### Medium Priority (Light Optimization)

| Page Type | SEO Approach |
|-----------|--------------|
| About page | Brand keywords, basic optimization |
| Pricing page | Keyword in title, schema markup |
| FAQ page | Question schema, long-tail |
| Contact page | Local SEO, NAP consistency |

### Low/No Priority (Skip or Minimal)

| Page Type | Why Skip SEO |
|-----------|--------------|
| Landing pages (paid) | Traffic is paid, focus on conversion |
| Checkout/cart | No search intent |
| Account pages | Internal utility |
| Thank you pages | Post-conversion |
| Legal pages | Compliance only |
| Demo request pages | CRO-focused |

---

## SEO Elements That Help CRO

Some SEO best practices also improve conversion:

### Page Speed

| Impact | Data |
|--------|------|
| SEO ranking factor | Yes (Core Web Vitals) |
| CRO impact | 7% conversion loss per second delay |

### Mobile Optimization

| Impact | Data |
|--------|------|
| SEO ranking factor | Yes (mobile-first indexing) |
| CRO impact | 60%+ of traffic is mobile |

### Structured Data

| Schema Type | SEO Benefit | CRO Benefit |
|-------------|-------------|-------------|
| Product | Rich snippets | Click-through rate |
| FAQ | FAQ rich results | Reduced bounce |
| Review | Star ratings in SERP | Trust signals |
| Breadcrumb | Site hierarchy | Navigation clarity |

### Content Quality

| Factor | SEO Benefit | CRO Benefit |
|--------|-------------|-------------|
| Clear headlines | Keyword targeting | Value prop clarity |
| Scannable content | Dwell time | Reduced bounce |
| Comprehensive answers | Topical authority | Trust building |

---

## Common SEO Mistakes on Conversion-Focused Sites

### Mistake 1: Over-Optimizing Landing Pages

**Problem**: Stuffing landing pages with keywords for organic traffic
**Issue**: Dilutes conversion focus, confuses messaging
**Solution**: Separate content pages (SEO) from landing pages (CRO)

### Mistake 2: Ignoring Commercial Intent

**Problem**: Chasing high-volume informational keywords
**Issue**: Traffic without purchase intent doesn't convert
**Solution**: Target transactional and commercial keywords

### Mistake 3: Duplicate Content from A/B Tests

**Problem**: Multiple page variants indexed
**Issue**: Dilutes ranking signals, confuses search
**Solution**: Canonical tags, noindex on variants

### Mistake 4: Thin Product Pages

**Problem**: Minimal content on product pages
**Issue**: Won't rank, doesn't convert
**Solution**: Rich descriptions, specs, reviews, FAQ

---

## Technical SEO Essentials

### For All Pages

```html
<title>Primary Keyword - Secondary | Brand</title>
<meta name="description" content="Compelling description with keyword...">
<link rel="canonical" href="https://example.com/page/">
```

### For Product Pages

```json
{
  "@type": "Product",
  "name": "Product Name",
  "aggregateRating": { "ratingValue": "4.5" },
  "offers": { "price": "99.00" }
}
```

### For FAQ Pages

```json
{
  "@type": "FAQPage",
  "mainEntity": [{
    "@type": "Question",
    "name": "Question text?",
    "acceptedAnswer": { "text": "Answer text..." }
  }]
}
```

---

## Key Metrics

### SEO Metrics That Matter for Conversion

| Metric | Why It Matters |
|--------|----------------|
| **Organic conversion rate** | Not just traffic—conversions |
| **Assisted conversions** | SEO's role in the journey |
| **Branded vs. non-branded** | Awareness vs. acquisition |
| **Landing page performance** | Which organic pages convert |

### What to Ignore

| Metric | Why It's Misleading |
|--------|---------------------|
| Raw organic traffic | Volume without intent |
| Keyword rankings alone | Rankings ≠ conversions |
| Domain authority | Vanity metric |

---

## Resources

### Internal Cross-References

- [Page Blueprints](../pages/) — SEO-optimized page structures
- [Content Strategy](../content/) — Writing for search and conversion
- [Analytics](../analytics/) — Tracking organic performance
- [Technical Performance](../analytics/technical-performance.md) — Core Web Vitals

### External Resources

- Google Search Central — [Official documentation](https://developers.google.com/search)
- Ahrefs Blog — SEO tactics and research
- Moz — SEO guides and tools
- Search Engine Journal — Industry news

---

## Key Takeaways

1. **Not every page needs SEO** — Use PSMART to decide
2. **Match intent to conversion** — Target keywords with purchase intent
3. **SEO and CRO can coexist** — Technical SEO often helps conversion
4. **Measure what matters** — Organic conversions, not just traffic
5. **Separate content from landing** — Different goals, different optimization

---

*Rank for intent that converts, not just traffic.*
