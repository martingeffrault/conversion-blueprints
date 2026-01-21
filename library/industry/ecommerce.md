# E-Commerce Patterns

> **Purpose**: Proven patterns from successful online retailers
> **Focus**: Product discovery, conversion optimization, and purchase completion
> **Principle**: Reduce friction at every step — every click is an opportunity to lose a customer

---

## Industry Leaders Analysis

### By Category

| Category | Leaders | Key Patterns |
|----------|---------|--------------|
| **Marketplace** | Amazon, eBay, Etsy | Vast selection, reviews, Prime/fast shipping |
| **Fashion** | ASOS, Zara, Net-a-Porter | Visual-first, size guides, lookbooks |
| **DTC Brands** | Glossier, Warby Parker, Casper | Story-driven, social proof, simplicity |
| **Electronics** | Best Buy, B&H, Newegg | Specs comparison, expert reviews, bundles |
| **Home** | Wayfair, IKEA, Williams-Sonoma | Room visualization, dimensions, lifestyle |
| **Luxury** | Farfetch, Mr Porter, Mytheresa | Editorial content, exclusivity, white space |
| **Grocery** | Instacart, Amazon Fresh, Ocado | Speed, substitutions, recurring orders |

---

## Homepage Patterns

### Hero Section

**Best performers**: Product showcase, not lifestyle imagery.

```
┌─────────────────────────────────────────────────────────────────┐
│  [Seasonal/Promo Banner - Dismissible]                          │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  [Product Hero]              "New Arrivals"                     │
│  ┌─────────────┐                                               │
│  │   Product   │             Up to 30% off                      │
│  │    Image    │             select styles                      │
│  │             │                                               │
│  └─────────────┘             [Shop Now]                         │
│                                                                 │
│  Free shipping on orders $50+ | Easy 30-day returns            │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Key elements**:
- Promo bar (urgency, free shipping threshold)
- Hero featuring actual products (not just lifestyle)
- Value proposition visible immediately
- Trust badges below fold line

### Navigation Patterns

| Pattern | Used By | Best For |
|---------|---------|----------|
| Mega menu | Amazon, Target, Walmart | Large catalogs (500+ SKUs) |
| Simple dropdown | Glossier, Everlane | Small catalogs (<100 SKUs) |
| Visual categories | IKEA, Wayfair | Visual products |
| Search-first | Amazon, eBay | Known-item shopping |

**Mega Menu Structure**:
```
┌─────────────────────────────────────────────────────────────────┐
│ Women ▼  Men  Kids  Sale  [Search_________________] Cart (3)    │
├─────────────────────────────────────────────────────────────────┤
│ ┌─────────────────────────────────────────────────────────────┐ │
│ │ Clothing      Shoes         Accessories   Featured          │ │
│ │ ─────────     ──────        ───────────   ────────          │ │
│ │ Dresses       Sneakers      Bags          [Image]           │ │
│ │ Tops          Heels         Jewelry       New Arrivals      │ │
│ │ Pants         Boots         Scarves                         │ │
│ │ Jackets       Sandals       Watches       [Image]           │ │
│ │ Activewear    Flats         Belts         Best Sellers      │ │
│ │ View All →    View All →    View All →                      │ │
│ └─────────────────────────────────────────────────────────────┘ │
└─────────────────────────────────────────────────────────────────┘
```

---

## Category Page Patterns

### Filter Sidebar

**Optimal order** (by usage frequency):
1. Category/Subcategory
2. Price range
3. Size (fashion)
4. Color
5. Brand
6. Rating
7. Availability
8. Special attributes

**Filter UX Best Practices**:

| Pattern | Impact | Notes |
|---------|--------|-------|
| Faceted search | +12% CVR | Show count per filter |
| Sticky filters | +8% engagement | Mobile: use bottom sheet |
| "Clear all" button | Reduces frustration | Always visible |
| Applied filters visible | Orientation | Chips with X to remove |
| Price slider | +15% engagement | Show min/max dynamically |

### Product Grid

| Grid Style | Best For | Desktop | Mobile |
|------------|----------|---------|--------|
| Dense (4-5 col) | High-volume browsing | 4-5 products | 2 products |
| Standard (3-4 col) | Fashion, lifestyle | 3-4 products | 2 products |
| Spacious (2-3 col) | Luxury, high-ticket | 2-3 products | 1-2 products |
| List view | Tech specs, comparisons | Full width | Full width |

**Product Card Elements**:

```
┌─────────────────────────────┐
│  [Wishlist ♡]    [Quick View]│
│  ┌───────────────────────┐  │
│  │                       │  │
│  │     Product Image     │  │
│  │   (hover: alt view)   │  │
│  │                       │  │
│  └───────────────────────┘  │
│  ● ● ●  (color variants)    │
│  Brand Name                 │
│  Product Title              │
│  ⭐⭐⭐⭐⭐ (127)                │
│  $99.00  $129.00            │
│  [Add to Cart]              │
└─────────────────────────────┘
```

**Must-haves**:
- Hover state showing alternate image
- Quick add to cart (optional for complex products)
- Rating with review count
- Price (crossed out if on sale)
- Color/variant indicators
- Wishlist functionality

---

## Product Page Patterns

### Layout Options

**Split Layout** (most common):
```
┌─────────────────────────────────────────────────────────────────┐
│  Breadcrumb: Home > Women > Dresses > Midi Dresses              │
├─────────────────────────────────────────────────────────────────┤
│  ┌──────────────────┐  │  Brand Name                            │
│  │                  │  │  Product Title Here                    │
│  │   Main Image     │  │  ⭐⭐⭐⭐⭐ 4.8 (234 reviews)              │
│  │                  │  │                                        │
│  │                  │  │  $129.00  $159.00                      │
│  └──────────────────┘  │  or 4 payments of $32.25 with Klarna   │
│  ┌──┐┌──┐┌──┐┌──┐┌──┐  │                                        │
│  │  ││  ││  ││  ││  │  │  Color: Navy Blue                      │
│  └──┘└──┘└──┘└──┘└──┘  │  ● ● ● ●                               │
│                        │                                        │
│                        │  Size:  XS  S  [M]  L  XL              │
│                        │  [Size Guide]                          │
│                        │                                        │
│                        │  [    Add to Cart    ]                 │
│                        │  [    Buy Now         ]                │
│                        │                                        │
│                        │  ✓ Free shipping over $50              │
│                        │  ✓ Free returns within 30 days         │
│                        │  ✓ In stock - ships today              │
└─────────────────────────────────────────────────────────────────┘
```

### Gallery Best Practices

| Feature | Impact | Implementation |
|---------|--------|----------------|
| Multiple angles | +27% CVR | Min 4-5 images |
| Zoom on hover | +23% engagement | High-res required |
| Video | +80% CVR | Product in use |
| 360° view | +13% CVR | Furniture, electronics |
| Model/scale reference | -22% returns | Fashion especially |
| User-generated photos | +15% trust | In reviews section |

### Product Information

**Above fold** (critical):
- Title, brand
- Price (sale price prominent)
- Rating + review count
- Color/size selectors
- Add to cart
- Availability/shipping info

**Below fold** (scrollable):
- Full description
- Specifications/details
- Size guide
- Reviews
- Related products
- Recently viewed

### Trust Elements on Product Page

| Element | Placement | Impact |
|---------|-----------|--------|
| Stock status | Near ATC button | Creates urgency |
| Shipping estimate | Near ATC button | Sets expectations |
| Return policy | Near ATC button | Reduces risk |
| Security badges | Footer of product area | Subtle reassurance |
| Reviews snippet | Near price | Social proof |

---

## Cart Patterns

### Mini Cart (Header)

```
┌─────────────────────────────────────┐
│  Your Cart (3)                  [×] │
├─────────────────────────────────────┤
│  ┌────┐ Product Name                │
│  │img │ Size: M  Color: Blue        │
│  └────┘ Qty: [-] 1 [+]     $99.00  │
├─────────────────────────────────────┤
│  ┌────┐ Another Product             │
│  │img │ Size: L                     │
│  └────┘ Qty: [-] 2 [+]    $158.00  │
├─────────────────────────────────────┤
│  Subtotal:              $257.00     │
│  You're $43 away from free shipping │
│  ████████████░░░░░░ (85%)           │
├─────────────────────────────────────┤
│  [    View Cart    ]                │
│  [    Checkout     ]                │
└─────────────────────────────────────┘
```

### Cart Page

**Essential elements**:
- Product images (clickable back to PDP)
- Easy quantity adjustment
- Remove item option
- Save for later
- Order summary (sticky on scroll)
- Promo code field
- Shipping calculator
- Free shipping progress bar

**Cart abandonment reducers**:

| Element | Impact |
|---------|--------|
| Free shipping threshold progress | +18% AOV |
| Save for later | -12% abandonment |
| Guest checkout visible | -23% abandonment |
| Express checkout options | +35% mobile CVR |
| Security badges | +17% completion |

---

## Checkout Patterns

### Checkout Flow Options

| Flow | Best For | Conversion |
|------|----------|------------|
| Single-page | Low-cart-value, impulse | Highest |
| Multi-step (3 steps) | Standard e-commerce | High |
| Accordion | Medium complexity | Good |
| One-click (saved users) | Repeat customers | Excellent |

### Optimal Checkout Steps

```
[1. Information] → [2. Shipping] → [3. Payment]
      ●─────────────────○──────────────────○
```

**Step 1: Information**
- Email (for guest checkout)
- Shipping address (with autocomplete)
- Phone (optional unless required)

**Step 2: Shipping**
- Shipping method selection
- Delivery date estimates
- Gift options

**Step 3: Payment**
- Payment method selection
- Billing address (same as shipping default)
- Order review
- Place order CTA

### Checkout Trust Elements

| Element | Position | Impact |
|---------|----------|--------|
| Order summary (sticky) | Right sidebar | Orientation |
| Security badges | Near payment | +17% completion |
| Money-back guarantee | Near CTA | +11% CVR |
| Customer service contact | Footer | Reduces anxiety |
| Progress indicator | Top | Completion expectation |

### Payment Options

**Essential** (by market):
- Credit/debit cards
- PayPal
- Apple Pay / Google Pay
- Buy Now Pay Later (Klarna, Afterpay)
- Local payment methods (by region)

**Impact**: Offering 3+ payment methods = +30% CVR

---

## Mobile Commerce Patterns

### Mobile Statistics

| Metric | Value |
|--------|-------|
| Mobile commerce share | 73% of e-commerce traffic |
| Mobile conversion rate | 2.25% (vs 4.81% desktop) |
| Cart abandonment mobile | 85.65% |
| Checkout time acceptable | Under 3 minutes |

### Mobile-Specific Optimizations

| Pattern | Implementation |
|---------|----------------|
| Sticky ATC button | Fixed at bottom of screen |
| Bottom sheet filters | Instead of sidebar |
| Thumb-zone CTAs | Bottom 60% of screen |
| Simplified navigation | Hamburger + search prominent |
| Express checkout | Apple Pay / Google Pay prominent |
| Infinite scroll | With "back to top" button |

### Mobile Product Page

```
┌─────────────────────────────────────┐
│  ← Back                    ♡   [bag]│
├─────────────────────────────────────┤
│  ┌───────────────────────────────┐  │
│  │                               │  │
│  │      Product Image            │  │
│  │      (swipe for more)         │  │
│  │                               │  │
│  └───────────────────────────────┘  │
│           ● ○ ○ ○ ○                 │
│                                     │
│  Brand Name                         │
│  Product Title Here                 │
│  ⭐⭐⭐⭐⭐ 4.8 (234)                   │
│                                     │
│  $129.00  $159.00                   │
│  or 4 × $32.25 with Klarna          │
│                                     │
│  Color: Navy Blue                   │
│  [●] [○] [○] [○]                    │
│                                     │
│  Size: [Select Size ▼]              │
│                                     │
├─────────────────────────────────────┤
│  [     Add to Cart - $129    ]      │ ← Sticky
└─────────────────────────────────────┘
```

---

## Search & Discovery

### Search Box Patterns

| Feature | Impact |
|---------|--------|
| Autocomplete suggestions | +24% searches completed |
| Visual results (product images) | +38% click-through |
| Recent searches | +15% engagement |
| Trending searches | +12% discovery |
| Typo tolerance | Prevents 0-result pages |
| Filters in search results | +18% relevance |

### Zero Results Page

Never show an empty page. Include:
- Search suggestions
- Spelling corrections
- Popular categories
- Bestsellers
- Contact for help

---

## Conversion Rate Benchmarks

### By Category

| Category | Average CVR | Top Performers |
|----------|-------------|----------------|
| Food & Beverage | 5.5% | 8%+ |
| Health & Beauty | 3.5% | 6%+ |
| Fashion & Apparel | 2.7% | 4%+ |
| Electronics | 1.8% | 3%+ |
| Furniture | 0.9% | 2%+ |
| Luxury | 0.5% | 1.5%+ |

### By Device

| Device | Average CVR |
|--------|-------------|
| Desktop | 4.81% |
| Tablet | 3.88% |
| Mobile | 2.25% |

---

## Key Metrics to Track

| Metric | Target | Optimization Focus |
|--------|--------|-------------------|
| Conversion rate | 2-4% | Entire funnel |
| Add-to-cart rate | 8-12% | Product page |
| Cart abandonment | <70% | Cart + checkout |
| Average order value | Industry dependent | Upsells, bundles |
| Return rate | <10% | Product info, sizing |
| Customer acquisition cost | <30% of first order | Marketing efficiency |

---

## Common Mistakes to Avoid

| Mistake | Impact | Solution |
|---------|--------|----------|
| Required account creation | +26% abandonment | Guest checkout first |
| Hidden shipping costs | +48% abandonment | Show early (PDP or cart) |
| Complex checkout | +17% per step abandoned | 3 steps maximum |
| No mobile optimization | Lose 73% of traffic | Mobile-first design |
| Slow site speed | -7% CVR per second | Target <3s load |
| Poor search | Lose 43% of visitors | Invest in search UX |
| No reviews | -15% CVR | Enable reviews everywhere |

*Account creation and shipping data: [Baymard Institute](https://baymard.com/lists/cart-abandonment-rate). Site speed data: [Google/Deloitte](https://www2.deloitte.com/ie/en/pages/consulting/articles/milliseconds-make-millions.html).*

---

## Sources

- [Baymard Institute - E-Commerce UX](https://baymard.com/research)
- [Shopify E-Commerce Benchmark Report](https://www.shopify.com/research)
- [Google Retail Research](https://www.thinkwithgoogle.com/consumer-insights/consumer-trends/)
- [Statista E-Commerce Reports](https://www.statista.com/topics/871/online-shopping/)
- [NNGroup E-Commerce Studies](https://www.nngroup.com/topic/e-commerce/)
- [Klaviyo Benchmark Report](https://www.klaviyo.com/marketing-resources/benchmarks)
