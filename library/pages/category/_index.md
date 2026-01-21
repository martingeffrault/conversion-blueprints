# Category & Hub Pages

> **Purpose**: Organize and present collections of related content
> **Types**: Product categories, content hubs, topic pages, resource centers
> **Principle**: Help users navigate and discover while building topical authority

---

## What Are Category Pages?

Category pages serve as organized entry points to collections of related content—products, articles, services, or resources. They bridge the gap between high-level navigation and individual detail pages.

### Category Page Types

| Type | Purpose | Example |
|------|---------|---------|
| **Product Category** | Browse products by type | "/shoes/running" |
| **Content Hub** | Explore topic content | "/guides/seo" |
| **Service Category** | Browse service offerings | "/services/marketing" |
| **Resource Center** | Access learning materials | "/resources/templates" |
| **Knowledge Base** | Find help articles | "/help/billing" |

---

## Anatomy of a Category Page

### Essential Elements

```
CATEGORY PAGE STRUCTURE

┌─────────────────────────────────────────────────┐
│ Breadcrumbs: Home > Category > Subcategory      │
├─────────────────────────────────────────────────┤
│ HERO SECTION                                    │
│ ├── Category Title (H1)                         │
│ ├── Description/Value Proposition               │
│ └── Quick Filters or Search (optional)          │
├─────────────────────────────────────────────────┤
│ NAVIGATION AIDS                                 │
│ ├── Subcategory Links                           │
│ ├── Filter/Sort Options                         │
│ └── View Toggle (grid/list)                     │
├─────────────────────────────────────────────────┤
│ CONTENT GRID                                    │
│ ├── Item Cards (products/articles/services)     │
│ ├── Featured/Promoted Items (optional)          │
│ └── Pagination or Load More                     │
├─────────────────────────────────────────────────┤
│ SUPPORTING CONTENT                              │
│ ├── Related Categories                          │
│ ├── Popular Items                               │
│ └── SEO Content Block                           │
└─────────────────────────────────────────────────┘
```

### Header Section

| Element | Purpose | Implementation |
|---------|---------|----------------|
| **Breadcrumbs** | Navigation context | Schema.org markup |
| **H1 Title** | Clear category name | Include keyword |
| **Description** | Value proposition | 1-2 sentences |
| **Item count** | Set expectations | "Showing 48 products" |

### Filtering & Sorting

| Feature | Best Practices |
|---------|----------------|
| **Filters** | Most relevant attributes first, collapsible on mobile |
| **Sort options** | Relevance, price, newest, rating, popularity |
| **Active filters** | Show applied filters, easy to clear |
| **Filter counts** | Show number of results per filter option |

### Content Grid

| Consideration | Recommendation |
|---------------|----------------|
| **Card design** | Consistent, scannable, key info visible |
| **Grid columns** | 3-4 desktop, 2 tablet, 1-2 mobile |
| **Image ratio** | Consistent aspect ratios (1:1 or 4:3) |
| **Pagination** | 24-48 items per page, or infinite scroll |

---

## Category Page by Type

### E-commerce Product Category

**Key Elements:**
- Product count and filter summary
- Price range filter
- Availability filter
- Brand/attribute filters
- Quick add to cart
- Price display
- Rating stars
- Sale badges

**Layout Example:**

```
┌──────────────────────────────────────────────┐
│ Running Shoes (128 products)                 │
│ [Filter] [Sort: Best Selling ▼]              │
├──────────────────────────────────────────────┤
│ SIDEBAR          │  PRODUCT GRID             │
│ ├ Price Range    │  ┌────┐ ┌────┐ ┌────┐    │
│ ├ Brand          │  │ 🏃 │ │ 🏃 │ │ 🏃 │    │
│ ├ Size           │  │$129│ │$89 │ │$199│    │
│ ├ Color          │  │★★★★│ │★★★ │ │★★★★★    │
│ └ Rating         │  └────┘ └────┘ └────┘    │
└──────────────────────────────────────────────┘
```

### Content Hub / Topic Page

**Key Elements:**
- Topic introduction
- Featured/pillar content
- Content by subtopic
- Recent articles
- Popular articles
- Related topics

**Layout Example:**

```
┌──────────────────────────────────────────────┐
│ SEO Guide: Everything You Need to Know       │
│ Master search engine optimization with our   │
│ comprehensive guides and tutorials.          │
├──────────────────────────────────────────────┤
│ FEATURED GUIDE                               │
│ ┌──────────────────────────────────────────┐ │
│ │ Complete SEO Guide 2025 [PILLAR]         │ │
│ └──────────────────────────────────────────┘ │
├──────────────────────────────────────────────┤
│ BROWSE BY TOPIC                              │
│ [On-Page] [Technical] [Link Building] [Local]│
├──────────────────────────────────────────────┤
│ LATEST GUIDES                                │
│ ┌────┐ ┌────┐ ┌────┐ ┌────┐                 │
│ │ 📄 │ │ 📄 │ │ 📄 │ │ 📄 │                 │
│ └────┘ └────┘ └────┘ └────┘                 │
└──────────────────────────────────────────────┘
```

### Service Category

**Key Elements:**
- Service overview
- Service cards with descriptions
- Pricing indicators
- CTA for each service
- Case studies/social proof
- Comparison if applicable

### Knowledge Base / Help Center

**Key Elements:**
- Search prominently placed
- Popular articles
- Categories with icons
- Article counts per category
- Quick links to common issues

---

## Mobile Optimization

### Mobile-Specific Patterns

| Pattern | Implementation |
|---------|----------------|
| **Sticky filter bar** | Pin filters to top on scroll |
| **Filter drawer** | Full-screen filter panel |
| **Load more** | Instead of pagination |
| **Swipe actions** | Quick add/favorite |
| **Compact cards** | Essential info only |

### Mobile Layout

```
MOBILE CATEGORY PAGE

┌─────────────────────┐
│ Category Title      │
│ [Filters ▼] [Sort ▼]│
├─────────────────────┤
│ ┌─────────────────┐ │
│ │ Item 1          │ │
│ │ $99 ★★★★        │ │
│ └─────────────────┘ │
│ ┌─────────────────┐ │
│ │ Item 2          │ │
│ │ $149 ★★★★★      │ │
│ └─────────────────┘ │
│                     │
│ [Load More]         │
└─────────────────────┘
```

---

## SEO for Category Pages

### On-Page SEO

| Element | Best Practice |
|---------|---------------|
| **Title tag** | "[Category] - [Benefit/Modifier] | [Brand]" |
| **H1** | Primary keyword, descriptive |
| **Meta description** | Include category, count, value prop |
| **URL** | Short, keyword-rich: /category/subcategory |
| **Content** | Unique intro + SEO block at bottom |

### Technical SEO

| Consideration | Implementation |
|---------------|----------------|
| **Canonicals** | Handle filtered URL duplicates |
| **Pagination** | rel="next/prev" or single page with infinite scroll |
| **Faceted navigation** | Block low-value filter combos from indexing |
| **Internal linking** | Link to subcategories and top items |

### Schema Markup

```html
<!-- Product Category -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "CollectionPage",
  "name": "Running Shoes",
  "description": "...",
  "breadcrumb": {...}
}
</script>

<!-- Breadcrumbs -->
<script type="application/ld+json">
{
  "@context": "https://schema.org",
  "@type": "BreadcrumbList",
  "itemListElement": [
    {"@type": "ListItem", "position": 1, "name": "Home", "item": "..."},
    {"@type": "ListItem", "position": 2, "name": "Shoes", "item": "..."},
    {"@type": "ListItem", "position": 3, "name": "Running"}
  ]
}
</script>
```

---

## Conversion Optimization

### Above-the-Fold Priorities

| Priority | Element |
|----------|---------|
| 1 | Clear category title and context |
| 2 | First 2-4 items visible |
| 3 | Filter/sort accessible |
| 4 | Trust signals (ratings, reviews count) |

### Card Design for Conversion

| Element | Impact |
|---------|--------|
| **Quality images** | Primary attention driver |
| **Price visibility** | Reduces friction |
| **Rating display** | Social proof |
| **Stock status** | Creates urgency |
| **Quick actions** | Reduces steps to conversion |

### Empty State Handling

When filters return no results:

```
┌─────────────────────────────────────────┐
│ No products match your filters          │
│                                         │
│ Try:                                    │
│ • Removing some filters                 │
│ • Checking another category             │
│                                         │
│ [Clear All Filters]                     │
│                                         │
│ You might also like:                    │
│ [Related Category] [Popular Items]      │
└─────────────────────────────────────────┘
```

---

## Performance Considerations

### Loading Strategy

| Content | Strategy |
|---------|----------|
| **Initial items** | Server-render first 12-24 |
| **Images** | Lazy load below fold |
| **Filters** | Client-side for speed |
| **Additional items** | Load on scroll/click |

### Image Optimization

| Practice | Benefit |
|----------|---------|
| Responsive images | Right size for device |
| WebP/AVIF format | Smaller file size |
| Lazy loading | Faster initial load |
| Placeholder/skeleton | Better perceived speed |

---

## Common Mistakes

| Mistake | Solution |
|---------|----------|
| No content for SEO | Add category description |
| Thin pages | Minimum viable content + items |
| Poor mobile filters | Full-screen filter drawer |
| No empty state | Helpful fallback UI |
| Slow loading | Lazy load + pagination |
| Duplicate content | Canonical URLs for filters |

---

## Category Page Checklist

### Structure
- [ ] Clear H1 with category name
- [ ] Breadcrumb navigation
- [ ] Category description
- [ ] Item count displayed
- [ ] Logical subcategory structure

### Navigation
- [ ] Relevant filters
- [ ] Sort options
- [ ] Clear applied filters
- [ ] Easy filter clearing
- [ ] Pagination or load more

### Cards
- [ ] Quality images
- [ ] Key info visible (price, rating)
- [ ] Consistent layout
- [ ] Clear CTAs or links
- [ ] Responsive design

### SEO
- [ ] Unique meta title/description
- [ ] Schema markup
- [ ] Canonical handling
- [ ] Internal links to items
- [ ] SEO content block

### Mobile
- [ ] Touch-friendly filters
- [ ] Appropriate card size
- [ ] Sticky navigation
- [ ] Fast loading

---

## Key Takeaways

1. **Navigation hub**: Category pages help users find what they want
2. **SEO opportunity**: Rank for category-level keywords
3. **Conversion point**: Make items easy to evaluate and act on
4. **Mobile-first**: Filters and browsing must work on mobile
5. **Performance matters**: Fast loading keeps users engaged

---

## Cross-References

- [E-commerce Patterns](../industry/ecommerce.md)
- [Information Architecture](../../content/information-architecture.md)
- [Card Components](../../components/cards.md)
- [Navigation Patterns](../../components/navigation.md)
