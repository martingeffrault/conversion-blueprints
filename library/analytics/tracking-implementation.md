# Tracking Implementation Guide

> **Purpose**: Technical implementation of analytics and tracking
> **Tool**: Google Tag Manager (GTM) — the industry standard
> **Principle**: Use GTM for flexibility; never hardcode tracking

---

## Google Tag Manager Overview

### Why Use GTM?

| Without GTM | With GTM |
|-------------|----------|
| Code changes for each tag | Add tags in UI |
| Developer dependency | Marketing can manage |
| Slow deployment | Instant publish |
| Risk of conflicts | Organized containers |
| Hard to test | Built-in preview mode |

### GTM Architecture

```
GTM Container
├── Tags (What to fire)
│   ├── GA4 Configuration
│   ├── GA4 Event
│   ├── Google Ads Conversion
│   └── Facebook Pixel
├── Triggers (When to fire)
│   ├── Page View
│   ├── Click
│   ├── Form Submit
│   └── Custom Event
└── Variables (What data to use)
    ├── Built-in
    ├── Data Layer
    └── Custom JavaScript
```

### GTM Installation

**Container snippet (in <head>)**:
```html
<!-- Google Tag Manager -->
<script>(function(w,d,s,l,i){w[l]=w[l]||[];w[l].push({'gtm.start':
new Date().getTime(),event:'gtm.js'});var f=d.getElementsByTagName(s)[0],
j=d.createElement(s),dl=l!='dataLayer'?'&l='+l:'';j.async=true;j.src=
'https://www.googletagmanager.com/gtm.js?id='+i+dl;f.parentNode.insertBefore(j,f);
})(window,document,'script','dataLayer','GTM-XXXXXXX');</script>
<!-- End Google Tag Manager -->
```

**Noscript fallback (after opening <body>)**:
```html
<!-- Google Tag Manager (noscript) -->
<noscript><iframe src="https://www.googletagmanager.com/ns.html?id=GTM-XXXXXXX"
height="0" width="0" style="display:none;visibility:hidden"></iframe></noscript>
<!-- End Google Tag Manager (noscript) -->
```

---

## The Data Layer

### What Is the Data Layer?

> "The data layer is a JavaScript object that passes information from your website to GTM."

```javascript
// Initialize before GTM loads
window.dataLayer = window.dataLayer || [];

// Push data
dataLayer.push({
  'event': 'custom_event',
  'category': 'engagement',
  'action': 'scroll',
  'label': '50%'
});
```

### Data Layer Best Practices

| Rule | Example |
|------|---------|
| Initialize before GTM | `window.dataLayer = window.dataLayer || [];` |
| Use camelCase | `productName`, not `product_name` |
| Push complete objects | Include all related data at once |
| Avoid arrays | Push each item separately |
| Don't modify history | Push new objects |

### Common Data Layer Variables

```javascript
// Page data
dataLayer.push({
  'pageType': 'product',
  'pageName': 'Blue T-Shirt',
  'pageCategory': 'Apparel'
});

// User data
dataLayer.push({
  'userLoggedIn': true,
  'userId': 'ABC123',
  'userType': 'premium'
});

// E-commerce data
dataLayer.push({
  'event': 'view_item',
  'ecommerce': {
    'items': [{
      'item_id': 'SKU123',
      'item_name': 'Blue T-Shirt',
      'price': 29.99
    }]
  }
});
```

---

## GTM Tags

### GA4 Configuration Tag

**Setup**:
1. Tags → New
2. Tag Type: Google Analytics: GA4 Configuration
3. Measurement ID: G-XXXXXXXXXX
4. Trigger: All Pages

**Settings**:
- Send page views: Yes (unless using custom event)
- Server container URL: (for server-side tagging)

### GA4 Event Tag

**Setup**:
1. Tags → New
2. Tag Type: Google Analytics: GA4 Event
3. Configuration Tag: Select your GA4 config
4. Event Name: Your event name
5. Event Parameters: Add as needed
6. Trigger: Your custom trigger

**Example - Form Submit**:
```
Event Name: generate_lead
Parameters:
  - form_name: {{Form ID}}
  - form_location: {{Page Path}}
Trigger: Form Submit - Contact Form
```

### Google Ads Conversion

**Setup**:
1. Tags → New
2. Tag Type: Google Ads Conversion Tracking
3. Conversion ID: From Google Ads
4. Conversion Label: From Google Ads
5. Conversion Value: {{Transaction Total}} (optional)
6. Trigger: Purchase Confirmation

### Facebook Pixel

**Setup**:
1. Tags → New
2. Tag Type: Custom HTML
3. Add Facebook Pixel code
4. Trigger: All Pages (base) + events

**Standard Events**:
```html
<script>
  fbq('track', 'PageView');
</script>
```

```html
<script>
  fbq('track', 'Purchase', {
    value: {{Transaction Total}},
    currency: 'USD'
  });
</script>
```

---

## GTM Triggers

### Built-in Triggers

| Trigger | Fires When |
|---------|------------|
| All Pages | Every page view |
| DOM Ready | DOM fully loaded |
| Window Loaded | All resources loaded |
| Click | Any click |
| Link Click | Click on `<a>` |
| Form Submit | Form submitted |
| Scroll Depth | Scroll threshold reached |
| Timer | After set duration |
| History Change | URL hash/pushState change |

### Custom Event Trigger

**Setup**:
1. Triggers → New
2. Trigger Type: Custom Event
3. Event Name: Your dataLayer event name

**Data Layer Push**:
```javascript
dataLayer.push({
  'event': 'newsletter_signup'
});
```

**GTM Trigger**:
- Event Name: `newsletter_signup`

### Click Triggers

**All Elements Click**:
- Fires on any click

**Just Links Click**:
- Fires only on `<a>` tags

**Click Variables**:
- `{{Click Element}}` - The clicked element
- `{{Click Classes}}` - CSS classes
- `{{Click ID}}` - Element ID
- `{{Click URL}}` - Link URL
- `{{Click Text}}` - Link text

**Example - CTA Button Click**:
```
Trigger: Click - All Elements
Condition: Click Classes contains "btn-primary"
```

### Form Submit Trigger

**Setup**:
1. Triggers → New
2. Trigger Type: Form Submission
3. Check validation (optional)
4. Condition: Form ID equals "contact-form"

**Variables**:
- `{{Form Element}}` - Form element
- `{{Form Classes}}` - Form classes
- `{{Form ID}}` - Form ID
- `{{Form URL}}` - Form action URL

### Scroll Depth Trigger

**Setup**:
1. Triggers → New
2. Trigger Type: Scroll Depth
3. Vertical/Horizontal
4. Percentages: 25, 50, 75, 90
5. Fire on: Specific pages (optional)

---

## GTM Variables

### Built-in Variables

Enable in Variables → Built-in:

| Category | Variables |
|----------|-----------|
| Pages | Page URL, Page Path, Page Hostname |
| Utilities | Container ID, Debug Mode, Random Number |
| Errors | Error Message, Error URL, Error Line |
| Clicks | Click Element, Classes, ID, URL, Text |
| Forms | Form Element, Classes, ID, URL, Text |
| History | New URL, Old URL, History Source |
| Videos | Video Provider, Status, Title, Duration |
| Scrolling | Scroll Depth Threshold, Units |

### Data Layer Variables

**Setup**:
1. Variables → User-Defined → New
2. Variable Type: Data Layer Variable
3. Data Layer Variable Name: `ecommerce.items.0.item_name`

**Nested Access**:
```
ecommerce.items.0.price → First item's price
userProfile.name → User's name
```

### Custom JavaScript Variables

**Setup**:
1. Variables → User-Defined → New
2. Variable Type: Custom JavaScript
3. Write JavaScript function

**Example - Get Cookie Value**:
```javascript
function() {
  var name = 'user_id=';
  var cookies = document.cookie.split(';');
  for (var i = 0; i < cookies.length; i++) {
    var c = cookies[i].trim();
    if (c.indexOf(name) === 0) {
      return c.substring(name.length);
    }
  }
  return null;
}
```

### Lookup Table Variables

Transform values based on input:

| Input | Output |
|-------|--------|
| `/` | Homepage |
| `/products` | Products |
| `/blog` | Blog |
| (default) | Other |

### Regex Table Variables

Pattern matching for variable values:

| Pattern | Output |
|---------|--------|
| `^/products/.*` | Product Page |
| `^/blog/.*` | Blog Post |
| `.*` | Other |

---

## E-commerce Tracking

### Data Layer for E-commerce

**Product View**:
```javascript
dataLayer.push({
  'event': 'view_item',
  'ecommerce': {
    'items': [{
      'item_id': 'SKU123',
      'item_name': 'Blue T-Shirt',
      'item_brand': 'Brand',
      'item_category': 'Apparel',
      'item_variant': 'Blue / L',
      'price': 29.99,
      'currency': 'USD',
      'quantity': 1
    }]
  }
});
```

**Add to Cart**:
```javascript
dataLayer.push({
  'event': 'add_to_cart',
  'ecommerce': {
    'items': [{
      'item_id': 'SKU123',
      'item_name': 'Blue T-Shirt',
      'price': 29.99,
      'currency': 'USD',
      'quantity': 1
    }]
  }
});
```

**Purchase**:
```javascript
dataLayer.push({
  'event': 'purchase',
  'ecommerce': {
    'transaction_id': 'T12345',
    'value': 59.98,
    'tax': 4.90,
    'shipping': 5.99,
    'currency': 'USD',
    'items': [{
      'item_id': 'SKU123',
      'item_name': 'Blue T-Shirt',
      'price': 29.99,
      'quantity': 2
    }]
  }
});
```

### GTM E-commerce Setup

1. **Data Layer Variable**: `ecommerce.items`
2. **GA4 Event Tag**: Event name from dataLayer
3. **Trigger**: Custom Event for each e-commerce event

---

## Debugging

### GTM Preview Mode

1. Click "Preview" in GTM
2. Enter your website URL
3. Debug panel opens alongside site
4. See tags fired, triggers matched, data layer

**What to Check**:
- Tags Fired vs Not Fired
- Trigger conditions met
- Data Layer values
- Variable values

### Browser DevTools

**Console**:
```javascript
// View data layer
console.log(dataLayer);

// Watch for data layer pushes
dataLayer.push = function(obj) {
  console.log('Data Layer Push:', obj);
  Array.prototype.push.call(this, obj);
};
```

**Network Tab**:
- Filter by `google`, `analytics`, `collect`
- Check payload parameters

### GA4 DebugView

1. GA4 Admin → DebugView
2. Install GA Debugger extension
3. See real-time events from your session

### Tag Assistant (Legacy)

Google Tag Assistant extension for Chrome:
- Shows all Google tags
- Validates implementation
- Suggests fixes

---

## Server-Side Tracking

### Why Server-Side?

| Client-Side | Server-Side |
|-------------|-------------|
| Browser sends data | Server sends data |
| Ad blockers block | Ad blockers don't affect |
| Slower (more requests) | Faster (consolidated) |
| Less control | Full control |
| Cookie limitations | First-party cookies |

### Server-Side GTM Setup

1. Create Server Container in GTM
2. Set up App Engine or Cloud Run
3. Point subdomain to server
4. Update container to server URL

### Implementation Flow

```
Browser → First-Party Server (your domain)
              ↓
          Server GTM Container
              ↓
    GA4 / Google Ads / Facebook
```

---

## Common Implementations

### Newsletter Signup

**Data Layer**:
```javascript
document.querySelector('#newsletter-form').addEventListener('submit', function() {
  dataLayer.push({
    'event': 'newsletter_signup',
    'formLocation': 'footer'
  });
});
```

**GTM Setup**:
- Trigger: Custom Event `newsletter_signup`
- Tag: GA4 Event `generate_lead`

### CTA Click Tracking

**GTM Setup**:
- Trigger: Click - All Elements where Click Classes contains "cta"
- Tag: GA4 Event `cta_click` with parameters:
  - cta_text: {{Click Text}}
  - cta_location: {{Page Path}}

### Scroll Tracking

**GTM Setup**:
- Trigger: Scroll Depth 25%, 50%, 75%, 90%
- Tag: GA4 Event `scroll` with parameter:
  - scroll_depth: {{Scroll Depth Threshold}}

### Video Tracking

**GTM Setup** (YouTube):
1. Enable built-in Video variables
2. Trigger: YouTube Video - Start, Progress, Complete
3. Tag: GA4 Event `video_{{Video Status}}` with parameters:
   - video_title: {{Video Title}}
   - video_percent: {{Video Percent}}

### File Downloads

**GTM Setup**:
- Trigger: Click - Just Links where Click URL contains `.pdf`
- Tag: GA4 Event `file_download` with parameters:
  - file_name: {{Click URL}}

### Outbound Links

**GTM Setup**:
- Trigger: Click - Just Links where Click URL does not contain your domain
- Tag: GA4 Event `outbound_click` with parameters:
  - link_url: {{Click URL}}
  - link_text: {{Click Text}}

---

## Testing Checklist

### Before Publishing

- [ ] Preview mode shows correct tags firing
- [ ] Data layer values are correct
- [ ] No JavaScript errors in console
- [ ] Tags fire on correct triggers only
- [ ] No duplicate tags firing
- [ ] E-commerce data is accurate

### After Publishing

- [ ] Real-time GA4 shows events
- [ ] Conversions tracking correctly
- [ ] E-commerce revenue accurate
- [ ] Third-party pixels receiving data
- [ ] No site performance issues

---

## Naming Conventions

### Tags

Format: `[Platform] - [Type] - [Description]`

Examples:
- `GA4 - Config - All Pages`
- `GA4 - Event - Form Submit`
- `Google Ads - Conversion - Purchase`
- `Facebook - Event - Add to Cart`

### Triggers

Format: `[Type] - [Description]`

Examples:
- `Page View - All Pages`
- `Click - CTA Buttons`
- `Form - Contact Submit`
- `Custom Event - Newsletter Signup`

### Variables

Format: `[Type] - [Description]`

Examples:
- `DLV - Transaction ID`
- `JS - Cookie User ID`
- `Lookup - Page Type`
- `Const - GA4 Measurement ID`

---

## Sources

- [Google Tag Manager Docs](https://developers.google.com/tag-platform/tag-manager)
- [Simo Ahava - GTM Tutorials](https://www.simoahava.com/)
- [Analytics Mania](https://www.analyticsmania.com/)
- [MeasureSchool](https://measureschool.com/)
- [Google Tag Manager Community](https://support.google.com/tagmanager/community)
