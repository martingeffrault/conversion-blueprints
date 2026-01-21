# E-commerce: Marketplace Architecture

> **Model**: Multi-vendor platform connecting buyers and sellers
> **Examples**: Etsy, Amazon, eBay, Airbnb, Uber, Fiverr, Upwork
> **Characteristics**: Two-sided, network effects, trust mechanisms, commission-based

---

## Marketplace Types

| Type | Examples | Key Challenge |
|------|----------|---------------|
| **Product marketplace** | Etsy, Amazon, eBay | Product discovery, fulfillment |
| **Service marketplace** | Upwork, Fiverr, Thumbtack | Quality matching, trust |
| **Rental marketplace** | Airbnb, Turo | Availability, verification |
| **B2B marketplace** | Alibaba, Faire | Volume, payment terms |

---

## Two-Sided Architecture

Marketplaces serve two distinct audiences:

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│                        MARKETPLACE                              │
│                                                                 │
│  ┌─────────────────────────┐    ┌─────────────────────────┐    │
│  │                         │    │                         │    │
│  │   BUYER EXPERIENCE      │    │   SELLER EXPERIENCE     │    │
│  │                         │    │                         │    │
│  │   • Browse/Search       │    │   • Seller Dashboard    │    │
│  │   • Product Pages       │    │   • Listing Management  │    │
│  │   • Checkout            │    │   • Orders/Fulfillment  │    │
│  │   • Order Tracking      │    │   • Analytics           │    │
│  │   • Reviews             │    │   • Payouts             │    │
│  │                         │    │                         │    │
│  └─────────────────────────┘    └─────────────────────────┘    │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Site Architecture

### Buyer-Facing Pages

```
/                           Homepage (discovery-focused)
├── /browse/                Category browsing
│   ├── /browse/[category]/
│   └── /browse/[category]/[subcategory]/
├── /search/                Search results
├── /product/[slug]/        Product/listing pages
├── /seller/[username]/     Seller storefront
├── /cart/                  Shopping cart
├── /checkout/              Checkout flow
└── /account/               Buyer account
    ├── /account/orders/
    ├── /account/messages/
    ├── /account/favorites/
    └── /account/reviews/
```

### Seller-Facing Pages

```
/sell/                      Seller landing page
├── /sell/start/            Seller onboarding
├── /dashboard/             Seller dashboard
│   ├── /dashboard/listings/
│   │   ├── /dashboard/listings/new/
│   │   └── /dashboard/listings/[id]/edit/
│   ├── /dashboard/orders/
│   ├── /dashboard/analytics/
│   ├── /dashboard/payouts/
│   ├── /dashboard/messages/
│   └── /dashboard/settings/
└── /seller-help/           Seller documentation
```

### Platform Pages

```
├── /about/                 Platform story
├── /how-it-works/          For both buyers and sellers
├── /trust-safety/          Trust & safety policies
├── /blog/                  Platform blog
├── /press/                 Press & media
└── /careers/               Jobs
```

### Legal & Support

```
├── /help/                  Help center
├── /contact/               Contact support
├── /privacy/
├── /terms/
├── /seller-terms/          Seller-specific terms
└── /prohibited-items/      Policy pages
```

---

## Homepage Structure (Marketplace)

```
┌─────────────────────────────────────────────────────────────────┐
│ [Logo]     Categories ▼   [   Search...                 🔍]    │
│                                             [Sell] [Login]      │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌──────────────────────────────────────────────────────────┐  │
│  │                                                          │  │
│  │            Find unique [products/services]               │  │
│  │            from [seller type] worldwide                  │  │
│  │                                                          │  │
│  │  [          Search for anything...            ] [Search] │  │
│  │                                                          │  │
│  │  Popular: [Tag] [Tag] [Tag] [Tag] [Tag]                 │  │
│  │                                                          │  │
│  └──────────────────────────────────────────────────────────┘  │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Browse Categories                                              │
│                                                                 │
│  ┌─────────┐  ┌─────────┐  ┌─────────┐  ┌─────────┐  ┌──────┐ │
│  │[Image]  │  │[Image]  │  │[Image]  │  │[Image]  │  │[Image]│ │
│  │Category │  │Category │  │Category │  │Category │  │Categ. │ │
│  └─────────┘  └─────────┘  └─────────┘  └─────────┘  └──────┘ │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Editor's Picks                                                 │
│                                                                 │
│  [Product] [Product] [Product] [Product] [Product] [Product]   │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Recently Viewed / Recommended for You                          │
│                                                                 │
│  [Product] [Product] [Product] [Product]                       │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Top Sellers This Week                                          │
│                                                                 │
│  ┌─────────────────┐  ┌─────────────────┐                      │
│  │ [Seller Avatar] │  │ [Seller Avatar] │                      │
│  │ Seller Name     │  │ Seller Name     │                      │
│  │ ⭐ 4.9 (500+)   │  │ ⭐ 4.8 (320+)   │                      │
│  │ [Visit Shop]    │  │ [Visit Shop]    │                      │
│  └─────────────────┘  └─────────────────┘                      │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Why Shop With Us                                               │
│                                                                 │
│  🔒 Secure payments  │  ✓ Verified sellers  │  💬 24/7 support │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌──────────────────────────────────────────────────────────┐  │
│  │                                                          │  │
│  │  Start Selling Today                                     │  │
│  │                                                          │  │
│  │  Join [X]+ sellers earning on [Platform]                 │  │
│  │                                                          │  │
│  │  [Start Selling]                                         │  │
│  │                                                          │  │
│  └──────────────────────────────────────────────────────────┘  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Key Marketplace Elements

### 1. Search & Discovery

Search is the primary navigation for marketplaces:

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Search: "handmade jewelry"                            ] [🔍] │
│                                                                 │
│  Filters:                                                       │
│  [Price ▼] [Shipping ▼] [Seller Rating ▼] [Location ▼]         │
│                                                                 │
│  "handmade jewelry" — 12,345 results                           │
│  Sort: [Best Match ▼]                                          │
│                                                                 │
│  ┌─────────┐  ┌─────────┐  ┌─────────┐  ┌─────────┐           │
│  │[Product]│  │[Product]│  │[Product]│  │[Product]│           │
│  │ $XX     │  │ $XX     │  │ $XX     │  │ $XX     │           │
│  │ ⭐ 4.8  │  │ ⭐ 5.0  │  │ ⭐ 4.7  │  │ ⭐ 4.9  │           │
│  │ Seller  │  │ Seller  │  │ Seller  │  │ Seller  │           │
│  └─────────┘  └─────────┘  └─────────┘  └─────────┘           │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Key filters:**
- Price range
- Shipping options (free, location)
- Seller rating
- Delivery time
- Category-specific (size, color, etc.)

### 2. Trust & Safety

Trust is the #1 challenge for marketplaces:

| Trust Element | Buyer Side | Seller Side |
|---------------|------------|-------------|
| **Verification** | ID, payment verification | ID, tax info, address |
| **Reviews** | Rate sellers & products | Rate buyers |
| **Escrow** | Payment held until delivery | Payment released on completion |
| **Policies** | Buyer protection, refunds | Seller protection |
| **Communication** | Message before buying | Respond to inquiries |

### 3. Listing Page Structure

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  ┌──────────────────────┐  ┌──────────────────────────────┐    │
│  │                      │  │                              │    │
│  │  [Product Gallery]   │  │  Product Title               │    │
│  │                      │  │  ⭐⭐⭐⭐⭐ 4.9 (128 reviews) │    │
│  │  [img][img][img]     │  │                              │    │
│  │                      │  │  $XX.XX                      │    │
│  │                      │  │                              │    │
│  │                      │  │  [Options/Variants]          │    │
│  │                      │  │                              │    │
│  │                      │  │  Quantity: [1] [-][+]        │    │
│  │                      │  │                              │    │
│  │                      │  │  [Add to Cart]               │    │
│  │                      │  │                              │    │
│  │                      │  │  ✓ Free shipping             │    │
│  │                      │  │  📦 Ships in 1-3 days        │    │
│  │                      │  │  ↩️ 30-day returns           │    │
│  │                      │  │                              │    │
│  └──────────────────────┘  └──────────────────────────────┘    │
│                                                                 │
│  ─────────────────────────────────────────────────────────────  │
│                                                                 │
│  Seller Information                                             │
│                                                                 │
│  ┌──────────────────────────────────────────────────────────┐  │
│  │  [Avatar]  ShopName                                      │  │
│  │            ⭐ 4.9 (500+ sales)  │  Member since 2020     │  │
│  │            Usually responds within 1 hour                │  │
│  │            [Message Seller] [Visit Shop]                 │  │
│  └──────────────────────────────────────────────────────────┘  │
│                                                                 │
│  ─────────────────────────────────────────────────────────────  │
│                                                                 │
│  Description                                                    │
│  [Full product description]                                     │
│                                                                 │
│  ─────────────────────────────────────────────────────────────  │
│                                                                 │
│  Shipping & Policies                                            │
│  [Shipping info] [Returns] [Seller policies]                   │
│                                                                 │
│  ─────────────────────────────────────────────────────────────  │
│                                                                 │
│  Reviews (128)                                                  │
│  [Review cards with seller responses]                           │
│                                                                 │
│  ─────────────────────────────────────────────────────────────  │
│                                                                 │
│  More from This Seller                                          │
│  [Products]                                                     │
│                                                                 │
│  Similar Items                                                  │
│  [Products]                                                     │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### 4. Seller Dashboard

```
┌─────────────────────────────────────────────────────────────────┐
│ [Logo]                                    [View Shop] [Help] [?]│
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌────────────────┐  ┌──────────────────────────────────────┐  │
│  │                │  │                                      │  │
│  │  Dashboard     │  │  Welcome back, [Name]!               │  │
│  │  Listings      │  │                                      │  │
│  │  Orders        │  │  ┌────────────┐  ┌────────────┐     │  │
│  │  Messages (3)  │  │  │ $1,234     │  │ 23         │     │  │
│  │  Analytics     │  │  │ This month │  │ Orders     │     │  │
│  │  Payouts       │  │  └────────────┘  └────────────┘     │  │
│  │  Settings      │  │                                      │  │
│  │                │  │  ┌────────────┐  ┌────────────┐     │  │
│  │                │  │  │ 4.9 ⭐     │  │ 98%        │     │  │
│  │                │  │  │ Rating     │  │ Ship on time│     │  │
│  │                │  │  └────────────┘  └────────────┘     │  │
│  │                │  │                                      │  │
│  │                │  │  To-Do:                              │  │
│  │                │  │  • 5 orders to ship                  │  │
│  │                │  │  • 3 messages to respond             │  │
│  │                │  │  • 2 listings need attention         │  │
│  │                │  │                                      │  │
│  └────────────────┘  └──────────────────────────────────────┘  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## SEO for Marketplaces

### Massive SEO Opportunity

Marketplaces can dominate SEO due to:
- Thousands/millions of unique product pages
- User-generated content (reviews, descriptions)
- Fresh content constantly added
- Long-tail keyword coverage

### SEO-Optimized URL Structure

```
/[category]/[subcategory]/                    (category pages)
/[category]/[product-keyword]-[id]/           (product pages)
/seller/[seller-name]/                        (seller pages)
/search?q=[query]                             (search results - noindex)
```

### Key SEO Pages

| Page Type | Keyword Target | Notes |
|-----------|----------------|-------|
| Category pages | "[category] for sale" | Main ranking targets |
| Subcategory | "[specific item] online" | Long-tail |
| Product pages | "[exact product name]" | Often unique |
| Seller pages | "[seller name] shop" | Branded |
| Guide content | "how to buy [category]" | Top-of-funnel |

### SEO Challenges

- Duplicate content from similar listings
- Thin content on sparse listings
- Crawl budget management
- Faceted navigation (duplicate URLs)

**Solutions:**
- Canonical tags on variations
- Minimum content requirements for listings
- robots.txt for filtered URLs
- Pagination with rel=prev/next

---

## Conversion Metrics

### Marketplace-Specific Metrics

| Metric | Description | Target |
|--------|-------------|--------|
| **GMV** | Gross Merchandise Value | Growth metric |
| **Take rate** | Commission percentage | 10-20% typical |
| **Buyer conversion** | Visitors to purchasers | 2-5% |
| **Seller activation** | New sellers listing | 70%+ |
| **Liquidity** | Listings that sell | 30%+ |
| **Repeat purchase** | Buyers who return | 30%+ |

### The "Chicken and Egg" Problem

Marketplaces must balance:
1. **Supply** (sellers) — Need products to attract buyers
2. **Demand** (buyers) — Need buyers to attract sellers

**Common solutions:**
- Start single-player (useful even without other side)
- Seed supply first (recruit sellers before launch)
- Geographic focus (density in one area first)
- Vertical focus (one category first)

---

## Sources

- [a16z - Marketplace Handbook](https://a16z.com/marketplace-100/)
- [NFX - Network Effects Bible](https://www.nfx.com/post/network-effects-bible)
- [Lenny's Newsletter - Marketplace strategies](https://www.lennysnewsletter.com/)
- [Etsy, Airbnb, Uber case studies](https://www.cbinsights.com/research/)
- [Shopify - Marketplace trends](https://www.shopify.com/enterprise/marketplace-trends)
