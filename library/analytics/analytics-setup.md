# Analytics Setup Guide

> **Purpose**: Implement measurement that drives business decisions
> **Platform**: Google Analytics 4 (GA4) — the industry standard
> **Principle**: Plan what to measure before implementing tracking

---

## Analytics Strategy

### Before Implementation

> "Most companies are data rich but information poor."
>
> *— Avinash Kaushik*

Answer these questions first:
1. What business outcomes matter?
2. What user actions indicate success?
3. What decisions will data inform?
4. Who needs access to reports?

### The Measurement Plan

| Component | Question | Example |
|-----------|----------|---------|
| **Objective** | What business goal? | Increase online sales |
| **Strategy** | How to achieve it? | Optimize checkout flow |
| **KPI** | How to measure success? | Conversion rate, revenue |
| **Target** | What's the goal? | 3% conversion rate |
| **Segment** | Who to analyze? | Mobile vs desktop |

---

## Google Analytics 4 Setup

### Account Structure

```
Account (Business)
└── Property (Website/App)
    └── Data Stream (Web, iOS, Android)
```

**Best Practices**:
- One account per business/client
- One property per product/website
- Separate properties for staging/production

### GA4 vs Universal Analytics

| Feature | Universal Analytics | GA4 |
|---------|---------------------|-----|
| Data model | Session-based | Event-based |
| Tracking | Page views, events | Everything is an event |
| Cross-platform | Limited | Web + app unified |
| ML insights | Basic | Built-in |
| Privacy | Cookie-dependent | Privacy-centric |

### Installation Methods

| Method | Best For | Difficulty |
|--------|----------|------------|
| **gtag.js** | Simple sites | Easy |
| **Google Tag Manager** | Complex sites | Medium |
| **CMS plugins** | WordPress, Shopify | Easy |

**gtag.js Installation**:
```html
<!-- Place in <head> -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-XXXXXXXXXX"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());
  gtag('config', 'G-XXXXXXXXXX');
</script>
```

---

## Event Tracking

### GA4 Event Types

| Type | Description | Example |
|------|-------------|---------|
| **Automatically collected** | Built-in | page_view, first_visit, session_start |
| **Enhanced measurement** | Toggle on | scroll, outbound_click, file_download |
| **Recommended events** | Standard names | purchase, sign_up, add_to_cart |
| **Custom events** | You define | contact_form_submit, pricing_view |

### Enhanced Measurement Events

Enable in GA4 Admin → Data Streams → Enhanced Measurement:

| Event | What It Tracks |
|-------|----------------|
| Page views | URL changes, virtual pages |
| Scrolls | 90% page depth |
| Outbound clicks | Clicks leaving your domain |
| Site search | Search queries |
| Video engagement | YouTube embeds |
| File downloads | PDF, doc, etc. |
| Form interactions | Start, submit (Beta) |

### Recommended Events

Use Google's recommended event names for automatic reports:

| Event | Parameters | Use Case |
|-------|------------|----------|
| `sign_up` | method | User registration |
| `login` | method | User login |
| `purchase` | transaction_id, value, currency, items | E-commerce |
| `add_to_cart` | currency, value, items | E-commerce |
| `generate_lead` | currency, value | Lead generation |
| `view_item` | currency, value, items | Product views |
| `begin_checkout` | currency, value, items | Checkout start |

### Custom Event Naming

**Convention**: `object_action` or `action_object`

| Good | Bad |
|------|-----|
| `form_submit` | `FormSubmit` |
| `video_play` | `video played` |
| `pricing_view` | `Pricing_View` |
| `cta_click` | `CTA Click!` |

**Rules**:
- Lowercase
- Underscores for spaces
- No special characters
- Max 40 characters
- Descriptive but concise

---

## Conversion Tracking

### Setting Up Conversions

**In GA4**:
1. Admin → Events
2. Find your event
3. Toggle "Mark as conversion"

Or:
1. Admin → Conversions
2. "New conversion event"
3. Enter event name

### Key Conversions by Business Type

| Business | Primary Conversions | Secondary Conversions |
|----------|---------------------|----------------------|
| **E-commerce** | purchase | add_to_cart, begin_checkout |
| **SaaS** | sign_up, subscription | demo_request, pricing_view |
| **Lead Gen** | generate_lead | form_start, phone_click |
| **Content** | sign_up (newsletter) | scroll_90, return_visit |

### Conversion Value

Assign monetary values to conversions:

```javascript
gtag('event', 'generate_lead', {
  'currency': 'USD',
  'value': 50.00  // Average lead value
});
```

---

## E-commerce Tracking

### GA4 E-commerce Events

| Funnel Stage | Event | Required Parameters |
|--------------|-------|---------------------|
| Browse | `view_item_list` | item_list_id, items |
| View | `view_item` | currency, value, items |
| Add to cart | `add_to_cart` | currency, value, items |
| View cart | `view_cart` | currency, value, items |
| Checkout | `begin_checkout` | currency, value, items |
| Shipping | `add_shipping_info` | currency, value, items, shipping_tier |
| Payment | `add_payment_info` | currency, value, items, payment_type |
| Purchase | `purchase` | transaction_id, currency, value, items |

### Item Parameters

```javascript
items: [{
  item_id: 'SKU_12345',
  item_name: 'Product Name',
  item_brand: 'Brand',
  item_category: 'Category',
  item_category2: 'Subcategory',
  item_variant: 'Color/Size',
  price: 29.99,
  quantity: 1
}]
```

### Purchase Event Example

```javascript
gtag('event', 'purchase', {
  transaction_id: 'T12345',
  value: 59.98,
  tax: 4.80,
  shipping: 5.99,
  currency: 'USD',
  coupon: 'SUMMER20',
  items: [{
    item_id: 'SKU_12345',
    item_name: 'T-Shirt',
    price: 29.99,
    quantity: 2
  }]
});
```

---

## User Properties

### Built-in User Properties

GA4 automatically collects:
- Device category
- Operating system
- Browser
- Language
- Country

### Custom User Properties

Set user-level attributes:

```javascript
gtag('set', 'user_properties', {
  user_type: 'premium',
  account_tier: 'enterprise',
  signup_date: '2024-01-15'
});
```

**Best Practices**:
- Max 25 custom user properties
- No PII (names, emails, etc.)
- Use for segmentation

---

## Attribution Models

### GA4 Attribution

| Model | Description | Best For |
|-------|-------------|----------|
| **Data-driven** | ML-based credit allocation | Default, most accurate |
| **Last click** | 100% to final touchpoint | Simple, conservative |
| **First click** | 100% to first touchpoint | Brand awareness |
| **Linear** | Equal credit to all | Long sales cycles |
| **Position-based** | 40% first, 40% last, 20% middle | Balanced view |
| **Time decay** | More credit to recent | Short cycles |

### Setting Attribution Model

Admin → Attribution Settings → Reporting Attribution Model

### Lookback Window

How far back to credit conversions:

| Conversion Type | Default | Range |
|-----------------|---------|-------|
| Acquisition | 30 days | 1-90 days |
| All other | 90 days | 1-90 days |

---

## Audiences & Segments

### Creating Audiences

Admin → Audiences → New Audience

**Useful Audiences**:
- Users who viewed pricing but didn't convert
- Users who abandoned cart
- High-value customers (top 10% by revenue)
- Engaged users (3+ sessions in 7 days)
- Users from specific campaigns

### Audience Triggers

Automatically fire events when users join an audience:

```
Audience: High-value customers
Trigger event: high_value_customer
```

---

## Goals & Targets

### Setting Up Goals

**In GA4**: Conversions replace goals, but you can set benchmarks:

| Metric | Formula | Benchmark |
|--------|---------|-----------|
| Conversion Rate | Conversions / Users × 100 | 2-5% |
| Bounce Rate | Single-page sessions / Sessions × 100 | < 50% |
| Pages/Session | Pageviews / Sessions | > 2 |
| Avg. Session Duration | Total duration / Sessions | > 2 min |

### Funnel Analysis

Explorations → Funnel Exploration:

1. Define steps (events)
2. Set order (open or closed)
3. Analyze drop-off points
4. Segment by dimensions

---

## Privacy & Consent

### Consent Mode

Adjust tracking based on user consent:

```javascript
gtag('consent', 'default', {
  'ad_storage': 'denied',
  'analytics_storage': 'denied'
});

// On user consent
gtag('consent', 'update', {
  'analytics_storage': 'granted'
});
```

### Data Retention

Admin → Data Settings → Data Retention:
- 2 months (default)
- 14 months (maximum)

### IP Anonymization

GA4 anonymizes IP addresses by default.

### Data Deletion

Admin → Data Settings → Data Deletion Requests

---

## Reporting Essentials

### Standard Reports

| Report | Purpose |
|--------|---------|
| **Realtime** | Live activity |
| **Acquisition** | Where users come from |
| **Engagement** | What users do |
| **Monetization** | Revenue and transactions |
| **Retention** | User return behavior |

### Custom Reports (Explorations)

| Type | Best For |
|------|----------|
| **Free-form** | Custom tables |
| **Funnel** | Conversion flows |
| **Path** | User journeys |
| **Segment overlap** | Audience comparison |
| **Cohort** | Time-based analysis |

### Key Dimensions

| Dimension | Usage |
|-----------|-------|
| Source / Medium | Traffic origin |
| Campaign | Marketing campaigns |
| Device category | Desktop vs mobile |
| Landing page | Entry points |
| Page path | Content performance |
| Event name | User actions |

---

## Implementation Checklist

### Basic Setup
- [ ] GA4 property created
- [ ] Data stream configured
- [ ] Tracking code installed
- [ ] Real-time data verified
- [ ] Enhanced measurement enabled

### Conversions
- [ ] Key conversions defined
- [ ] Events marked as conversions
- [ ] Conversion values assigned
- [ ] Funnel steps tracked

### E-commerce (if applicable)
- [ ] E-commerce events implemented
- [ ] Product data structured
- [ ] Purchase tracking verified
- [ ] Revenue reporting accurate

### Privacy
- [ ] Consent mode configured
- [ ] Data retention set
- [ ] Cookie policy updated
- [ ] Privacy policy updated

### Reporting
- [ ] Key audiences created
- [ ] Custom reports built
- [ ] Dashboards configured
- [ ] Team access granted

---

## Common Mistakes

| Mistake | Impact | Fix |
|---------|--------|-----|
| No tracking plan | Messy data | Document before implementing |
| Too many events | Quota limits, noise | Focus on key actions |
| Inconsistent naming | Hard to analyze | Use naming convention |
| No conversions set | Can't measure success | Define 3-5 conversions |
| Ignoring filters | Internal traffic | Exclude office IPs |
| Not testing | Broken tracking | Test in staging first |

---

## Sources

- [Google Analytics Academy](https://analytics.google.com/analytics/academy/)
- [GA4 Documentation](https://developers.google.com/analytics/devguides/collection/ga4)
- [Simo Ahava's Blog](https://www.simoahava.com/)
- [Avinash Kaushik's Blog](https://www.kaushik.net/avinash/)
- [Google Tag Manager Docs](https://developers.google.com/tag-platform/tag-manager)
- [CXL Analytics Guides](https://cxl.com/institute/)
