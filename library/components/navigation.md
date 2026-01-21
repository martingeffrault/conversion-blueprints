# Navigation Patterns & Best Practices

> **Purpose**: Create intuitive, accessible navigation that guides users
> **Impact**: Navigation affects every page and user journey
> **Principle**: Users should always know where they are and where they can go

---

## Header Navigation

### Standard Header Pattern

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Logo]     Products ▼    Solutions    Pricing    Resources ▼  │
│                                                                 │
│                                          [Login]  [Get Started] │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Header Components

| Element | Purpose | Notes |
|---------|---------|-------|
| Logo | Brand identity, home link | Always link to homepage |
| Primary nav | Main sections | 4-7 items maximum |
| Utility nav | Secondary actions | Login, account, search |
| CTA | Primary action | Stand out from nav items |

### Header Variations

**Minimal (creative agencies, portfolios)**:
```
┌─────────────────────────────────────────────────────────────────┐
│  [Logo]                               Work   About   Contact    │
└─────────────────────────────────────────────────────────────────┘
```

**Centered logo (luxury, lifestyle)**:
```
┌─────────────────────────────────────────────────────────────────┐
│  Shop    About              [Logo]              Blog    Contact │
└─────────────────────────────────────────────────────────────────┘
```

**Full-width with search (e-commerce, content)**:
```
┌─────────────────────────────────────────────────────────────────┐
│  [Logo]  [──────── Search ────────]   Account  Cart($99)  ☰    │
├─────────────────────────────────────────────────────────────────┤
│  All Categories    New Arrivals    Sale    Brands    Help      │
└─────────────────────────────────────────────────────────────────┘
```

---

## Mega Menus

### When to Use

| Use Case | Mega Menu? |
|----------|-----------|
| 10+ subcategories | ✓ Yes |
| Complex product structure | ✓ Yes |
| Need to show promotions | ✓ Yes |
| Simple 5-page site | ✗ No (overkill) |
| Mobile-first audience | ✗ Consider alternatives |

### Mega Menu Structure

```
┌─────────────────────────────────────────────────────────────────┐
│  Products ▼                                                     │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  BY CATEGORY          BY USE CASE         RESOURCES             │
│  ───────────          ───────────         ─────────             │
│  • Analytics          • For Marketing     • Documentation       │
│  • Automation         • For Sales         • API Reference       │
│  • Integration        • For Support       • Guides              │
│  • Reporting          • For Engineering   • Webinars            │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  [Featured Image]                                       │   │
│  │  New: AI-Powered Analytics                              │   │
│  │  Learn how AI can transform your data →                 │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Mega Menu Best Practices

| Do | Don't |
|----|-------|
| Group items logically | Dump all links randomly |
| Use clear column headers | Leave columns unlabeled |
| Include featured content | Make it just a link dump |
| Keep 3-4 columns max | Overwhelm with 6+ columns |
| Ensure keyboard accessible | Rely only on hover |

---

## Mobile Navigation

### Hamburger Menu

```
┌────────────────────────────────────────┐
│  [Logo]                          [☰]  │
└────────────────────────────────────────┘

When opened:
┌────────────────────────────────────────┐
│  [Logo]                          [✕]  │
├────────────────────────────────────────┤
│                                        │
│  Products                          ▼   │
│  Solutions                         ▼   │
│  Pricing                               │
│  Resources                         ▼   │
│                                        │
│  ─────────────────────────────────     │
│                                        │
│  Login                                 │
│  [     Get Started     ]               │
│                                        │
└────────────────────────────────────────┘
```

### Mobile Menu Patterns

| Pattern | Best For | Notes |
|---------|----------|-------|
| **Hamburger (slide)** | Most sites | Standard, recognized |
| **Bottom tab bar** | Apps, high-frequency actions | Thumb-friendly |
| **Hamburger (full screen)** | Creative sites | More immersive |
| **Priority+ nav** | Content sites | Shows key items, hides rest |

### Bottom Tab Bar (App-Style)

```
┌────────────────────────────────────────┐
│                                        │
│           [Page Content]               │
│                                        │
├────────────────────────────────────────┤
│  🏠        🔍        ❤️        👤       │
│  Home    Search   Saved    Account     │
└────────────────────────────────────────┘
```

**Best for**: E-commerce, apps, high-engagement sites
**Limit**: 4-5 items maximum

---

## Sticky/Fixed Navigation

### Scroll Behavior Patterns

**Always sticky**:
```
Header stays fixed at top during all scrolling
Best for: Short pages, frequent navigation needed
```

**Sticky after scroll**:
```
Normal → scroll 100px → becomes sticky
Best for: Long pages, preserve initial visual impact
```

**Hide on scroll down, show on scroll up**:
```
User scrolls down → header hides (more content space)
User scrolls up → header reappears (ready to navigate)
Best for: Mobile, content-heavy pages
```

### Sticky Header Transformation

```
Full header (top of page):
┌─────────────────────────────────────────────────────────────────┐
│  [Logo]     Products   Solutions   Pricing   [Login] [Sign Up] │
│                                                                 │
│  Tagline or secondary navigation                               │
└─────────────────────────────────────────────────────────────────┘

Compact header (after scroll):
┌─────────────────────────────────────────────────────────────────┐
│  [Logo]  Products  Solutions  Pricing  [Login] [Sign Up]       │
└─────────────────────────────────────────────────────────────────┘
```

---

## Breadcrumbs

### When to Use

| Use Case | Need Breadcrumbs? |
|----------|------------------|
| E-commerce (categories) | ✓ Essential |
| Blog with categories | ✓ Helpful |
| Documentation | ✓ Essential |
| Simple brochure site | ✗ Usually not needed |
| Single-page app | ✗ Not applicable |

### Breadcrumb Structure

```
Home > Products > Category > Subcategory > Product Name
  ↑       ↑          ↑           ↑             ↑
Link    Link       Link        Link      Current (not linked)
```

### Breadcrumb Variations

**Standard (chevron separator)**:
```
Home › Products › Cameras › DSLR
```

**Slash separator**:
```
Home / Products / Cameras / DSLR
```

**With icons**:
```
🏠 Home › 📦 Products › 📷 Cameras › DSLR
```

### Breadcrumb Best Practices

| Do | Don't |
|----|-------|
| Start with "Home" | Start with current page |
| Keep labels short | Use full page titles |
| Make all but last clickable | Make current page clickable |
| Use schema markup | Forget SEO benefits |
| Show full path | Skip hierarchy levels |

---

## Pagination

### When to Use

| Pattern | Best For |
|---------|----------|
| **Pagination** | Structured browsing (search results, products) |
| **Infinite scroll** | Casual browsing (social feeds, news) |
| **Load more button** | Balance of both |

### Pagination Pattern

```
← Previous    1  2  [3]  4  5  ...  20    Next →
                    ↑
              Current page
```

### Pagination Variations

**Basic**:
```
← Previous    1  2  3  4  5    Next →
```

**With ellipsis (many pages)**:
```
← Previous    1  2  3  ...  18  19  20    Next →
```

**With page count**:
```
← Previous    1  2  [3]  4  5    Next →
                Page 3 of 20
```

**Mobile-friendly**:
```
┌──────────────────────────────────────┐
│   ←     Page 3 of 20      →         │
└──────────────────────────────────────┘
```

### Pagination Best Practices

| Do | Don't |
|----|-------|
| Show current page clearly | Leave user guessing |
| Provide previous/next | Only show numbers |
| Show total pages/items | Leave count unknown |
| Keep touch targets large (mobile) | Make tiny click areas |

---

## In-Page Navigation

### Table of Contents (Long Content)

```
┌───────────────────┐
│  On this page     │
│                   │
│  1. Introduction  │
│  2. Features      │ ← Scrolls to section
│  3. Pricing       │
│  4. FAQ           │
│  5. Contact       │
│                   │
└───────────────────┘
```

**Placement options**:
- Sticky sidebar (desktop)
- Collapsible at top (mobile)
- Floating button that reveals TOC

### Anchor Navigation (Single Page)

```
┌─────────────────────────────────────────────────────────────────┐
│  Overview    Features    Pricing    FAQ    Contact             │
│     ↓           ↓           ↓        ↓         ↓               │
│  Smooth scroll to section on same page                         │
└─────────────────────────────────────────────────────────────────┘
```

### Tab Navigation

```
┌─────────────────────────────────────────────────────────────────┐
│  [Monthly]  [Annual]  [Enterprise]                             │
│      ↑                                                          │
│   Active tab                                                    │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Monthly pricing content...                                     │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Footer Navigation

### Standard Footer Structure

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Logo]              PRODUCT        COMPANY        RESOURCES    │
│                                                                 │
│  Brief company       Features       About Us       Blog         │
│  description or      Pricing        Careers        Help Center  │
│  value proposition   Integrations   Press          Documentation│
│                      API            Contact        Community    │
│                                                                 │
│  [Newsletter Signup Form]                                       │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  © 2024 Company Name    Privacy  Terms  Cookies                │
│                                                                 │
│  [Social Icons]                                                 │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Footer Variations

**Minimal**:
```
┌─────────────────────────────────────────────────────────────────┐
│  © 2024 Company    Privacy  Terms    [Twitter] [LinkedIn]      │
└─────────────────────────────────────────────────────────────────┘
```

**Fat footer (content-heavy)**:
```
┌─────────────────────────────────────────────────────────────────┐
│  PRODUCTS    SOLUTIONS    RESOURCES    COMPANY    SUPPORT      │
│  Item        Item         Item         Item       Item         │
│  Item        Item         Item         Item       Item         │
│  Item        Item         Item         Item       Item         │
│  Item        Item         Item         Item       Item         │
├─────────────────────────────────────────────────────────────────┤
│  [Language ▼]  [Country ▼]             © 2024 • Privacy • Terms│
└─────────────────────────────────────────────────────────────────┘
```

### Footer Must-Haves

| Essential | Nice to Have |
|-----------|--------------|
| Copyright | Newsletter signup |
| Privacy policy link | Social links |
| Terms of service link | Contact info |
| Key navigation links | Company description |

---

## Search Navigation

### Search Placement

```
Option 1: In header (always visible)
┌─────────────────────────────────────────────────────────────────┐
│  [Logo]  [────── Search ──────]        Nav Items   [CTA]       │
└─────────────────────────────────────────────────────────────────┘

Option 2: Icon that expands
┌─────────────────────────────────────────────────────────────────┐
│  [Logo]     Nav Items                            🔍   [CTA]    │
└─────────────────────────────────────────────────────────────────┘
         Click 🔍 → expands to full search bar

Option 3: In mega menu / dropdown
```

### Search Results

```
┌─────────────────────────────────────────────────────────────────┐
│  Results for "analytics"                     42 results        │
│                                                                 │
│  Products (12)    Blog Posts (18)    Help Articles (12)        │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  Analytics Dashboard                        Product     │   │
│  │  Track all your metrics in one place...                 │   │
│  └─────────────────────────────────────────────────────────┘   │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  Getting Started with Analytics             Blog        │   │
│  │  Learn how to set up your first dashboard...            │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Autocomplete/Suggestions

```
┌─────────────────────────────────────────┐
│  analy                              🔍  │
├─────────────────────────────────────────┤
│  analytics dashboard                    │
│  analytics api                          │
│  analytics pricing                      │
│  analytics vs reporting                 │
└─────────────────────────────────────────┘
```

---

## Navigation Accessibility

### Keyboard Navigation

| Key | Action |
|-----|--------|
| Tab | Move to next focusable element |
| Shift+Tab | Move to previous element |
| Enter | Activate link/button |
| Escape | Close dropdown/menu |
| Arrow keys | Navigate within menus |

### ARIA Landmarks

```html
<header role="banner">
  <nav role="navigation" aria-label="Main">
    <!-- Primary navigation -->
  </nav>
</header>

<main role="main">
  <!-- Page content -->
</main>

<footer role="contentinfo">
  <nav role="navigation" aria-label="Footer">
    <!-- Footer navigation -->
  </nav>
</footer>
```

### Skip Links

```html
<!-- First element in body -->
<a href="#main-content" class="skip-link">
  Skip to main content
</a>
```

---

## Navigation Anti-Patterns

| Anti-Pattern | Problem | Solution |
|--------------|---------|----------|
| Too many items | Decision paralysis | Limit to 7±2 items |
| Hover-only dropdowns | Mobile unusable | Click to open |
| Mystery icons | Users guess meaning | Add labels |
| Deep nesting | Hard to navigate | Flatten hierarchy |
| No current page indicator | User lost | Highlight active item |
| Tiny touch targets | Frustrating on mobile | Min 44x44px |

---

## Sources

- [Nielsen Norman Group - Navigation Design](https://www.nngroup.com/articles/navigation-menu-design/)
- [Baymard Institute - E-Commerce Navigation](https://baymard.com/blog/ecommerce-navigation)
- [Smashing Magazine - Responsive Navigation Patterns](https://www.smashingmagazine.com/2017/04/overview-responsive-navigation-patterns/)
- [W3C - Navigation Accessibility](https://www.w3.org/WAI/tutorials/menus/)
- [Google - Mobile Navigation Best Practices](https://developers.google.com/web/fundamentals/design-and-ux/responsive/)
