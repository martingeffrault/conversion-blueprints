# Visual Hierarchy

> **Purpose**: Guide user attention through intentional design choices
> **Impact**: Clear hierarchy reduces cognitive load and improves comprehension — [HCI.org](https://www.hci.org.uk/article/the-impact-of-visual-hierarchy-in-user-interface-design-a-cognitive-perspective/)
> **Principle**: If everything is important, nothing is important

---

## What Is Visual Hierarchy?

> "Visual hierarchy is the arrangement of graphic elements in a design in order of importance of each element."
>
> *Source: [Interaction Design Foundation](https://www.interaction-design.org/literature/topics/visual-hierarchy)*

Visual hierarchy tells users:
1. **Where to look first**
2. **What's most important**
3. **How information relates**
4. **What actions to take**

---

## The Six Principles of Visual Hierarchy

### 1. Size & Scale

**Larger elements command more attention.**

| Element | Typical Scale | Impact |
|---------|---------------|--------|
| Hero headline | 48-72px | Highest attention |
| Section titles | 30-36px | Major divisions |
| Subheadings | 20-24px | Secondary divisions |
| Body text | 16-18px | Content consumption |
| Captions | 12-14px | Supporting info |

**Golden Ratio Scale**: 1.618x between levels
- 16px → 26px → 42px → 68px

**Modular Scale**: Consistent multiplier (1.25, 1.333, 1.5)
- 16px → 20px → 25px → 31px → 39px → 49px

### 2. Color & Contrast

**High contrast draws attention; low contrast recedes.**

| Contrast Level | Usage | Example |
|----------------|-------|---------|
| **High** (7:1+) | Headlines, CTAs | Black on white |
| **Medium** (4.5:1) | Body text | Dark gray on white |
| **Low** (3:1) | Secondary text | Gray on white |
| **Color accent** | CTAs, important | Blue button on gray |

**Color for Emphasis**:
```
Primary color → Primary CTA, key links
Success green → Positive actions, confirmations
Warning yellow → Alerts, caution
Error red → Errors, destructive actions
Neutral gray → Secondary content
```

### 3. Position & Placement

**Top-left gets seen first; bottom-right gets seen last** (in LTR languages).

Reading patterns:
- **F-Pattern**: Content-heavy pages (blogs, listings)
- **Z-Pattern**: Landing pages, sparse content
- **Center focus**: Hero sections, modals

| Position | Attention Level |
|----------|-----------------|
| Top-left | Very high |
| Top-center | High |
| Top-right | High (for CTAs) |
| Center | High |
| Bottom-center | Medium |
| Bottom-right | Lower (but good for CTAs) |

### 4. Typography Weight & Style

**Heavier weights and distinct styles create emphasis.**

| Style | Usage |
|-------|-------|
| **Bold (700)** | Headlines, emphasis |
| **Semi-bold (600)** | Subheadings |
| **Medium (500)** | Navigation, labels |
| **Regular (400)** | Body text |
| **Light (300)** | Large display text |
| *Italic* | Emphasis, quotes |
| CAPS | Labels, badges |

### 5. White Space (Negative Space)

**More space around an element = more importance.**

> "White space is to be regarded as an active element, not a passive background."
>
> *— Jan Tschichold*

| Spacing Amount | Signal |
|----------------|--------|
| Generous padding | Premium, important |
| Normal padding | Standard content |
| Tight padding | Dense info, related items |
| Isolated element | Call attention |

### 6. Proximity & Grouping

**Related items should be close together.**

Gestalt Law of Proximity:
- Tight spacing = related
- Wide spacing = separate

```
Title                    ← Tight (8px)
Subtitle
                         ← Wide (32px)
[Unrelated Element]
```

---

## Typography Hierarchy

### Heading Levels

| Level | Usage | Size Range | Weight |
|-------|-------|------------|--------|
| H1 | Page title (once) | 36-72px | Bold |
| H2 | Major sections | 28-36px | Semi-bold |
| H3 | Subsections | 22-28px | Semi-bold |
| H4 | Minor headings | 18-22px | Medium |
| H5 | Small headings | 16-18px | Medium |
| H6 | Micro headings | 14-16px | Medium |

### Text Hierarchy Stack

```
EYEBROW                          ← 12-14px, uppercase, tracking, muted
Hero Headline                    ← 48-72px, bold, tight leading
Supporting subheadline           ← 20-24px, normal, muted color

Section Title                    ← 28-36px, semi-bold
Section description              ← 16-18px, muted

Card Title                       ← 18-22px, semi-bold
Card body text that describes    ← 14-16px, normal
the card content.

Caption or metadata              ← 12-14px, muted
```

### Type Pairing Guidelines

| Heading Font | Body Font | Vibe |
|--------------|-----------|------|
| Sans-serif (Inter) | Sans-serif (Inter) | Modern, clean |
| Serif (Playfair) | Sans-serif (Inter) | Editorial, elegant |
| Display (Clash) | Sans-serif (Inter) | Bold, contemporary |
| Rounded (Nunito) | Sans-serif (Inter) | Friendly, approachable |

---

## Color Hierarchy

### The 60-30-10 Rule

| Percentage | Usage | Example |
|------------|-------|---------|
| 60% | Dominant (backgrounds) | White/light gray |
| 30% | Secondary (text, cards) | Dark gray, off-white |
| 10% | Accent (CTAs, highlights) | Brand color |

### Color as Priority Signal

| Color Role | Elements |
|------------|----------|
| **Primary** | Main CTA, active states |
| **Secondary** | Secondary buttons, links |
| **Neutral dark** | Headlines, body text |
| **Neutral light** | Backgrounds, dividers |
| **Accent** | Badges, highlights |

### Contrast Hierarchy

| Element | Min Contrast | Reasoning |
|---------|--------------|-----------|
| Body text | 4.5:1 | WCAG AA readability |
| Large text (24px+) | 3:1 | Larger = easier to read |
| Icons + graphics | 3:1 | UI components |
| Non-essential | No minimum | Decorative |

---

## Component Hierarchy

### Card Hierarchy

```
┌─────────────────────────────────────────────────┐
│                                                 │
│  [Badge]                     ← Small, colorful  │
│                                                 │
│  Card Title                  ← Largest, bold    │
│                                                 │
│  Supporting description      ← Medium, muted    │
│  text for the card.                             │
│                                                 │
│  [CTA Button]                ← Prominent        │
│                                                 │
│  Secondary link              ← Smaller, subtle  │
│                                                 │
└─────────────────────────────────────────────────┘
```

### Hero Section Hierarchy

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│                        EYEBROW TEXT                             │
│                                                                 │
│              Main Headline That                                 │
│              Commands Attention                                 │
│                                                                 │
│       Supporting text that provides context and                 │
│       explains the value proposition clearly.                   │
│                                                                 │
│            [Primary CTA]    Secondary Link                      │
│                                                                 │
│                     Social proof element                        │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Navigation Hierarchy

```
┌──────────────────────────────────────────────────────────────────┐
│  LOGO          Nav 1    Nav 2    Nav 3    Nav 4      [CTA]      │
│   ↑               ↑                                     ↑        │
│  Prominent    Regular weight                      Primary button │
│                  ↓                                               │
│              Active = Bold/underlined                            │
└──────────────────────────────────────────────────────────────────┘
```

---

## Page-Level Hierarchy

### Landing Page Pattern

```
1. Hero (Highest priority)
   └── Headline + CTA

2. Social Proof
   └── Logos, numbers

3. Features/Benefits
   └── Value propositions

4. How It Works
   └── Process explanation

5. Testimonials
   └── Trust building

6. Pricing (if applicable)
   └── Decision support

7. FAQ
   └── Objection handling

8. Final CTA
   └── Last conversion attempt

9. Footer
   └── Lowest priority navigation
```

### Blog Article Pattern

```
1. Title (H1)
   └── Highest priority

2. Meta (date, author, reading time)
   └── Supporting info

3. Lead paragraph
   └── Key takeaway

4. Section headers (H2)
   └── Content structure

5. Body paragraphs
   └── Main content

6. Subsection headers (H3)
   └── Detailed structure

7. Callouts/quotes
   └── Emphasized points

8. Conclusion
   └── Summary/CTA
```

---

## Creating Hierarchy: Step by Step

### Step 1: Identify Priorities

Rank all page elements by importance:
1. **Critical**: Must see immediately
2. **Important**: Should see soon
3. **Supportive**: Helpful context
4. **Optional**: Nice to have

### Step 2: Apply Size Contrast

| Priority | Size Treatment |
|----------|----------------|
| Critical | Largest (2-3x body) |
| Important | Large (1.5-2x body) |
| Supportive | Normal (body size) |
| Optional | Small (0.8-0.9x body) |

### Step 3: Apply Color Contrast

| Priority | Color Treatment |
|----------|-----------------|
| Critical | High contrast, brand color |
| Important | High contrast, neutral |
| Supportive | Medium contrast |
| Optional | Low contrast, muted |

### Step 4: Apply Spacing

| Priority | Spacing Treatment |
|----------|-------------------|
| Critical | Generous white space |
| Important | Good white space |
| Supportive | Normal spacing |
| Optional | Tighter spacing |

### Step 5: Test with Squint Test

Blur your vision (squint) and see if hierarchy is still clear.

---

## Common Hierarchy Mistakes

### Mistake 1: Competing Headlines

| Wrong | Right |
|-------|-------|
| Two 48px headlines | One 48px hero, others smaller |
| Multiple bold red CTAs | One primary CTA per section |

### Mistake 2: Burying CTAs

| Wrong | Right |
|-------|-------|
| CTA same color as body text | CTA in brand color, high contrast |
| CTA at bottom, small | CTA prominent, above fold |

### Mistake 3: Too Many Levels

| Wrong | Right |
|-------|-------|
| H1, H2, H3, H4, H5, H6 on one page | Max 3-4 heading levels |
| 10 different text sizes | 5-6 distinct sizes |

### Mistake 4: Uniform Spacing

| Wrong | Right |
|-------|-------|
| 20px between everything | Variable: 8px, 16px, 32px, 64px |
| Related items same spacing as unrelated | Grouped items closer |

### Mistake 5: Low Contrast Text

| Wrong | Right |
|-------|-------|
| Light gray on white (#999 on #fff) | Dark gray on white (#333 on #fff) |
| Decorative over functional | Readable first |

---

## Hierarchy Testing Methods

### 5-Second Test

1. Show page for 5 seconds
2. Ask: "What is this page about?"
3. If unclear → hierarchy needs work

### Squint Test

1. Blur vision or zoom out
2. Can you still identify:
   - Main headline?
   - Primary CTA?
   - Key sections?

### Grayscale Test

1. View design in grayscale
2. If hierarchy disappears → relying too much on color

### Attention Heatmap

Tools like Attention Insight or EyeQuant predict where users look first.

---

## Hierarchy Checklist

### Page Level
- [ ] Single clear H1 headline
- [ ] Consistent heading hierarchy (H1 → H2 → H3)
- [ ] One primary CTA per section
- [ ] Visual flow guides eye naturally
- [ ] Most important info above fold

### Component Level
- [ ] Clear title/body/action distinction
- [ ] Consistent sizing within component types
- [ ] Primary vs secondary actions distinct
- [ ] Related elements grouped visually

### Text Level
- [ ] Obvious heading vs body distinction
- [ ] Links distinguishable from body text
- [ ] Emphasis (bold/italic) used sparingly
- [ ] Line length aids readability (50-75 chars)

---

## Sources

- [Interaction Design Foundation - Visual Hierarchy](https://www.interaction-design.org/literature/topics/visual-hierarchy)
- [Nielsen Norman Group - F-Shaped Pattern](https://www.nngroup.com/articles/f-shaped-pattern-reading-web-content/)
- [Laws of UX](https://lawsofux.com/)
- [Gestalt Principles of Design](https://www.smashingmagazine.com/2014/03/design-principles-visual-perception-and-the-principles-of-gestalt/)
- [Butterick's Practical Typography](https://practicaltypography.com/)
- [Material Design - Typography](https://m3.material.io/styles/typography/overview)
