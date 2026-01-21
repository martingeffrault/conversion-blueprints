# Spacing & Layout Systems

> **Purpose**: Create predictable, harmonious layouts through systematic spacing
> **Impact**: Consistent spacing improves scannability, reduces cognitive load, increases trust
> **Principle**: Spacing is a relationship — elements grouped by proximity share meaning

---

## The Science of Spacing

### Gestalt Law of Proximity

> "Objects that are near, or proximate to each other, tend to be grouped together."
>
> *Source: [Laws of UX](https://lawsofux.com/law-of-proximity/)*

Elements with **less space between them** are perceived as related. This principle drives all spacing decisions.

### Spacing Creates Hierarchy

| Spacing Amount | Perception | Example |
|----------------|------------|---------|
| Tight (4-8px) | Same group | Label + input |
| Medium (16-24px) | Related items | List items |
| Large (32-48px) | Different groups | Sections |
| Very large (64px+) | Major divisions | Page sections |

---

## The 8-Point Grid System

### Why 8 Points?

> "8 is a highly composite number, divisible by 2 and 4, allowing for easy subdivision and scaling."
>
> *Source: [Spec.fm - 8pt Grid](https://spec.fm/specifics/8-pt-grid)*

| Base | Multiples |
|------|-----------|
| 8px | 8, 16, 24, 32, 40, 48, 56, 64, 72, 80... |
| 4px soft grid | 4, 8, 12, 16, 20, 24... (for icons, small elements) |

### 8-Point Scale

```
4px  ──  Micro (icons, badges)
8px  ──  XS (tight grouping)
12px ──  SM (compact)
16px ──  MD (base unit)
24px ──  LG (comfortable)
32px ──  XL (spacious)
48px ──  2XL (section gaps)
64px ──  3XL (major sections)
96px ──  4XL (hero spacing)
128px ── 5XL (full sections)
```

### Applying the Grid

| Context | Spacing Range |
|---------|---------------|
| Icon + text | 4-8px |
| Form label + input | 4-8px |
| List items | 8-16px |
| Card content | 16-24px |
| Cards in grid | 16-32px |
| Section content | 24-48px |
| Between sections | 64-128px |

---

## Spacing Tokens

### Absolute Spacing Scale

| Token | Value | Usage |
|-------|-------|-------|
| `--space-0` | 0 | Reset |
| `--space-1` | 4px | Micro |
| `--space-2` | 8px | XS |
| `--space-3` | 12px | SM |
| `--space-4` | 16px | MD (base) |
| `--space-5` | 20px | MD+ |
| `--space-6` | 24px | LG |
| `--space-8` | 32px | XL |
| `--space-10` | 40px | XL+ |
| `--space-12` | 48px | 2XL |
| `--space-16` | 64px | 3XL |
| `--space-20` | 80px | 3XL+ |
| `--space-24` | 96px | 4XL |
| `--space-32` | 128px | 5XL |

### Semantic Spacing Tokens

| Token | Value | Purpose |
|-------|-------|---------|
| `--spacing-inline-xs` | 4px | Icon-text gaps |
| `--spacing-inline-sm` | 8px | Button icon gaps |
| `--spacing-inline-md` | 16px | Horizontal content |
| `--spacing-inline-lg` | 24px | Wide horizontal gaps |
| `--spacing-stack-xs` | 4px | Tight vertical |
| `--spacing-stack-sm` | 8px | Compact vertical |
| `--spacing-stack-md` | 16px | Standard vertical |
| `--spacing-stack-lg` | 24px | Spacious vertical |
| `--spacing-stack-xl` | 32px | Section internal |

### Component Spacing Tokens

| Token | Value | Component |
|-------|-------|-----------|
| `--button-padding-x` | 16-24px | Button horizontal |
| `--button-padding-y` | 8-12px | Button vertical |
| `--input-padding-x` | 12-16px | Input horizontal |
| `--input-padding-y` | 8-12px | Input vertical |
| `--card-padding` | 24-32px | Card internal |
| `--modal-padding` | 24-32px | Modal internal |

---

## Layout Systems

### Container System

```
┌─────────────────────────────────────────────────────────────────┐
│  ← Page Margin →│← Container (max-width) →│← Page Margin →     │
│                 │                         │                     │
│     16-64px     │      640-1280px        │      16-64px        │
│                 │                         │                     │
└─────────────────────────────────────────────────────────────────┘
```

### Container Widths

| Token | Width | Usage |
|-------|-------|-------|
| `--container-xs` | 480px | Forms, narrow content |
| `--container-sm` | 640px | Article text |
| `--container-md` | 768px | Standard content |
| `--container-lg` | 1024px | Wide content |
| `--container-xl` | 1280px | Full layouts |
| `--container-2xl` | 1536px | Dashboard layouts |

### Responsive Page Margins

| Breakpoint | Margin | Reasoning |
|------------|--------|-----------|
| Mobile (<640px) | 16px | Maximum content space |
| Tablet (640-1024px) | 24-32px | Comfortable padding |
| Desktop (1024px+) | 64px+ or fluid | Centered containers |

---

## Grid Systems

### 12-Column Grid

The 12-column grid is the industry standard because 12 is divisible by 2, 3, 4, and 6.

```
│ 1 │ 2 │ 3 │ 4 │ 5 │ 6 │ 7 │ 8 │ 9 │ 10│ 11│ 12│
├───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┴───┤
│               Full Width (12)                  │
├───────────────────────────┬───────────────────┤
│       Two-thirds (8)      │   One-third (4)   │
├───────────────────┬───────┴───────────────────┤
│    Half (6)       │         Half (6)          │
├─────────┬─────────┼─────────┬─────────────────┤
│ 1/4 (3) │ 1/4 (3) │ 1/4 (3) │     1/4 (3)     │
└─────────┴─────────┴─────────┴─────────────────┘
```

### Common Column Patterns

| Pattern | Columns | Use Case |
|---------|---------|----------|
| Full | 12 | Hero, full-width sections |
| Sidebar + Content | 3 + 9 or 4 + 8 | Blog, docs |
| Two columns | 6 + 6 | Comparison, features |
| Three columns | 4 + 4 + 4 | Card grids, features |
| Four columns | 3 + 3 + 3 + 3 | Gallery, team |
| Asymmetric | 5 + 7 or 7 + 5 | Hero with image |

### Grid Gutter Sizes

| Size | Gutter | Usage |
|------|--------|-------|
| Tight | 16px | Compact grids, mobile |
| Default | 24px | Standard layouts |
| Spacious | 32px | Card grids |
| Wide | 48px | Feature sections |

### Auto-Fit vs Auto-Fill

```css
/* Auto-fill: Maintains column size, adds empty columns */
grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));

/* Auto-fit: Stretches columns to fill space */
grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
```

| Property | Behavior | Best For |
|----------|----------|----------|
| `auto-fill` | Creates empty tracks | Fixed-size cards |
| `auto-fit` | Collapses empty tracks | Flexible layouts |

---

## Section Rhythm

### Vertical Section Spacing

```
┌──────────────────────────────────────────────────────────────┐
│                          HERO                                 │
│                     (special: 80-120px)                       │
├──────────────────────────────────────────────────────────────┤
│                                                               │
│                    64-96px gap                                │
│                                                               │
├──────────────────────────────────────────────────────────────┤
│                      SECTION 1                                │
│                   (padding: 64-96px)                          │
├──────────────────────────────────────────────────────────────┤
│                                                               │
│                    64-96px gap                                │
│                                                               │
├──────────────────────────────────────────────────────────────┤
│                      SECTION 2                                │
│                   (padding: 64-96px)                          │
└──────────────────────────────────────────────────────────────┘
```

### Section Padding Scale

| Section Type | Mobile | Tablet | Desktop |
|--------------|--------|--------|---------|
| Hero | 48px | 64px | 96px+ |
| Standard | 48px | 64px | 80px |
| Compact | 32px | 48px | 64px |
| CTA | 48px | 64px | 80px |
| Footer | 48px | 64px | 80px |

### Internal Section Rhythm

```
Section
├── Section header (title + subtitle)
│   └── 32-48px gap after header
├── Section content
│   ├── Item 1
│   │   └── 16-24px gap
│   ├── Item 2
│   │   └── 16-24px gap
│   └── Item 3
│       └── 32-48px gap to CTA
└── Section CTA (optional)
```

---

## Component Spacing Patterns

### Card Spacing

```
┌─────────────────────────────────────────────┐
│                                             │
│  ← 24px padding →                           │
│                                             │
│    ┌─────────────────────────────────┐     │
│    │         Image/Media             │     │
│    └─────────────────────────────────┘     │
│                                             │
│    ← 16px gap →                             │
│                                             │
│    Title                                    │
│                                             │
│    ← 8px gap →                              │
│                                             │
│    Description text that wraps              │
│    to multiple lines                        │
│                                             │
│    ← 16px gap →                             │
│                                             │
│    [Button]                                 │
│                                             │
│  ← 24px padding →                           │
│                                             │
└─────────────────────────────────────────────┘
```

### Form Spacing

```
┌─────────────────────────────────────────────┐
│                                             │
│  Label                                      │
│  ← 4-8px gap →                              │
│  ┌─────────────────────────────────────┐   │
│  │ Input field                         │   │
│  └─────────────────────────────────────┘   │
│  ← 4px gap →                                │
│  Helper text                                │
│                                             │
│  ← 16-24px gap to next field →              │
│                                             │
│  Label                                      │
│  ← 4-8px gap →                              │
│  ┌─────────────────────────────────────┐   │
│  │ Input field                         │   │
│  └─────────────────────────────────────┘   │
│                                             │
│  ← 24-32px gap to button →                  │
│                                             │
│  [Submit Button]                            │
│                                             │
└─────────────────────────────────────────────┘
```

### Navigation Spacing

```
┌─────────────────────────────────────────────────────────────┐
│  Logo      ← 32px →   Nav Item  ← 24px →  Nav Item  │ CTA  │
│                                                     │      │
│  ←16px→                                        ←16px→      │
└─────────────────────────────────────────────────────────────┘
```

| Element | Spacing |
|---------|---------|
| Logo to nav | 32-48px |
| Nav items | 16-32px between |
| Nav to CTA | 24-32px |
| Header padding | 16-24px vertical |

---

## Responsive Spacing Strategy

### Spacing Multipliers by Breakpoint

| Breakpoint | Multiplier | Base → Result |
|------------|------------|---------------|
| Mobile | 0.75x | 64px → 48px |
| Tablet | 0.875x | 64px → 56px |
| Desktop | 1x | 64px → 64px |
| Large | 1.25x | 64px → 80px |

### Fluid Spacing with Clamp

```css
/* Fluid section padding: 48px → 96px */
padding: clamp(3rem, 5vw + 1.5rem, 6rem);

/* Fluid container margin: 16px → 64px */
margin-inline: clamp(1rem, 4vw, 4rem);

/* Fluid gap: 16px → 32px */
gap: clamp(1rem, 2vw + 0.5rem, 2rem);
```

### Responsive Spacing Tokens

```css
:root {
  --section-padding: 48px;
  --card-gap: 16px;
}

@media (min-width: 768px) {
  :root {
    --section-padding: 64px;
    --card-gap: 24px;
  }
}

@media (min-width: 1024px) {
  :root {
    --section-padding: 80px;
    --card-gap: 32px;
  }
}
```

---

## Common Spacing Mistakes

### Mistake 1: Inconsistent Spacing

| Problem | Solution |
|---------|----------|
| Random padding values | Use spacing scale tokens |
| Different gaps in similar contexts | Apply same token to same element types |
| "Eyeballing" | Always reference the scale |

### Mistake 2: Too Much or Too Little

| Context | Too Little | Just Right | Too Much |
|---------|------------|------------|----------|
| Card padding | 8px | 24px | 48px |
| Section padding | 24px | 64-80px | 160px |
| Between sections | 16px | 64-96px | 200px |

### Mistake 3: Ignoring Content Relationships

| Wrong | Right |
|-------|-------|
| Same gap everywhere | Tighter gaps within groups, larger between |
| Label far from input | Label close to input (4-8px) |
| Related items separated | Group related items with tight spacing |

### Mistake 4: Not Accounting for Line Height

Line height adds visual space. Account for it:
- 16px font with 1.5 line height = 24px total height
- 8px margin may look like 16px+ visually

---

## Layout Patterns

### Split Layout (50/50 or 60/40)

```
┌─────────────────────────┬─────────────────────────┐
│                         │                         │
│         Content         │         Image           │
│                         │                         │
│    ← padding: 48px →    │    ← padding: 48px →    │
│                         │                         │
└─────────────────────────┴─────────────────────────┘
        ↑ gap: 48-64px ↑
```

### Z-Pattern Layout

```
┌─────────────────────────────────────────────────────┐
│  Logo                                        CTA    │
│    ↘                                       ↗        │
│       ↘                                 ↗           │
│          ↘                           ↗              │
│             [Main Content Area]                     │
│          ↗                           ↘              │
│       ↗                                 ↘           │
│    ↗                                       ↘        │
│  Secondary Info                     Secondary CTA   │
└─────────────────────────────────────────────────────┘
```

### F-Pattern Layout

```
┌─────────────────────────────────────────────────────┐
│  Header ─────────────────────────────────────────   │ ← Primary scan
│                                                     │
│  Subheader ──────────────────────────               │ ← Secondary scan
│                                                     │
│  Content ───                                        │
│  Content ──                                         │ ← Vertical scan
│  Content ─                                          │
│  Content                                            │
└─────────────────────────────────────────────────────┘
```

---

## Checklist

### Spacing Audit

- [ ] Using 8-point grid consistently
- [ ] Semantic spacing tokens defined
- [ ] Related elements grouped with tight spacing
- [ ] Unrelated elements separated with large spacing
- [ ] Section rhythm is consistent
- [ ] Responsive spacing scales appropriately
- [ ] Card spacing is consistent across all cards
- [ ] Form spacing follows best practices
- [ ] Navigation spacing is comfortable
- [ ] No orphaned elements with inconsistent spacing

---

## Sources

- [Spec.fm - 8pt Grid](https://spec.fm/specifics/8-pt-grid)
- [Material Design - Layout](https://m3.material.io/foundations/layout/understanding-layout)
- [Laws of UX - Law of Proximity](https://lawsofux.com/law-of-proximity/)
- [Nathan Curtis - Space in Design Systems](https://medium.com/eightshapes-llc/space-in-design-systems-188bcbae0d62)
- [Smashing Magazine - Spacing in CSS](https://www.smashingmagazine.com/2019/03/css-alignment/)
- [Every Layout](https://every-layout.dev/)
