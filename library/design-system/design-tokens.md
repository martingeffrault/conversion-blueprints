# Design Tokens

> **Purpose**: Create consistent visual foundations through systematic design values
> **Impact**: Tokens enable design consistency, faster development, and easier theming
> **Principle**: Name tokens by purpose, not by value

---

## What Are Design Tokens?

> "Design tokens are the visual design atoms of the design system — specifically, they are named entities that store visual design attributes."
>
> *Source: [Salesforce Lightning Design System](https://www.lightningdesignsystem.com/design-tokens/)*

Design tokens are:
- **Platform-agnostic** — Work across web, iOS, Android
- **Themeable** — Change values without changing code
- **Self-documenting** — Names describe purpose
- **Single source of truth** — One place for all values

---

## Token Architecture

### Three-Tier System

```
┌─────────────────────────────────────────────────────────────────┐
│  GLOBAL TOKENS (Primitives)                                     │
│  Raw values: colors, sizes, fonts                               │
│  Example: blue-500: #3b82f6                                     │
└─────────────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────────────┐
│  SEMANTIC TOKENS (Aliases)                                      │
│  Purpose-driven references to global tokens                     │
│  Example: color-primary: {blue-500}                             │
└─────────────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────────────┐
│  COMPONENT TOKENS (Scoped)                                      │
│  Component-specific overrides                                   │
│  Example: button-primary-bg: {color-primary}                    │
└─────────────────────────────────────────────────────────────────┘
```

### Why Three Tiers?

| Tier | Purpose | When to Change |
|------|---------|----------------|
| **Global** | Define palette | Brand evolution |
| **Semantic** | Define meaning | Theme changes |
| **Component** | Define specifics | Component redesign |

---

## Color System

### Color Palette Structure

```
Primary Color
├── 50   (lightest tint)
├── 100
├── 200
├── 300
├── 400
├── 500  (base)
├── 600
├── 700
├── 800
├── 900
└── 950  (darkest shade)
```

### Global Color Tokens

| Token | Purpose | Example |
|-------|---------|---------|
| `gray-{50-950}` | Neutral palette | Backgrounds, borders, text |
| `blue-{50-950}` | Primary actions | Default primary |
| `red-{50-950}` | Errors, danger | Destructive actions |
| `green-{50-950}` | Success | Confirmations |
| `yellow-{50-950}` | Warnings | Alerts |
| `purple-{50-950}` | Accent | Alternative accent |

### Semantic Color Tokens

| Token | Maps To | Usage |
|-------|---------|-------|
| `color-primary` | `blue-600` | Primary actions, links |
| `color-primary-hover` | `blue-700` | Hover state |
| `color-primary-light` | `blue-50` | Light backgrounds |
| `color-secondary` | `gray-600` | Secondary actions |
| `color-success` | `green-600` | Success states |
| `color-warning` | `yellow-500` | Warning states |
| `color-error` | `red-600` | Error states |
| `color-info` | `blue-500` | Informational |

### Background Tokens

| Token | Light Mode | Dark Mode | Usage |
|-------|------------|-----------|-------|
| `bg-primary` | `white` | `gray-900` | Page background |
| `bg-secondary` | `gray-50` | `gray-800` | Section alternation |
| `bg-tertiary` | `gray-100` | `gray-700` | Cards, modals |
| `bg-inverse` | `gray-900` | `gray-50` | Inverted sections |

### Text Color Tokens

| Token | Light Mode | Dark Mode | Usage |
|-------|------------|-----------|-------|
| `text-primary` | `gray-900` | `gray-50` | Headings, body |
| `text-secondary` | `gray-600` | `gray-400` | Descriptions |
| `text-tertiary` | `gray-500` | `gray-500` | Captions, hints |
| `text-disabled` | `gray-400` | `gray-600` | Disabled states |
| `text-inverse` | `white` | `gray-900` | On dark backgrounds |
| `text-link` | `blue-600` | `blue-400` | Links |

### Border Tokens

| Token | Light Mode | Dark Mode | Usage |
|-------|------------|-----------|-------|
| `border-primary` | `gray-200` | `gray-700` | Default borders |
| `border-secondary` | `gray-300` | `gray-600` | Emphasized |
| `border-focus` | `blue-500` | `blue-400` | Focus rings |

---

## Typography Scale

### Type Scale (Based on 1.25 ratio)

> "A typographic scale creates visual harmony through proportional relationships."
>
> *Source: [Type-scale.com](https://type-scale.com/)*

| Token | Size | Line Height | Usage |
|-------|------|-------------|-------|
| `text-xs` | 12px | 16px | Fine print, labels |
| `text-sm` | 14px | 20px | Captions, secondary |
| `text-base` | 16px | 24px | Body text |
| `text-lg` | 18px | 28px | Lead paragraphs |
| `text-xl` | 20px | 28px | Large body |
| `text-2xl` | 24px | 32px | H4, small headings |
| `text-3xl` | 30px | 36px | H3 |
| `text-4xl` | 36px | 40px | H2 |
| `text-5xl` | 48px | 48px | H1 |
| `text-6xl` | 60px | 60px | Display |
| `text-7xl` | 72px | 72px | Hero |

### Font Weight Tokens

| Token | Value | Usage |
|-------|-------|-------|
| `font-thin` | 100 | Rarely used |
| `font-light` | 300 | Display text |
| `font-normal` | 400 | Body text |
| `font-medium` | 500 | Emphasized body |
| `font-semibold` | 600 | Subheadings |
| `font-bold` | 700 | Headings |
| `font-extrabold` | 800 | Display headings |

### Font Family Tokens

| Token | Default | Usage |
|-------|---------|-------|
| `font-sans` | Inter, system-ui | UI, body |
| `font-serif` | Georgia, serif | Editorial |
| `font-mono` | JetBrains Mono | Code |
| `font-display` | Custom display | Heroes |

### Line Height Tokens

| Token | Value | Usage |
|-------|-------|-------|
| `leading-none` | 1 | Single line headings |
| `leading-tight` | 1.25 | Headings |
| `leading-snug` | 1.375 | Subheadings |
| `leading-normal` | 1.5 | Body text |
| `leading-relaxed` | 1.625 | Long-form |
| `leading-loose` | 2 | Spacious text |

### Letter Spacing Tokens

| Token | Value | Usage |
|-------|-------|-------|
| `tracking-tighter` | -0.05em | Large headings |
| `tracking-tight` | -0.025em | Headings |
| `tracking-normal` | 0 | Body text |
| `tracking-wide` | 0.025em | Small caps |
| `tracking-wider` | 0.05em | Labels |
| `tracking-widest` | 0.1em | All caps |

---

## Spacing System

### 8-Point Grid Scale

> "The 8pt grid is a design system that uses multiples of 8 to define dimensions, padding, and margins."
>
> *Source: [Spec.fm](https://spec.fm/specifics/8-pt-grid)*

| Token | Value | Pixels | Usage |
|-------|-------|--------|-------|
| `space-0` | 0 | 0px | Reset |
| `space-px` | 1px | 1px | Hairlines |
| `space-0.5` | 0.125rem | 2px | Micro spacing |
| `space-1` | 0.25rem | 4px | Icon gaps |
| `space-2` | 0.5rem | 8px | Compact spacing |
| `space-3` | 0.75rem | 12px | Small gaps |
| `space-4` | 1rem | 16px | Base spacing |
| `space-5` | 1.25rem | 20px | Medium-small |
| `space-6` | 1.5rem | 24px | Medium |
| `space-8` | 2rem | 32px | Large |
| `space-10` | 2.5rem | 40px | Extra large |
| `space-12` | 3rem | 48px | Section padding |
| `space-16` | 4rem | 64px | Large sections |
| `space-20` | 5rem | 80px | Hero spacing |
| `space-24` | 6rem | 96px | Major sections |
| `space-32` | 8rem | 128px | Full sections |

### Semantic Spacing Tokens

| Token | Value | Usage |
|-------|-------|-------|
| `spacing-page-x` | `space-4` → `space-8` | Page horizontal padding |
| `spacing-section-y` | `space-16` → `space-24` | Section vertical padding |
| `spacing-card-padding` | `space-6` | Card internal padding |
| `spacing-stack-sm` | `space-2` | Small vertical rhythm |
| `spacing-stack-md` | `space-4` | Medium vertical rhythm |
| `spacing-stack-lg` | `space-8` | Large vertical rhythm |
| `spacing-inline-sm` | `space-2` | Small horizontal gaps |
| `spacing-inline-md` | `space-4` | Medium horizontal gaps |
| `spacing-inline-lg` | `space-6` | Large horizontal gaps |

---

## Elevation (Shadows)

### Shadow Scale

| Token | Value | Usage |
|-------|-------|-------|
| `shadow-none` | none | Flat elements |
| `shadow-sm` | 0 1px 2px rgba(0,0,0,0.05) | Subtle lift |
| `shadow-md` | 0 4px 6px rgba(0,0,0,0.1) | Cards |
| `shadow-lg` | 0 10px 15px rgba(0,0,0,0.1) | Dropdowns |
| `shadow-xl` | 0 20px 25px rgba(0,0,0,0.1) | Modals |
| `shadow-2xl` | 0 25px 50px rgba(0,0,0,0.25) | Dialogs |
| `shadow-inner` | inset 0 2px 4px rgba(0,0,0,0.05) | Inset elements |

### Elevation Levels

| Level | Shadow | Z-Index | Elements |
|-------|--------|---------|----------|
| 0 | none | 0 | Background |
| 1 | sm | 10 | Cards at rest |
| 2 | md | 20 | Cards on hover |
| 3 | lg | 30 | Dropdowns |
| 4 | xl | 40 | Modals |
| 5 | 2xl | 50 | Notifications |

---

## Border Radius

### Radius Scale

| Token | Value | Usage |
|-------|-------|-------|
| `rounded-none` | 0 | Sharp corners |
| `rounded-sm` | 2px | Subtle rounding |
| `rounded-md` | 4px | Default buttons |
| `rounded-lg` | 8px | Cards |
| `rounded-xl` | 12px | Large cards |
| `rounded-2xl` | 16px | Modals |
| `rounded-3xl` | 24px | Hero cards |
| `rounded-full` | 9999px | Pills, avatars |

### Semantic Radius Tokens

| Token | Value | Usage |
|-------|-------|-------|
| `radius-button` | `rounded-md` | Buttons |
| `radius-input` | `rounded-md` | Form inputs |
| `radius-card` | `rounded-lg` | Cards |
| `radius-modal` | `rounded-xl` | Modals |
| `radius-badge` | `rounded-full` | Badges, pills |

---

## Breakpoints

### Breakpoint Scale

> "Design mobile-first, enhance progressively."

| Token | Value | Target |
|-------|-------|--------|
| `screen-sm` | 640px | Large phones |
| `screen-md` | 768px | Tablets |
| `screen-lg` | 1024px | Laptops |
| `screen-xl` | 1280px | Desktops |
| `screen-2xl` | 1536px | Large screens |

### Container Widths

| Token | Value | Usage |
|-------|-------|-------|
| `container-sm` | 640px | Narrow content |
| `container-md` | 768px | Article width |
| `container-lg` | 1024px | Standard width |
| `container-xl` | 1280px | Wide content |
| `container-2xl` | 1536px | Full width |

---

## Animation Tokens

### Duration Scale

| Token | Value | Usage |
|-------|-------|-------|
| `duration-75` | 75ms | Micro interactions |
| `duration-100` | 100ms | Quick feedback |
| `duration-150` | 150ms | Button states |
| `duration-200` | 200ms | Default |
| `duration-300` | 300ms | Emphasis |
| `duration-500` | 500ms | Complex |
| `duration-700` | 700ms | Large elements |
| `duration-1000` | 1000ms | Page transitions |

### Easing Functions

| Token | Value | Usage |
|-------|-------|-------|
| `ease-linear` | linear | Continuous |
| `ease-in` | cubic-bezier(0.4, 0, 1, 1) | Exit |
| `ease-out` | cubic-bezier(0, 0, 0.2, 1) | Enter |
| `ease-in-out` | cubic-bezier(0.4, 0, 0.2, 1) | Default |
| `ease-bounce` | cubic-bezier(0.34, 1.56, 0.64, 1) | Playful |

---

## Token Naming Conventions

### Naming Structure

```
{category}-{property}-{variant}-{state}
```

Examples:
- `color-background-primary`
- `text-size-heading-lg`
- `spacing-padding-card`
- `button-background-primary-hover`

### Naming Rules

| Rule | Good | Bad |
|------|------|-----|
| Purpose over value | `color-primary` | `color-blue` |
| Consistent prefixes | `text-primary` | `primary-text` |
| Lowercase with dashes | `font-weight-bold` | `fontWeightBold` |
| No magic numbers | `space-4` | `space-17` |
| Semantic over visual | `color-error` | `color-red` |

---

## Dark Mode Strategy

### Approach Options

| Strategy | Description | Best For |
|----------|-------------|----------|
| **Semantic inversion** | Swap semantic tokens | Most apps |
| **Separate palettes** | Distinct dark palette | Premium brands |
| **Calculated** | Programmatic adjustment | Large systems |

### Token Mapping Example

| Semantic Token | Light Value | Dark Value |
|----------------|-------------|------------|
| `bg-primary` | `white` | `gray-900` |
| `bg-secondary` | `gray-50` | `gray-800` |
| `text-primary` | `gray-900` | `gray-50` |
| `text-secondary` | `gray-600` | `gray-400` |
| `border-primary` | `gray-200` | `gray-700` |

### Implementation Pattern

```css
:root {
  --color-bg-primary: var(--white);
  --color-text-primary: var(--gray-900);
}

[data-theme="dark"] {
  --color-bg-primary: var(--gray-900);
  --color-text-primary: var(--gray-50);
}
```

---

## Token Organization

### File Structure

```
tokens/
├── global/
│   ├── colors.json
│   ├── typography.json
│   ├── spacing.json
│   ├── elevation.json
│   └── animation.json
├── semantic/
│   ├── colors.json
│   ├── typography.json
│   └── spacing.json
├── component/
│   ├── button.json
│   ├── card.json
│   └── form.json
└── themes/
    ├── light.json
    └── dark.json
```

### Documentation Requirements

Each token should include:
- **Name**: Token identifier
- **Value**: Current value
- **Description**: Purpose and usage
- **Category**: Grouping
- **Type**: color, dimension, etc.

---

## Sources

- [Salesforce Lightning Design Tokens](https://www.lightningdesignsystem.com/design-tokens/)
- [Google Material Design 3 Tokens](https://m3.material.io/foundations/design-tokens/overview)
- [Tailwind CSS Default Configuration](https://tailwindcss.com/docs/configuration)
- [Nathan Curtis - Tokens in Design Systems](https://medium.com/eightshapes-llc/tokens-in-design-systems-25dd82d58421)
- [Design Tokens W3C Community Group](https://www.designtokens.org/)
- [Style Dictionary](https://amzn.github.io/style-dictionary/)
