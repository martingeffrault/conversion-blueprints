# Material 3 Design Tokens Guide

> **Purpose**: Comprehensive token architecture for scalable, themeable design systems
> **Foundation**: Based on Material 3 principles with practical web implementation
> **Principle**: Define once, use everywhere — tokens create consistency at scale

---

## What Are Design Tokens?

Design tokens are the **atomic values** of a design system — colors, typography, spacing, shadows, and more stored as named variables. They bridge design and development.

```
Design Decision → Token → CSS Variable → Component
"Primary color"  → primary → --color-primary → .btn-primary
```

### Benefits

| Benefit | Description |
|---------|-------------|
| Consistency | Same values everywhere, no magic numbers |
| Themability | Change tokens = change entire theme |
| Maintainability | Update once, propagate everywhere |
| Communication | Shared language between design and dev |
| Scalability | Add new components using existing tokens |

---

## Token Architecture

### Three-Tier System

```
┌─────────────────────────────────────────────────────────────────┐
│  TIER 1: Reference Tokens (Primitives)                          │
│  Raw values: #722F37, 16px, 400                                 │
│  Named abstractly: red-700, space-4, weight-regular             │
└────────────────────────────┬────────────────────────────────────┘
                             ▼
┌─────────────────────────────────────────────────────────────────┐
│  TIER 2: System Tokens (Semantic)                               │
│  Purpose-based: primary, surface, on-surface                    │
│  Context-aware: scheme-light, scheme-dark                       │
└────────────────────────────┬────────────────────────────────────┘
                             ▼
┌─────────────────────────────────────────────────────────────────┐
│  TIER 3: Component Tokens                                       │
│  Specific usage: btn-bg, card-radius, input-border              │
│  Override points for fine-tuning                                │
└─────────────────────────────────────────────────────────────────┘
```

### Why Three Tiers?

| Tier | Role | Change Frequency |
|------|------|------------------|
| Reference | Define the palette | Rarely (brand changes) |
| System | Apply meaning | Sometimes (theme updates) |
| Component | Fine-tune details | Often (component tweaks) |

---

## Color Tokens

### Reference Colors (Tier 1)

Raw color values organized by hue:

```css
/* Reference palette - never used directly in components */
--ref-primary-50: #fdf2f3;
--ref-primary-100: #fce4e6;
--ref-primary-200: #f9ccd1;
--ref-primary-300: #f4a5ae;
--ref-primary-400: #ec7280;
--ref-primary-500: #e04858;
--ref-primary-600: #cc2941;
--ref-primary-700: #ab1f35;
--ref-primary-800: #8f1d31;
--ref-primary-900: #7a1c2f;
--ref-primary-950: #440a14;

/* Neutrals */
--ref-neutral-0: #ffffff;
--ref-neutral-50: #fafafa;
--ref-neutral-100: #f5f5f5;
--ref-neutral-200: #e5e5e5;
--ref-neutral-300: #d4d4d4;
--ref-neutral-400: #a3a3a3;
--ref-neutral-500: #737373;
--ref-neutral-600: #525252;
--ref-neutral-700: #404040;
--ref-neutral-800: #262626;
--ref-neutral-900: #171717;
--ref-neutral-950: #0a0a0a;
```

### System Colors (Tier 2)

Semantic colors that change based on theme:

```css
/* Light scheme */
[data-theme="light"] {
    /* Surfaces (background hierarchy) */
    --sys-surface: var(--ref-neutral-0);           /* L0: Page */
    --sys-surface-container: var(--ref-neutral-50); /* L1: Sections */
    --sys-surface-container-high: var(--ref-neutral-0); /* L2: Cards */

    /* Content on surfaces */
    --sys-on-surface: var(--ref-neutral-900);
    --sys-on-surface-variant: var(--ref-neutral-600);

    /* Primary color */
    --sys-primary: var(--ref-primary-700);
    --sys-on-primary: var(--ref-neutral-0);
    --sys-primary-container: var(--ref-primary-100);
    --sys-on-primary-container: var(--ref-primary-900);

    /* Borders */
    --sys-outline: var(--ref-neutral-300);
    --sys-outline-variant: var(--ref-neutral-200);
}

/* Dark scheme */
[data-theme="dark"] {
    --sys-surface: var(--ref-neutral-950);
    --sys-surface-container: var(--ref-neutral-900);
    --sys-surface-container-high: var(--ref-neutral-800);

    --sys-on-surface: var(--ref-neutral-50);
    --sys-on-surface-variant: var(--ref-neutral-400);

    --sys-primary: var(--ref-primary-300);
    --sys-on-primary: var(--ref-primary-900);
    --sys-primary-container: var(--ref-primary-800);
    --sys-on-primary-container: var(--ref-primary-100);

    --sys-outline: var(--ref-neutral-700);
    --sys-outline-variant: var(--ref-neutral-800);
}
```

### Surface Hierarchy

Critical for visual depth and information architecture:

```
┌─────────────────────────────────────────────────────────────────┐
│  L0: Surface (Page Background)                                  │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  L1: Surface Container (Sections)                        │   │
│  │  ┌─────────────────────────────────────────────────┐    │   │
│  │  │  L2: Surface Container High (Cards, Modals)     │    │   │
│  │  │                                                  │    │   │
│  │  └─────────────────────────────────────────────────┘    │   │
│  └─────────────────────────────────────────────────────────┘   │
└─────────────────────────────────────────────────────────────────┘
```

| Level | Token | Light Mode | Dark Mode | Usage |
|-------|-------|------------|-----------|-------|
| L0 | `surface` | White/Cream | Near black | Page background |
| L1 | `surface-container` | Light gray | Dark gray | Alternating sections |
| L2 | `surface-container-high` | White | Lighter dark | Cards, modals, dropdowns |

### Semantic Colors

For feedback and status:

```css
/* Success */
--sys-success: #22c55e;
--sys-success-container: #dcfce7;
--sys-on-success: #ffffff;

/* Warning */
--sys-warning: #eab308;
--sys-warning-container: #fef9c3;
--sys-on-warning: #1a1a1a;

/* Error */
--sys-error: #ef4444;
--sys-error-container: #fee2e2;
--sys-on-error: #ffffff;

/* Info */
--sys-info: #3b82f6;
--sys-info-container: #dbeafe;
--sys-on-info: #ffffff;
```

---

## Typography Tokens

### Type Scale

Based on a modular scale (typically 1.25 or 1.333 ratio):

```css
/* Font families */
--font-display: 'Inter', system-ui, sans-serif;
--font-body: 'Inter', system-ui, sans-serif;
--font-mono: 'JetBrains Mono', monospace;

/* Font sizes (modular scale 1.25) */
--text-xs: 0.75rem;    /* 12px */
--text-sm: 0.875rem;   /* 14px */
--text-base: 1rem;     /* 16px */
--text-lg: 1.125rem;   /* 18px */
--text-xl: 1.25rem;    /* 20px */
--text-2xl: 1.5rem;    /* 24px */
--text-3xl: 1.875rem;  /* 30px */
--text-4xl: 2.25rem;   /* 36px */
--text-5xl: 3rem;      /* 48px */
--text-6xl: 3.75rem;   /* 60px */

/* Font weights */
--weight-regular: 400;
--weight-medium: 500;
--weight-semibold: 600;
--weight-bold: 700;

/* Line heights */
--leading-tight: 1.2;
--leading-snug: 1.375;
--leading-normal: 1.5;
--leading-relaxed: 1.625;
--leading-loose: 2;

/* Letter spacing */
--tracking-tighter: -0.05em;
--tracking-tight: -0.025em;
--tracking-normal: 0;
--tracking-wide: 0.025em;
--tracking-wider: 0.05em;
```

### Typography Roles

Predefined text styles for common use cases:

```css
/* Display - Hero headlines */
--type-display-large: var(--weight-bold) var(--text-6xl)/var(--leading-tight) var(--font-display);
--type-display-medium: var(--weight-bold) var(--text-5xl)/var(--leading-tight) var(--font-display);
--type-display-small: var(--weight-bold) var(--text-4xl)/var(--leading-tight) var(--font-display);

/* Headline - Section titles */
--type-headline-large: var(--weight-semibold) var(--text-3xl)/var(--leading-snug) var(--font-display);
--type-headline-medium: var(--weight-semibold) var(--text-2xl)/var(--leading-snug) var(--font-display);
--type-headline-small: var(--weight-semibold) var(--text-xl)/var(--leading-snug) var(--font-display);

/* Title - Card titles, labels */
--type-title-large: var(--weight-medium) var(--text-lg)/var(--leading-normal) var(--font-body);
--type-title-medium: var(--weight-medium) var(--text-base)/var(--leading-normal) var(--font-body);
--type-title-small: var(--weight-medium) var(--text-sm)/var(--leading-normal) var(--font-body);

/* Body - Paragraphs */
--type-body-large: var(--weight-regular) var(--text-lg)/var(--leading-relaxed) var(--font-body);
--type-body-medium: var(--weight-regular) var(--text-base)/var(--leading-relaxed) var(--font-body);
--type-body-small: var(--weight-regular) var(--text-sm)/var(--leading-relaxed) var(--font-body);

/* Label - Buttons, form labels */
--type-label-large: var(--weight-medium) var(--text-base)/1 var(--font-body);
--type-label-medium: var(--weight-medium) var(--text-sm)/1 var(--font-body);
--type-label-small: var(--weight-medium) var(--text-xs)/1 var(--font-body);
```

---

## Spacing Tokens

### Base Scale

Using a 4px base unit:

```css
/* Spacing scale */
--space-0: 0;
--space-1: 0.25rem;   /* 4px */
--space-2: 0.5rem;    /* 8px */
--space-3: 0.75rem;   /* 12px */
--space-4: 1rem;      /* 16px */
--space-5: 1.25rem;   /* 20px */
--space-6: 1.5rem;    /* 24px */
--space-8: 2rem;      /* 32px */
--space-10: 2.5rem;   /* 40px */
--space-12: 3rem;     /* 48px */
--space-16: 4rem;     /* 64px */
--space-20: 5rem;     /* 80px */
--space-24: 6rem;     /* 96px */
--space-32: 8rem;     /* 128px */
```

### Semantic Spacing

Named for purpose:

```css
/* Component internal spacing */
--spacing-xs: var(--space-1);    /* 4px - Tight groupings */
--spacing-sm: var(--space-2);    /* 8px - Related items */
--spacing-md: var(--space-4);    /* 16px - Default padding */
--spacing-lg: var(--space-6);    /* 24px - Section padding */
--spacing-xl: var(--space-8);    /* 32px - Large sections */
--spacing-2xl: var(--space-12);  /* 48px - Major sections */

/* Section vertical spacing */
--section-padding-sm: var(--space-12);  /* 48px */
--section-padding-md: var(--space-16);  /* 64px */
--section-padding-lg: var(--space-20);  /* 80px */
--section-padding-xl: var(--space-24);  /* 96px */

/* Container max-widths */
--container-xs: 640px;
--container-sm: 768px;
--container-md: 1024px;
--container-lg: 1280px;
--container-xl: 1536px;
```

---

## Border Radius Tokens

### Scale

```css
/* Radius scale */
--radius-none: 0;
--radius-sm: 0.25rem;   /* 4px */
--radius-md: 0.5rem;    /* 8px */
--radius-lg: 0.75rem;   /* 12px */
--radius-xl: 1rem;      /* 16px */
--radius-2xl: 1.5rem;   /* 24px */
--radius-full: 9999px;  /* Pill shape */
```

### DNA-Based Radius

Design DNA controls corner style globally:

| DNA Setting | Radius Applied |
|-------------|----------------|
| `sharp` | `--radius-none` |
| `rounded` | `--radius-md` |
| `soft` | `--radius-lg` |
| `pill` | `--radius-full` |

```css
/* Applied via DNA */
--dna-radius: var(--radius-md);

/* Component tokens inherit */
--card-radius: var(--dna-radius);
--btn-radius: var(--dna-radius);
--input-radius: var(--dna-radius);
--modal-radius: calc(var(--dna-radius) * 1.5);
```

---

## Shadow Tokens

### Elevation Scale

```css
/* Shadow scale (elevation) */
--shadow-none: none;

--shadow-xs: 0 1px 2px 0 rgb(0 0 0 / 0.05);

--shadow-sm:
    0 1px 3px 0 rgb(0 0 0 / 0.1),
    0 1px 2px -1px rgb(0 0 0 / 0.1);

--shadow-md:
    0 4px 6px -1px rgb(0 0 0 / 0.1),
    0 2px 4px -2px rgb(0 0 0 / 0.1);

--shadow-lg:
    0 10px 15px -3px rgb(0 0 0 / 0.1),
    0 4px 6px -4px rgb(0 0 0 / 0.1);

--shadow-xl:
    0 20px 25px -5px rgb(0 0 0 / 0.1),
    0 8px 10px -6px rgb(0 0 0 / 0.1);

--shadow-2xl: 0 25px 50px -12px rgb(0 0 0 / 0.25);

/* Inner shadow */
--shadow-inner: inset 0 2px 4px 0 rgb(0 0 0 / 0.05);
```

### Colored Shadows

Brand-tinted shadows for premium feel:

```css
/* Brand shadow (uses primary color) */
--shadow-primary:
    0 10px 40px -10px color-mix(in srgb, var(--sys-primary) 30%, transparent);

/* Glow effect */
--shadow-glow:
    0 0 20px color-mix(in srgb, var(--sys-primary) 20%, transparent);
```

### DNA Shadow Settings

| DNA Setting | Applied Shadow |
|-------------|----------------|
| `none` | `--shadow-none` |
| `subtle` | `--shadow-sm` |
| `medium` | `--shadow-md` |
| `bold` | `--shadow-lg` |

---

## Transition Tokens

### Duration

```css
/* Durations */
--duration-instant: 0ms;
--duration-fast: 150ms;
--duration-normal: 200ms;
--duration-slow: 300ms;
--duration-slower: 500ms;
```

### Easing

```css
/* Standard easings */
--ease-linear: linear;
--ease-in: cubic-bezier(0.4, 0, 1, 1);
--ease-out: cubic-bezier(0, 0, 0.2, 1);
--ease-in-out: cubic-bezier(0.4, 0, 0.2, 1);

/* Expressive easings */
--ease-bounce: cubic-bezier(0.34, 1.56, 0.64, 1);
--ease-elastic: cubic-bezier(0.68, -0.55, 0.265, 1.55);
--ease-smooth: cubic-bezier(0.25, 0.1, 0.25, 1);
```

### Composite Transitions

```css
/* Common transitions */
--transition-colors: color var(--duration-fast) var(--ease-out),
                     background-color var(--duration-fast) var(--ease-out),
                     border-color var(--duration-fast) var(--ease-out);

--transition-opacity: opacity var(--duration-normal) var(--ease-out);

--transition-transform: transform var(--duration-normal) var(--ease-out);

--transition-all: all var(--duration-normal) var(--ease-out);

--transition-shadow: box-shadow var(--duration-normal) var(--ease-out);
```

---

## Component Tokens (Tier 3)

Fine-grained tokens for specific components:

### Button Tokens

```css
/* Button base */
--btn-height-sm: 2rem;      /* 32px */
--btn-height-md: 2.5rem;    /* 40px */
--btn-height-lg: 3rem;      /* 48px */

--btn-padding-x-sm: var(--space-3);
--btn-padding-x-md: var(--space-4);
--btn-padding-x-lg: var(--space-6);

--btn-font-size-sm: var(--text-sm);
--btn-font-size-md: var(--text-sm);
--btn-font-size-lg: var(--text-base);

--btn-font-weight: var(--weight-medium);
--btn-radius: var(--dna-radius);

/* Button variants */
--btn-primary-bg: var(--sys-primary);
--btn-primary-text: var(--sys-on-primary);
--btn-primary-hover-bg: var(--sys-primary-hover);

--btn-secondary-bg: transparent;
--btn-secondary-text: var(--sys-primary);
--btn-secondary-border: var(--sys-outline);
```

### Card Tokens

```css
/* Card structure */
--card-padding-sm: var(--space-4);
--card-padding-md: var(--space-6);
--card-padding-lg: var(--space-8);

--card-radius: var(--dna-radius);
--card-border-width: 1px;

/* Card surfaces */
--card-bg: var(--sys-surface-container-high);
--card-border: var(--sys-outline-variant);
--card-shadow: var(--dna-shadow);

/* Card hover */
--card-hover-shadow: var(--shadow-lg);
--card-hover-border: var(--sys-outline);
--card-hover-transform: translateY(-2px);
```

### Input Tokens

```css
/* Input structure */
--input-height: 2.75rem;    /* 44px - touch target */
--input-padding-x: var(--space-4);
--input-font-size: var(--text-base);
--input-radius: var(--dna-radius);

/* Input colors */
--input-bg: var(--sys-surface);
--input-border: var(--sys-outline);
--input-text: var(--sys-on-surface);
--input-placeholder: var(--sys-on-surface-variant);

/* Input states */
--input-focus-border: var(--sys-primary);
--input-focus-ring: 0 0 0 3px color-mix(in srgb, var(--sys-primary) 20%, transparent);
--input-error-border: var(--sys-error);
--input-disabled-bg: var(--sys-surface-container);
```

---

## Design DNA System

DNA tokens control global design characteristics:

### DNA Configuration

```css
/* DNA settings applied at :root */
:root {
    /* Corner style */
    --dna-corners: rounded;  /* sharp | rounded | soft | pill */
    --dna-radius: var(--radius-md);

    /* Shadow style */
    --dna-shadow-style: medium;  /* none | subtle | medium | bold */
    --dna-shadow: var(--shadow-md);

    /* Animation style */
    --dna-motion: elegant;  /* minimal | elegant | dramatic | playful */
    --dna-duration: var(--duration-normal);
    --dna-ease: var(--ease-smooth);

    /* Spacing density */
    --dna-spacing: balanced;  /* compact | balanced | generous */
    --dna-spacing-multiplier: 1;
}

/* Compact spacing */
[data-density="compact"] {
    --dna-spacing-multiplier: 0.75;
}

/* Generous spacing */
[data-density="generous"] {
    --dna-spacing-multiplier: 1.25;
}
```

### DNA Applied to Components

```css
/* Card inherits DNA */
.card {
    border-radius: var(--card-radius, var(--dna-radius));
    box-shadow: var(--card-shadow, var(--dna-shadow));
    padding: calc(var(--space-6) * var(--dna-spacing-multiplier));
    transition: var(--transition-all);
    transition-duration: var(--dna-duration);
}

/* Button inherits DNA */
.btn {
    border-radius: var(--btn-radius, var(--dna-radius));
    transition: var(--transition-all);
    transition-duration: var(--dna-duration);
    transition-timing-function: var(--dna-ease);
}
```

---

## Industry-Specific Token Adjustments

### E-Commerce

```css
/* Product-focused adjustments */
--product-image-ratio: 1;          /* Square product images */
--product-card-padding: var(--space-3);  /* Tighter for grid density */
--price-color: var(--sys-primary);
--sale-color: var(--sys-error);
--discount-badge-bg: var(--sys-error);
```

### Healthcare

```css
/* Trust and clarity focus */
--primary: #0066CC;  /* Trustworthy blue */
--body-font-size: var(--text-lg);  /* Larger for readability */
--input-height: 3rem;  /* Larger touch targets */
--card-radius: var(--radius-lg);  /* Softer, friendlier */
```

### Real Estate

```css
/* Property showcase */
--property-image-ratio: 4/3;
--gallery-thumbnail-size: 80px;
--map-height: 400px;
--price-font-size: var(--text-2xl);
```

### Finance

```css
/* Professional, secure feel */
--primary: #1E3A5F;  /* Navy blue */
--dna-corners: rounded;  /* Not too playful */
--dna-shadow-style: subtle;  /* Conservative */
--table-stripe-bg: var(--sys-surface-container);
```

### Restaurant/Food

```css
/* Warm, appetizing */
--primary: #D35400;  /* Warm orange */
--font-display: 'Playfair Display', serif;
--hero-overlay: 0.4;  /* Show food imagery */
--card-radius: var(--radius-lg);  /* Friendly */
```

---

## Implementation Checklist

### Setting Up Tokens

- [ ] Define reference color palette
- [ ] Create light and dark schemes
- [ ] Set up typography scale
- [ ] Define spacing scale
- [ ] Configure radius and shadow scales
- [ ] Set transition tokens
- [ ] Create component tokens

### Applying Tokens

- [ ] Use system tokens in components (not reference)
- [ ] Implement theme switching (data-theme attribute)
- [ ] Apply DNA settings globally
- [ ] Override component tokens where needed
- [ ] Test both light and dark modes

### Maintenance

- [ ] Document all custom tokens
- [ ] Keep token names semantic
- [ ] Avoid "magic numbers" in components
- [ ] Review tokens during design updates

---

## Token Naming Conventions

### Format

```
--[tier]-[category]-[property]-[variant]-[state]
```

### Examples

| Token | Breakdown |
|-------|-----------|
| `--ref-primary-500` | Reference → Primary → 500 shade |
| `--sys-surface-container` | System → Surface → Container variant |
| `--btn-primary-hover-bg` | Button → Primary → Hover state → Background |
| `--card-border-radius` | Card → Border → Radius |

### Rules

1. **Use kebab-case**: `--color-primary` not `--colorPrimary`
2. **Be specific**: `--btn-primary-bg` not `--btn-bg-1`
3. **State at end**: `--input-border-focus` not `--input-focus-border`
4. **Tier prefix for clarity**: `--ref-`, `--sys-`, or component name

---

## Sources

- [Material 3 Design System](https://m3.material.io/)
- [Tokens Studio Documentation](https://tokens.studio/)
- [Design Tokens W3C Draft](https://design-tokens.github.io/community-group/format/)
- [Tailwind CSS Design System](https://tailwindcss.com/docs)
- [Open Props](https://open-props.style/)
- [Style Dictionary](https://amzn.github.io/style-dictionary/)
