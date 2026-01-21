# Logo Cloud: Quick Trust Signals

> **Purpose**: Logo clouds provide instant credibility by showing recognizable brands that trust you. They work best immediately after the hero section.

---

## Why Logos Work

- **Instant recognition** — Visitors immediately know who trusts you
- **Borrowed credibility** — Association with known brands elevates you
- **Visual proof** — Harder to fake than text claims
- **Low cognitive load** — Processed faster than text

> "Even if the visitor doesn't recognize all of the companies, it's differentiation. It's visual evidence of legitimacy."
>
> *Source: [Orbit Media](https://www.orbitmedia.com/blog/social-proof-web-design/)*

---

## Logo Cloud Best Practices

### Number of Logos
- **Minimum**: 4-5 logos (fewer looks sparse)
- **Optimal**: 5-8 logos (enough credibility, not overwhelming)
- **Maximum**: 10-12 logos (more can feel cluttered)

### Logo Selection
Choose logos that:
- Your target audience will recognize
- Represent your ideal customer profile
- Have visual brand equity
- You have permission to use

**Priority order**:
1. Biggest/most recognizable names
2. Most relevant to target audience
3. Best logos visually (clean, distinct)

### Label Text

> "For the little text above the logos, consider 'trusted by' rather than 'our clients.' It reminds your visitor that these clients don't just work with you, they trust you."
>
> *Source: [Orbit Media](https://www.orbitmedia.com/blog/social-proof-web-design/)*

**Effective labels**:
- "Trusted by industry leaders"
- "Powering teams at"
- "Used by 10,000+ companies including"
- "Join companies like"
- "As seen in" (for press logos)

**Avoid**:
- "Our clients" (generic, weak)
- No label at all

---

## Visual Styling

### Monochrome Approach

> "Many websites restyle logos so they match the color of the page or the background. This way they blend naturally into the page and don't stick out."
>
> *Source: [Designmodo](https://designmodo.com/social-proof-website/)*

**Monochrome benefits**:
- Cleaner, more professional look
- Logos don't compete with your brand colors
- Consistent visual weight across all logos
- Works on any background

**Implementation**:
```css
.logo-cloud img {
  filter: grayscale(100%);
  opacity: 0.7;
}
.logo-cloud img:hover {
  filter: grayscale(0%);
  opacity: 1;
}
```

### Color vs. Monochrome

| Approach | When to Use |
|----------|-------------|
| **Monochrome** | Clean aesthetic, many logos, brand consistency |
| **Full color** | Few logos, recognizable by color (Google, Slack) |
| **Mix** | Key logos in color, others monochrome |

---

## Layout Patterns

### Horizontal Row
Best for 4-6 logos immediately after hero.

```
Trusted by industry leaders
[Logo] [Logo] [Logo] [Logo] [Logo]
```

### Grid
For more logos or dedicated section.

```
Trusted by 500+ companies
[Logo] [Logo] [Logo] [Logo]
[Logo] [Logo] [Logo] [Logo]
```

### Scrolling/Marquee
For many logos or adding movement.

```
[Logo] [Logo] [Logo] [Logo] →→→
       (auto-scrolling)
```

### Tiered
Separate client logos from press/partner logos.

```
CLIENTS:
[Logo] [Logo] [Logo] [Logo]

AS SEEN IN:
[Forbes] [TechCrunch] [WSJ]
```

---

## Logo Types

### Client/Customer Logos
Companies using your product/service.

**Label ideas**:
- "Trusted by"
- "Powering teams at"
- "Used by"

### Press Mention Logos
Publications that have featured you.

**Label ideas**:
- "As featured in"
- "As seen in"
- "In the press"

### Partner/Integration Logos
Companies you integrate with or partner.

**Label ideas**:
- "Integrates with"
- "Works with"
- "Connects to"

### Certification/Award Logos
Industry recognitions and badges.

**Label ideas**:
- "Recognized by"
- "Certified by"
- "Award-winning"

---

## Placement

### Primary Placement: After Hero
Most common and effective position — provides immediate credibility.

```
[HERO SECTION]

Trusted by 10,000+ companies
[Logo] [Logo] [Logo] [Logo] [Logo]

[REST OF PAGE]
```

### Secondary Placements
- Before pricing section
- Before main CTA
- Footer area
- Sidebar on blog

---

## Adding Context

> "Client logos are a common form of social proof, but they need context to be truly effective. Simply displaying logos can be viewed with scepticism — after all, anyone can add a company logo to their website."
>
> *Source: [Blend B2B](https://www.blendb2b.com/blog/website-social-proof)*

### Ways to Add Context

**Link to case studies**:
```
[Logo clickable → leads to case study]
```

**Add stats**:
```
Trusted by 10,000+ companies
Powering $2B+ in annual transactions
[Logo] [Logo] [Logo] [Logo]
```

**Combined with testimonial**:
```
"[Product] transformed our workflow." — VP at [Logo]
[Logo] [Logo] [Logo] [Logo]
```

---

## Permission & Legal

### Getting Permission
- Include in contract/terms of service
- Request via email with specific usage
- Use logos from their press kit/media page
- Some companies have explicit logo usage guidelines

### Safe Usage
- Don't modify logos beyond size/color treatment
- Don't imply partnership if you're just a customer
- Don't use logos of companies you haven't worked with
- Respect brand guidelines

---

## Mobile Considerations

- Reduce number of logos (4-5 max in view)
- Use horizontal scroll or 2-row grid
- Ensure logos are large enough to recognize
- Consider carousel for many logos

---

## Common Mistakes

### ❌ Too Many Logos
More than 12 looks desperate and clutters the page.

### ❌ Unknown Logos Only
If no one recognizes the brands, there's no borrowed credibility.

### ❌ Mismatched Sizes
Logos should have consistent visual weight.

### ❌ No Label
Without context, logos are just decorative images.

### ❌ Low Quality Images
Pixelated or distorted logos hurt credibility.

### ❌ Using Logos Without Permission
Can lead to legal issues and reputation damage.

---

## Examples

### SaaS Example
```
Trusted by 10,000+ teams worldwide

[Stripe] [Shopify] [Notion] [Figma] [Slack]
```

### Press Example
```
As featured in

[TechCrunch] [Forbes] [WSJ] [Fast Company]
```

### Combined Example
```
Join industry leaders

[Logo] [Logo] [Logo] [Logo] [Logo]

"We've seen 3x ROI since switching" — Sarah, CMO at [Logo]
```

---

## Sources

- [Orbit Media - Social Proof Web Design](https://www.orbitmedia.com/blog/social-proof-web-design/)
- [Designmodo - Adding Social Proof with Client Logos](https://designmodo.com/social-proof-website/)
- [Blend B2B - Website Social Proof](https://www.blendb2b.com/blog/website-social-proof)
- [Davey & Krista - Ways to Incorporate Social Proof](https://daveyandkrista.com/ways-incorporate-social-proof/)
