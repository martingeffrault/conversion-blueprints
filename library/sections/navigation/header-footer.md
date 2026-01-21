# Navigation: Header & Footer Best Practices

> **Purpose**: Guide users through the site, provide quick access to key pages, build trust
> **Position**: Header (top of every page), Footer (bottom of every page)
> **Goal**: Easy navigation, clear information architecture, conversion support

---

## Header Navigation

### Core Principles

1. **Simplicity**: Limit top-level items to 5-7
2. **Hierarchy**: Most important pages are most visible
3. **Consistency**: Same navigation on every page
4. **Accessibility**: Keyboard navigable, screen reader friendly

### Header Elements

```
┌─────────────────────────────────────────────────────────────────┐
│ [Logo]  [Primary Nav]  [Utility Nav]  [CTA Button]              │
└─────────────────────────────────────────────────────────────────┘
```

| Element | Purpose | Examples |
|---------|---------|----------|
| **Logo** | Brand identity, home link | Company logo |
| **Primary Nav** | Main site sections | Products, Services, About |
| **Utility Nav** | Support actions | Search, Login, Cart |
| **CTA** | Primary conversion | "Get Started", "Contact" |

---

## Header Patterns

### Pattern 1: Standard (Most Common)

```
┌─────────────────────────────────────────────────────────────────┐
│ [Logo]     Nav 1    Nav 2    Nav 3    Nav 4     [🔍] [CTA]      │
└─────────────────────────────────────────────────────────────────┘
```

**Best for**: SaaS, corporate, most websites

### Pattern 2: Centered Logo

```
┌─────────────────────────────────────────────────────────────────┐
│ Nav 1    Nav 2    [Logo]    Nav 3    Nav 4     [🔍] [Cart]      │
└─────────────────────────────────────────────────────────────────┘
```

**Best for**: Luxury brands, fashion, lifestyle

### Pattern 3: Minimal

```
┌─────────────────────────────────────────────────────────────────┐
│ [Logo]                                          [Menu ☰]        │
└─────────────────────────────────────────────────────────────────┘
```

**Best for**: Portfolio, creative, single-page

### Pattern 4: E-commerce

```
┌─────────────────────────────────────────────────────────────────┐
│ [Logo]  [🔍 Search..............................]  [👤] [🛒 3]  │
├─────────────────────────────────────────────────────────────────┤
│ Shop ▼    New    Sale    Collections    About                   │
└─────────────────────────────────────────────────────────────────┘
```

**Best for**: Online stores with many categories

### Pattern 5: Local Business

```
┌─────────────────────────────────────────────────────────────────┐
│ [Logo]  Services  About  Contact        📞 (555) 123-4567       │
└─────────────────────────────────────────────────────────────────┘
```

**Best for**: Service businesses, local companies

---

## Mega Menu

For sites with many pages or categories.

### Structure

```
┌─────────────────────────────────────────────────────────────────┐
│ [Logo]     Products ▼     Solutions     Pricing     [CTA]       │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  PRODUCTS              BY TEAM              RESOURCES           │
│  ─────────             ───────              ─────────           │
│  Product A             Sales                Documentation       │
│  Product B             Marketing            API Reference       │
│  Product C             Engineering          Blog                │
│  Product D             Support              Help Center         │
│                                                                 │
│  [Featured Product Image]                   [What's New →]      │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Mega Menu Best Practices

- **Group logically** (by category, audience, or use case)
- **Limit depth** (2 levels max in mega menu)
- **Include featured content** (highlight key pages)
- **Visual elements** (icons, images help scanning)
- **Clear exit** (click outside to close)

---

## Sticky/Fixed Header

### When to Use

- Long pages
- Important CTA always visible
- E-commerce (cart access)

### Behavior Options

| Behavior | Description | Best For |
|----------|-------------|----------|
| **Always visible** | Header stays fixed | Short pages |
| **Hide on scroll down** | Disappears when scrolling down, returns on scroll up | Long content |
| **Compact on scroll** | Shrinks height after scrolling | Most sites |

### Sticky Header Example

```
Before scroll:
┌─────────────────────────────────────────────────────────────────┐
│ [Logo]     Nav 1    Nav 2    Nav 3    Nav 4           [CTA]     │
│                                                                 │
│ Tagline or secondary info                                       │
└─────────────────────────────────────────────────────────────────┘

After scroll (compact):
┌─────────────────────────────────────────────────────────────────┐
│ [Logo]     Nav 1    Nav 2    Nav 3    Nav 4           [CTA]     │
└─────────────────────────────────────────────────────────────────┘
```

---

## Mobile Navigation

### Mobile Header

```
┌─────────────────────────┐
│ [☰]    [Logo]    [CTA]  │
└─────────────────────────┘
  ↑                   ↑
Hamburger         Action button
```

### Mobile Menu Patterns

**Pattern 1: Slide-out (Drawer)**
```
┌────────────────────┬────┐
│                    │    │
│  [✕]               │    │
│                    │    │
│  Home              │ O  │
│  Products ▼        │ v  │
│    - Product A     │ e  │
│    - Product B     │ r  │
│  About             │ l  │
│  Contact           │ a  │
│                    │ y  │
│  [CTA Button]      │    │
│                    │    │
└────────────────────┴────┘
```

**Pattern 2: Full Screen**
```
┌─────────────────────────┐
│                   [✕]   │
│                         │
│         Home            │
│       Products          │
│        About            │
│       Contact           │
│                         │
│    [CTA Button]         │
│                         │
└─────────────────────────┘
```

**Pattern 3: Bottom Sheet**
```
┌─────────────────────────┐
│                         │
│    (Page content)       │
│                         │
├─────────────────────────┤
│  ────  (drag handle)    │
│                         │
│  Home                   │
│  Products               │
│  About                  │
│  Contact                │
│                         │
└─────────────────────────┘
```

### Mobile Navigation Best Practices

- **Touch targets**: 44px minimum
- **Clear close button**: Easy to dismiss
- **Current page indicator**: Show where user is
- **Expandable sections**: For sub-navigation
- **CTA visible**: Don't bury the primary action
- **Phone number**: Click-to-call (local business)

---

## Footer Navigation

### Footer Purpose

1. **Secondary navigation**: Pages not in header
2. **Legal compliance**: Privacy, terms
3. **Trust signals**: Certifications, security
4. **Contact info**: Multiple contact methods
5. **Social proof**: Social links, newsletter

### Footer Patterns

**Pattern 1: Multi-Column (Standard)**

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  PRODUCT         COMPANY        RESOURCES       LEGAL           │
│  ───────         ───────        ─────────       ─────           │
│  Features        About          Blog            Privacy         │
│  Pricing         Careers        Help Center     Terms           │
│  Integrations    Press          Documentation   Cookies         │
│  What's New      Contact        API             Security        │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  [Logo]          Newsletter: [email________] [Subscribe]        │
│  Tagline         [Twitter] [LinkedIn] [GitHub]                  │
│                                                                 │
│  © 2024 Company Name. All rights reserved.                      │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Pattern 2: Minimal**

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Logo]                                                         │
│                                                                 │
│  Home    About    Services    Contact    Privacy    Terms       │
│                                                                 │
│  © 2024 Company Name                                            │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Pattern 3: Contact-Focused (Local Business)**

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐ │
│  │ 📞 Call Us      │  │ 📍 Visit Us     │  │ ⏰ Hours        │ │
│  │ (555) 123-4567  │  │ 123 Main Street │  │ Mon-Fri 8-6     │ │
│  │                 │  │ City, ST 12345  │  │ Sat 9-4         │ │
│  └─────────────────┘  └─────────────────┘  └─────────────────┘ │
│                                                                 │
│  Services: Service 1 | Service 2 | Service 3 | All Services    │
│                                                                 │
│  © 2024 Business | License #123456 | Privacy | Terms            │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Pattern 4: E-commerce**

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  SHOP            HELP             COMPANY         CONNECT       │
│  ────            ────             ───────         ───────       │
│  All Products    FAQ              About           Instagram     │
│  New Arrivals    Shipping         Sustainability  TikTok        │
│  Sale            Returns          Press           Pinterest     │
│  Gift Cards      Size Guide       Careers         Newsletter    │
│                  Contact                                        │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  [Visa] [MC] [Amex] [PayPal] [Apple Pay]      [🔒 Secure]       │
│                                                                 │
│  © 2024 Store | Privacy | Terms | Accessibility                 │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Footer Content Priorities

### By Business Type

| Business Type | Priority Content |
|---------------|------------------|
| **SaaS** | Product links, Resources, Company, Social |
| **E-commerce** | Shop links, Help (shipping, returns), Payment badges |
| **Local Business** | Contact info, Hours, Location, Services |
| **Agency** | Work, Services, About, Social |
| **Blog/Media** | Categories, Newsletter, Social, About |

### Essential Footer Elements

| Element | Required | Notes |
|---------|----------|-------|
| **Copyright** | Yes | © Year Company |
| **Privacy Policy** | Yes | Legal requirement |
| **Terms** | Yes | Legal requirement |
| **Contact** | Recommended | Email or form link |
| **Logo** | Recommended | Brand presence |

---

## Navigation UX Best Practices

### Information Architecture

- **Primary nav**: 5-7 items max
- **Logical grouping**: Related pages together
- **User-centric labels**: Match user mental model
- **Clear hierarchy**: Most important = most visible

### Visual Design

- **Consistent placement**: Same position on all pages
- **Clear active state**: Show current page
- **Hover states**: Indicate interactivity
- **Adequate spacing**: Touch-friendly on mobile

### Accessibility

- **Keyboard navigation**: Tab through all items
- **Focus indicators**: Visible focus state
- **ARIA labels**: For screen readers
- **Skip to content**: Link for keyboard users
- **Descriptive labels**: "Contact us" not "Click here"

---

## Common Mistakes

### Header Mistakes

- ❌ **Too many items**: Creates decision paralysis
- ❌ **Unclear labels**: Generic or jargon
- ❌ **Hidden navigation**: Hamburger menu on desktop
- ❌ **No mobile optimization**: Tiny touch targets
- ❌ **Missing CTA**: No clear primary action

### Footer Mistakes

- ❌ **Link dump**: Unorganized list of every page
- ❌ **Missing legal**: No privacy or terms
- ❌ **Outdated info**: Wrong year, old address
- ❌ **Dead links**: Links to removed pages
- ❌ **Too minimal**: Missing helpful links

---

## Templates

### SaaS Header

```
[Logo]  Product ▼  Solutions  Pricing  Resources ▼  [Login] [Free Trial]
```

### E-commerce Header

```
[Logo]  [🔍 Search bar]  [Account] [Wishlist] [Cart (3)]
[All Categories ▼]  New  Sale  Brands  [Special Offer Banner]
```

### Agency Header

```
[Logo]     Work    Services    About    Blog    [Contact]
```

### Local Business Header

```
[Logo]  Services ▼  About  Reviews  Contact    📞 (555) 123-4567
```

---

## Sources

- UX research on navigation patterns
- Nielsen Norman Group studies
- E-commerce navigation best practices
- WCAG accessibility guidelines
