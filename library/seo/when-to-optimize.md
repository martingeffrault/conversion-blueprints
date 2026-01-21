# SEO: When to Optimize (and When Not To)

> **Purpose**: Understand which pages deserve SEO investment and which don't
> **Framework**: PSMART methodology for page-level SEO decisions
> **Goal**: Allocate SEO resources efficiently for maximum ROI

---

## Core Principle

Not every page should be optimized for search engines. Some pages serve conversion, brand, or support purposes where SEO is irrelevant or counterproductive. Spend SEO resources where they drive business outcomes.

> "The best SEO strategy is knowing when NOT to do SEO."
>
> *Source: Common SEO wisdom*

---

## PSMART Framework for Page SEO

Use PSMART to evaluate whether a page should be SEO-optimized:

| Letter | Question | If No → Skip SEO |
|--------|----------|------------------|
| **P**urpose | Is organic traffic a goal for this page? | Landing pages, checkout, account |
| **S**earchable | Do people search for this content? | Internal tools, niche processes |
| **M**atchable | Can we match search intent well? | If intent is ambiguous |
| **A**chievable | Can we realistically rank? | Extremely competitive SERPs |
| **R**elevant | Does traffic here drive business goals? | Traffic without conversions |
| **T**rackable | Can we measure SEO success? | If attribution is impossible |

---

## Page Types: SEO Priority Matrix

### High SEO Priority ✅

These pages should be fully optimized:

| Page Type | Why Optimize | Target Keywords |
|-----------|--------------|-----------------|
| **Homepage** | Brand searches, category | Brand + category |
| **Category/Hub pages** | Navigate intent | "[category]" |
| **Blog/Content** | Informational queries | Long-tail questions |
| **Comparison pages** | Decision stage | "[A] vs [B]" |
| **Product pages** | Transactional intent | "[product name]" |
| **Location pages** | Local search | "[service] + [city]" |
| **Resource pages** | Lead magnets | "[topic] guide" |

### Low/No SEO Priority ❌

These pages should NOT be optimized (or minimally):

| Page Type | Why Skip SEO | Focus Instead On |
|-----------|--------------|------------------|
| **Landing pages (paid)** | Traffic comes from ads | Conversion rate |
| **Checkout/Cart** | No search intent | UX, abandonment |
| **Account pages** | Logged-in users | Functionality |
| **Thank you pages** | Post-conversion | Next steps, upsells |
| **Legal pages** | Compliance, not discovery | Clarity, compliance |
| **Internal tools** | Not meant for public | Usability |
| **A/B test variants** | Temporary, thin | Test performance |
| **Filtered/Sorted URLs** | Duplicate content | Canonical to main |

---

## Landing Pages: The SEO Paradox

### Should Landing Pages Be SEO-Optimized?

**Short answer: Usually no.**

| LP Type | SEO Priority | Rationale |
|---------|--------------|-----------|
| **Paid campaign LP** | ❌ None | Traffic from ads, noindex often best |
| **Product LP** | ⚠️ Low-Medium | Can rank, but product pages often better |
| **Event/Webinar LP** | ❌ None | Time-sensitive, paid traffic |
| **Lead magnet LP** | ⚠️ Medium | Can rank for "[topic] guide" |
| **Evergreen LP** | ✅ High | If topic has search volume |

### Why Most LPs Shouldn't Be SEO-Optimized

1. **Message match**: LP copy must match ad copy; SEO requires different optimization
2. **Conversion focus**: SEO elements (links, navigation) reduce conversion
3. **Speed**: Quick experiments don't allow time for SEO to work
4. **Cannibalization**: LPs can compete with main site pages
5. **Intent mismatch**: Searchers often want information, not conversion-focused pages

### When LP SEO Makes Sense

- **Evergreen offers** that will exist for years
- **Topics with clear search volume** and transactional intent
- **Lead magnet LPs** where the guide/resource is the draw
- **Product-specific LPs** for branded searches

---

## SEO Considerations by Business Type

### SaaS / B2B

| Page | SEO Priority | Notes |
|------|--------------|-------|
| Homepage | High | Brand + category |
| Feature pages | High | "[feature] software" |
| Comparison pages | High | "[competitor] alternative" |
| Integration pages | High | "[tool A] + [tool B] integration" |
| Pricing page | Low | Few people search pricing |
| Demo page | None | Conversion-focused |
| Blog | High | Top-of-funnel awareness |
| Case studies | Medium | Branded + industry searches |
| Documentation | High | Problem-solving searches |

> **Source**: [Ahrefs - B2B SaaS SEO](https://ahrefs.com/blog/b2b-saas-seo/)

### E-commerce

| Page | SEO Priority | Notes |
|------|--------------|-------|
| Homepage | High | Brand searches |
| Category pages | Very High | Primary ranking targets |
| Product pages | High | Long-tail, specific intent |
| Collection pages | High | Curated themes |
| Blog/Guides | High | Top-of-funnel |
| Cart/Checkout | None | Conversion-only |
| Account pages | None | Logged-in users |
| Size guide | Medium | Can capture searches |

> **Source**: [BigCommerce - E-commerce SEO](https://www.bigcommerce.com/articles/ecommerce/ecommerce-seo/)

### Local Business

| Page | SEO Priority | Notes |
|------|--------------|-------|
| Homepage | Very High | "[service] + [city]" |
| Service pages | Very High | Individual services |
| Location pages | Very High | Multi-location businesses |
| About page | Medium | "[company name]" searches |
| Contact page | Low | People use GMB |
| Blog | High | Local content marketing |
| Reviews page | Medium | "[company] reviews" |

> **Source**: [Moz - Local SEO Guide](https://moz.com/learn/seo/local)

### Affiliate / Content Sites

| Page | SEO Priority | Notes |
|------|--------------|-------|
| Homepage | Medium | Often not the entry point |
| Category hubs | Very High | Topic clusters |
| Comparison articles | Very High | Decision-stage content |
| Review articles | Very High | Product-specific searches |
| "Best of" lists | Very High | High volume, competitive |
| Tool pages | High | Capture intent |
| About page | Low | Trust, not traffic |

> **Source**: [Authority Hacker - Affiliate SEO](https://www.authorityhacker.com/)

---

## Technical SEO Decisions

### Indexing Decisions

| Action | When to Use |
|--------|-------------|
| **Index** | Pages you want to rank |
| **Noindex** | Thin pages, duplicates, paid LPs, internal tools |
| **Canonical** | Preferred version of duplicate content |
| **robots.txt block** | Prevent crawling (use carefully) |

### Common Indexing Mistakes

| Mistake | Impact | Fix |
|---------|--------|-----|
| Noindexing important pages | Pages don't rank | Audit meta robots |
| No canonicals on filters | Duplicate content | Add canonicals |
| Blocking CSS/JS in robots | Rendering issues | Allow crawling |
| Indexing paginated pages | Thin content issues | Canonical to main or noindex |
| Indexing search results | Doorway pages | Noindex search pages |

---

## Schema Markup Priority

### High Priority (Always Implement)

| Schema Type | Pages | Benefit |
|-------------|-------|---------|
| **Organization** | Homepage | Knowledge panel |
| **Product** | Product pages | Rich snippets |
| **Article** | Blog posts | Rich snippets |
| **BreadcrumbList** | All pages | Navigation in SERPs |
| **FAQ** | FAQ pages | Rich snippets |
| **LocalBusiness** | Local sites | Local pack |

### Medium Priority (If Applicable)

| Schema Type | Pages | Benefit |
|-------------|-------|---------|
| **Review** | Reviews | Star ratings |
| **HowTo** | Tutorials | Rich snippets |
| **Event** | Events | Event listings |
| **Recipe** | Recipes | Rich snippets |
| **Course** | Courses | Course listings |

> **Source**: [Schema.org](https://schema.org/) and [Google - Structured Data](https://developers.google.com/search/docs/advanced/structured-data)

---

## Content Quality Signals (E-E-A-T)

Google evaluates content quality via E-E-A-T:

| Signal | What It Means | How to Demonstrate |
|--------|---------------|-------------------|
| **E**xperience | First-hand experience | Show you've done/used it |
| **E**xpertise | Knowledge depth | Author bios, credentials |
| **A**uthoritativeness | Recognition by others | Citations, links, mentions |
| **T**rustworthiness | Accuracy, transparency | Sources, disclosures, contact |

### E-E-A-T Matters Most For

- **YMYL** (Your Money or Your Life) topics
- Health, finance, legal, safety content
- Product reviews and comparisons
- News and current events

> **Source**: [Google Search Quality Guidelines](https://developers.google.com/search/docs/fundamentals/creating-helpful-content)

---

## SEO vs. Conversion: Finding Balance

### When They Conflict

| SEO Wants | Conversion Wants | Resolution |
|-----------|------------------|------------|
| More content | Less distraction | Test content placement |
| Navigation links | Focused journey | Strategic linking |
| External links | Keep on page | Open in new tab |
| Long-form content | Quick decisions | Scannable formatting |
| Multiple CTAs | Single focus | Contextual CTAs |

### Best Practice: Segment by Intent

- **Informational pages** → Optimize for SEO, soft CTAs
- **Commercial pages** → Balance SEO + conversion
- **Transactional pages** → Conversion first, SEO secondary
- **Navigational pages** → User experience first

---

## Measurement Framework

### SEO KPIs by Page Type

| Page Type | Primary KPI | Secondary KPIs |
|-----------|-------------|----------------|
| Blog/Content | Organic traffic | Rankings, engagement |
| Product pages | Organic revenue | Traffic, conversions |
| Category pages | Organic traffic | Rankings, CTR |
| Comparison pages | Conversions | Traffic, time on page |
| Local pages | Local pack visibility | Calls, directions |

### Attribution Challenges

SEO often assists conversions rather than closing them:

```
Blog Post (SEO) → Email Signup → Nurture → Demo → Sale
                  └── SEO gets assist, not credit
```

**Solution**: Use assisted conversion reports in GA4 or multi-touch attribution models.

---

## Checklist: SEO Investment Decision

Before optimizing a page for SEO:

- [ ] Does this page have a purpose that organic traffic supports?
- [ ] Do people actually search for this content? (Check search volume)
- [ ] Can we create the best result for this query?
- [ ] Is ranking achievable given competition?
- [ ] Will traffic from this page drive business outcomes?
- [ ] Can we track and attribute SEO success?

If you answer "no" to any of these, reconsider the SEO investment.

---

## Sources

- [Google Search Central - How Search Works](https://developers.google.com/search/docs/fundamentals/how-search-works)
- [Google Search Quality Evaluator Guidelines](https://static.googleusercontent.com/media/guidelines.raterhub.com/en//searchqualityevaluatorguidelines.pdf)
- [Ahrefs - SEO Fundamentals](https://ahrefs.com/blog/seo-basics/)
- [Moz - Beginner's Guide to SEO](https://moz.com/beginners-guide-to-seo)
- [Search Engine Journal - E-E-A-T Guide](https://www.searchenginejournal.com/google-eat/)
- [Backlinko - SEO Best Practices](https://backlinko.com/seo-this-year)
