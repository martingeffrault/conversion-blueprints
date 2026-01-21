# E-commerce Website Recipe

> **Business Type**: Online retail, physical or digital products
> **Primary Goals**: Drive purchases, reduce cart abandonment, maximize AOV
> **Revenue Model**: Product sales, subscriptions, bundles
> **Reference Sites**: Shopify stores, Amazon, Apple Store, Warby Parker, Glossier

---

## Choose Your Variant

E-commerce sites vary significantly based on business model. Choose the variant that matches yours:

| Variant | Best For | Key Characteristics | See Details |
|---------|----------|---------------------|-------------|
| **[DTC Brand](DTC-BRAND.md)** | Single brand, owned products | Brand story, community, premium pricing | [DTC-BRAND.md](DTC-BRAND.md) |
| **[Marketplace](MARKETPLACE.md)** | Multi-vendor platform | Two-sided, trust mechanisms, discovery | [MARKETPLACE.md](MARKETPLACE.md) |

The architecture below covers common elements applicable to most e-commerce sites.

---

## Site Architecture

### Core Pages (Must Have)

```
/                           Homepage (storefront)
├── /collections/           All collections/categories
│   └── /collections/[cat]/ Category pages
├── /products/              All products (optional)
│   └── /products/[slug]/   Individual product pages
├── /cart/                  Shopping cart
├── /checkout/              Checkout flow
├── /account/               Customer account
│   ├── /account/orders/    Order history
│   └── /account/addresses/ Saved addresses
├── /search/                Search results
├── /about/                 About/brand story
└── /contact/               Contact page
```

### Content & Trust Pages

```
├── /blog/                  Content hub
│   └── /blog/[post]/       Individual posts
├── /pages/
│   ├── /shipping/          Shipping information
│   ├── /returns/           Return policy
│   ├── /faq/               Frequently asked questions
│   ├── /size-guide/        Size guide (apparel)
│   └── /gift-cards/        Gift cards
```

### Legal Pages

```
├── /policies/
│   ├── /terms/             Terms of service
│   ├── /privacy/           Privacy policy
│   └── /accessibility/     Accessibility statement
```

---

## Page Hierarchy Diagram

```
                        ┌─────────────┐
                        │  HOMEPAGE   │
                        └──────┬──────┘
                               │
        ┌──────────────────────┼──────────────────────┐
        │                      │                      │
   ┌────▼────┐            ┌────▼────┐           ┌────▼────┐
   │  SHOP   │            │ CONTENT │           │ ACCOUNT │
   └────┬────┘            └────┬────┘           └────┬────┘
        │                      │                     │
   ┌────┼────┐            ┌────┼────┐          ┌────┼────┐
   │    │    │            │    │    │          │    │    │
Categories Products      Blog  About         Orders Addresses
   │         │            │
   └────┬────┘            └──────┬──────┐
        │                        │      │
   Product Page              Post   FAQ
```

---

## Navigation Structure

### Header Navigation

> "Simplify main navigation by limiting your top-level menu to 5-7 essential categories. Use clear, concise labels that customers will instantly understand."
>
> *Source: [Webstacks](https://www.webstacks.com/blog/ecommerce-web-design-best-practices)*

```
[Logo]  Shop ▼  Collections  New  Sale  About  [Search] [Cart]
```

### Mega Menu (Shop)

```
SHOP BY CATEGORY          FEATURED              NEW ARRIVALS
────────────────          ────────              ────────────
All Products              [Featured Image]      New This Week
Category 1                Best Sellers          Coming Soon
Category 2                Staff Picks
Category 3                Gift Ideas
Category 4
                         [Shop All →]
```

### Utility Navigation

```
[Search 🔍] [Account 👤] [Cart 🛒 (3)]
```

### Mobile Navigation

- Hamburger menu with categories
- Prominent search icon
- Sticky cart icon with item count
- Bottom navigation bar (optional):
  ```
  [Home] [Shop] [Search] [Account] [Cart]
  ```

### Footer Navigation

```
SHOP              HELP              COMPANY           CONNECT
────              ────              ───────           ───────
All Products      FAQ               About Us          Instagram
New Arrivals      Shipping          Careers           TikTok
Best Sellers      Returns           Press             Pinterest
Sale              Contact           Sustainability    Newsletter
Gift Cards        Size Guide

[Payment Icons]  [SSL Badge]

© 2024 Brand | Terms | Privacy | Accessibility
```

---

## Homepage Structure

### Recommended Section Order

```
1. Announcement Bar
   └── Shipping offer, sale, new launch

2. Header
   └── Logo, navigation, search, account, cart

3. Hero
   └── Hero image/video, headline, primary CTA

4. Trust Bar
   └── Shipping, returns, support promises

5. Featured Collections
   └── Category cards or product cards

6. New Arrivals / Best Sellers
   └── Product grid (8-12 products)

7. Category Navigation
   └── Visual category cards

8. Featured Product
   └── Hero product with story

9. Social Proof
   └── Reviews, press, Instagram

10. Content/Story
    └── Brand story, sustainability

11. Newsletter
    └── Email signup with incentive

12. Footer
    └── Navigation, legal, social
```

### Above the Fold

```
┌─────────────────────────────────────────────────────────────────┐
│ 🚚 Free shipping on orders over $50                    [✕]     │
├─────────────────────────────────────────────────────────────────┤
│ [Logo]    Shop ▼  New  Sale  About    [🔍] [👤] [🛒 2]        │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│              [Large Hero Image/Video]                           │
│                                                                 │
│                 NEW COLLECTION                                  │
│              Summer Essentials                                  │
│                                                                 │
│                [ Shop Now ]                                     │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Category Page Structure

### Page Elements

```
1. Breadcrumbs
   └── Home > Collections > Category

2. Category Header
   └── Title, description, product count

3. Filters & Sort
   └── Price, size, color, sort options

4. Product Grid
   └── Products with quick actions

5. Pagination / Load More
   └── Page numbers or infinite scroll

6. Category Description (SEO)
   └── Bottom content for SEO
```

### Filter Best Practices

> "Real-time filtering or sorting options allow users to exclude unnecessary items from hundreds of search results and guides users from the homepage to the most appropriate product page."
>
> *Source: [Ecorn Agency](https://www.ecorn.agency/blog/ecommerce-website-design-best-practices)*

**Essential Filters**:
| Category Type | Key Filters |
|---------------|-------------|
| Apparel | Size, Color, Price, Brand |
| Electronics | Price, Brand, Specs, Rating |
| Home | Room, Style, Price, Material |
| Beauty | Product Type, Skin Type, Concern |

**Filter UX**:
- Show applied filters clearly
- Enable multi-select
- Show result count after filtering
- Allow filter removal
- Remember filters during session

### Product Card Elements

```
┌─────────────────────────┐
│ [Product Image]         │
│ [Second Image on Hover] │
│                         │
│ Brand Name              │
│ Product Name            │
│ ★★★★☆ (42)             │
│ $99 $129 (23% off)      │
│                         │
│ [Color Swatches]        │
│ [Quick Add to Cart]     │
└─────────────────────────┘
```

---

## Product Page Structure

### Essential Elements

```
1. Breadcrumbs
   └── Home > Category > Product

2. Product Gallery
   └── Multiple images, zoom, video

3. Product Info
   └── Title, price, rating, description

4. Variant Selection
   └── Size, color, quantity

5. Add to Cart
   └── Primary CTA, availability

6. Product Details
   └── Tabs or accordion (details, sizing, care)

7. Social Proof
   └── Reviews section

8. Related Products
   └── "You May Also Like"

9. Recently Viewed
   └── Products user has viewed
```

### Product Info Layout

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  ┌─────────────────────┐   Product Title                        │
│  │                     │   Brand                                 │
│  │   [Main Image]      │   ★★★★★ (124 reviews)                 │
│  │                     │                                        │
│  │                     │   $129.00  $159.00                     │
│  │                     │                                        │
│  └─────────────────────┘   Color: Navy Blue                     │
│                            [●] [○] [○] [○]                      │
│  [thumb] [thumb] [thumb]                                        │
│                            Size: [Select Size ▼]                │
│                            Size Guide                           │
│                                                                 │
│                            Quantity: [- 1 +]                    │
│                                                                 │
│                            [ ADD TO CART ]                      │
│                            [ ♡ Add to Wishlist ]               │
│                                                                 │
│                            ✓ Free shipping over $50             │
│                            ✓ Free 30-day returns                │
│                            ✓ 2-year warranty                    │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Product Information Tabs

```
[Description] [Details & Care] [Sizing] [Reviews (124)]
─────────────────────────────────────────────────────────
│                                                       │
│  Product description with key features and benefits.  │
│                                                       │
│  • Feature 1                                          │
│  • Feature 2                                          │
│  • Feature 3                                          │
│                                                       │
└───────────────────────────────────────────────────────┘
```

---

## Cart & Checkout

### Cart Page Elements

```
1. Cart Header
   └── "Your Cart (3 items)"

2. Cart Items
   └── Image, name, variant, qty, price, remove

3. Cart Summary
   └── Subtotal, shipping estimate, total

4. Promo Code
   └── Code input field

5. CTAs
   └── Checkout, Continue Shopping

6. Trust Signals
   └── Secure payment, return policy

7. Cross-sells
   └── "Frequently Bought Together"
```

### Checkout Best Practices

**Reduce friction**:
- Guest checkout option
- Progress indicator (steps)
- Auto-fill addresses
- Multiple payment options
- Clear error messages

**Trust elements**:
- Security badges
- Money-back guarantee
- Clear shipping costs upfront
- Order summary visible throughout

**Checkout Flow**:
```
[Information] → [Shipping] → [Payment] → [Confirmation]
      1              2           3             4
```

---

## Trust & Conversion Elements

### Trust Signals Throughout

| Location | Trust Element |
|----------|---------------|
| Header | Security badge, reviews badge |
| Product Page | Stock status, shipping estimate |
| Cart | Secure checkout badge |
| Checkout | Payment icons, SSL badge |
| Footer | Return policy, contact info |

### Urgency & Scarcity

Use ethically and honestly:
- "Only 3 left in stock"
- "Sale ends in 2 days"
- "Selling fast"
- Limited edition labels

### Social Proof

- Product reviews with photos
- Star ratings everywhere
- "X people viewing this now"
- Instagram feed/UGC
- Press logos

---

## SEO Considerations

### Site Structure for SEO

> "Search engines rely on structure to understand and index ecommerce sites. Clear architecture improves crawlability, ensures important pages aren't buried, and supports logical internal linking."
>
> *Source: [BigCommerce](https://www.bigcommerce.com/articles/ecommerce-website-development/ecommerce-architecture/)*

**URL Structure**:
```
/collections/womens-clothing/
/products/summer-dress-blue/
/blog/summer-fashion-guide/
```

**Schema Markup**:
- `Product` schema with price, availability
- `Review` schema for ratings
- `BreadcrumbList` for navigation
- `Organization` for brand info

### Category Page SEO

- Unique title and meta description
- H1 with category name
- Intro content (100-200 words)
- Bottom content (300-500 words)
- Internal links to related categories

### Product Page SEO

- Unique product descriptions
- Alt text on all images
- Structured data
- Customer reviews (fresh content)
- Related product links

---

## Mobile Considerations

### Mobile-First Design

> "Since 79% of shoppers won't return to a site with poor performance, a strong website architecture with optimized site speed is crucial."
>
> *Source: [Parachute Design](https://parachutedesign.ca/blog/ecommerce-web-design-best-practices/)*

**Mobile Essentials**:
- Sticky add-to-cart on PDP
- Easy variant selection (buttons > dropdowns)
- Swipeable image galleries
- Simplified filters
- Touch-friendly buttons (44px min)
- Sticky bottom navigation
- Express checkout options (Apple Pay, etc.)

### Mobile Navigation

```
┌─────────────────────┐
│ [☰] [Logo] [🔍][🛒] │
└─────────────────────┘
```

---

## Performance

### Speed Optimization

> "A streamlined architecture leads to faster loading times and smoother interactions, which boost user experience and conversion rates."
>
> *Source: [BigCommerce](https://www.bigcommerce.com/articles/ecommerce-website-development/ecommerce-architecture/)*

**Critical optimizations**:
- Image optimization (WebP, lazy loading)
- CDN for static assets
- Minimize JavaScript
- Prefetch checkout pages
- Cache product data
- Optimize above-fold content

### Image Guidelines

- Product images: 1000x1000px minimum
- Multiple angles (4-8 per product)
- Zoom capability
- WebP format with JPEG fallback
- Lazy loading below fold

---

## Key User Journeys

### Journey 1: Browse to Purchase

```
Homepage → Collection → Product → Add to Cart → Checkout → Confirmation
```

### Journey 2: Search to Purchase

```
Search → Product → Add to Cart → Checkout → Confirmation
```

### Journey 3: Return Visitor

```
Homepage → Account → Past Order → Reorder → Checkout
```

### Journey 4: Sale Shopper

```
Sale Banner → Sale Collection → Filter by Size → Product → Purchase
```

---

## Implementation Checklist

### Foundation
- [ ] Core pages created
- [ ] Navigation structure
- [ ] Search functionality
- [ ] Mobile responsive

### Product
- [ ] Product pages with all elements
- [ ] Category pages with filters
- [ ] Product images optimized
- [ ] Variant selection working

### Cart & Checkout
- [ ] Cart page functional
- [ ] Checkout flow complete
- [ ] Payment integration
- [ ] Order confirmation emails

### Trust
- [ ] Reviews system
- [ ] Trust badges
- [ ] Clear policies
- [ ] Contact information

### SEO
- [ ] Schema markup
- [ ] Meta tags
- [ ] Sitemap
- [ ] Image alt text

### Performance
- [ ] Image optimization
- [ ] Page speed < 3s
- [ ] Mobile optimized
- [ ] CDN configured

---

## Sources

- [BigCommerce - Ecommerce Architecture](https://www.bigcommerce.com/articles/ecommerce-website-development/ecommerce-architecture/)
- [Webstacks - eCommerce Web Design Best Practices](https://www.webstacks.com/blog/ecommerce-web-design-best-practices)
- [Ecorn Agency - Ecommerce Website Design Best Practices](https://www.ecorn.agency/blog/ecommerce-website-design-best-practices)
- [Parachute Design - eCommerce Web Design Best Practices](https://parachutedesign.ca/blog/ecommerce-web-design-best-practices/)
- [Search Engine Land - Website Structure Guide](https://searchengineland.com/guide/website-structure)
