# Dark Mode Design Guidelines

> **Purpose**: Design inclusive, accessible dark themes that reduce eye strain and provide user choice.
> **Key principle**: Dark mode is not just inverted colors—it requires thoughtful redesign.
> **Accessibility note**: Dark mode helps some users but not all; always let users choose.

---

## When to Use Dark Mode

### Good Candidates

| Use Case | Why Dark Mode Works |
|----------|---------------------|
| Media/entertainment | Immersive viewing experience |
| Data visualization | Colors pop against dark backgrounds |
| Developer tools | Long coding sessions, reduces eye strain |
| Minimalist content | Sleek, modern aesthetic |
| Night/low-light usage | Reduces screen brightness |
| OLED displays | True blacks save battery |

### Poor Candidates

| Use Case | Why Dark Mode Struggles |
|----------|------------------------|
| Long-form text | Harder to read for many users |
| Complex B2B dashboards | Too much varied content |
| Detailed forms | Input fields need clear visibility |
| Print-oriented content | Paper metaphor doesn't translate |
| Accessibility-critical | Some users can't use dark mode |

> "Dark mode can make it better for some users, but not all of them."
>
> *Source: [Stéphanie Walter](https://stephaniewalter.design/blog/dark-mode-accessibility-myth-debunked/)*

---

## Background Colors

### Never Use Pure Black

> "One of the first rules of dark mode is to use dark grey (#121212) in place of true black (#000000) as the primary background color. Dark grey surfaces make it easier to express elevation and depth."
>
> *Source: [Material Design](https://m2.material.io/design/color/dark-theme.html)*

| Color | Usage | Example |
|-------|-------|---------|
| Pure black `#000000` | ❌ Avoid | Too harsh, hard to show shadows |
| Dark grey `#121212` | ✅ Recommended | Material Design standard |
| Dark blue-grey `#0d1117` | ✅ Good | GitHub's dark mode |
| Elevated grey `#1e1e1e` | ✅ Cards/surfaces | VS Code's dark theme |

### Surface Elevation System

```
┌─────────────────────────────────────────────────────────────────┐
│  ELEVATION LEVELS (Material Design)                             │
│                                                                 │
│  Level 0 (Background)    #121212    0% overlay                 │
│  Level 1 (Cards)         #1e1e1e    5% white overlay           │
│  Level 2 (Raised)        #232323    7% white overlay           │
│  Level 3 (Dialogs)       #252525    8% white overlay           │
│  Level 4 (Menus)         #272727    9% white overlay           │
│  Level 8 (Popups)        #2d2d2d    12% white overlay          │
│                                                                 │
│  Higher elevation = lighter surface = more prominent            │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Practical Palette Example

```css
/* Dark mode surface palette */
--bg-base: #0f0f0f;       /* Page background */
--bg-surface: #171717;    /* Cards, panels */
--bg-elevated: #1f1f1f;   /* Modals, dropdowns */
--bg-hover: #262626;      /* Hover states */
--bg-active: #2e2e2e;     /* Active/pressed states */
```

---

## Text Colors

### Don't Use Pure White

> "Just as pure black isn't ideal for a dark theme, bright white can glow too much in a dark UI, creating a jarring effect. Use a slightly darker shade of white."
>
> *Source: [Toptal](https://www.toptal.com/designers/ui/dark-ui-design)*

| Color | Contrast | Usage |
|-------|----------|-------|
| Pure white `#ffffff` | 21:1 | ❌ Too bright, causes glow |
| Off-white `#e4e4e7` | ~16:1 | ✅ Primary text |
| Light grey `#a1a1aa` | ~7:1 | ✅ Secondary text |
| Dark grey `#71717a` | ~4.5:1 | ✅ Muted text (meets WCAG) |

### Text Hierarchy

```css
/* Dark mode text colors */
--text-primary: #e4e4e7;      /* Headings, important text */
--text-secondary: #a1a1aa;    /* Body text */
--text-muted: #71717a;        /* Captions, hints */
--text-disabled: #52525b;     /* Disabled states */
```

---

## Color Saturation

### Desaturate Colors for Dark Backgrounds

> "Saturated colors create optical vibrations when on a dark background, causing eye strain. In general, your colors should have around 20 points lower saturation on dark mode than on light mode."
>
> *Source: [Atmos](https://atmos.style/blog/dark-mode-ui-best-practices)*

| Light Mode | Dark Mode | Adjustment |
|------------|-----------|------------|
| `hsl(220, 90%, 50%)` | `hsl(220, 70%, 60%)` | -20 sat, +10 light |
| `hsl(150, 85%, 45%)` | `hsl(150, 65%, 55%)` | -20 sat, +10 light |
| `hsl(0, 95%, 50%)` | `hsl(0, 75%, 60%)` | -20 sat, +10 light |

### Tonal Palette Selection

> "In light theme, illustrations may use a tonal value of 800. In dark theme, use a less saturated color—a tonal value of 200, 300, or 400 is recommended."
>
> *Source: [Material Design](https://m2.material.io/design/color/dark-theme.html)*

```
Light Mode                    Dark Mode
┌──────────────────────┐     ┌──────────────────────┐
│  Primary-800         │     │  Primary-300         │
│  Saturated           │ →   │  Desaturated         │
│  Darker              │     │  Lighter             │
└──────────────────────┘     └──────────────────────┘
```

---

## Contrast Requirements

### WCAG Compliance

| Element | Minimum Contrast | Target |
|---------|------------------|--------|
| Normal text | 4.5:1 | 7:1+ |
| Large text (18px+) | 3:1 | 4.5:1+ |
| UI components | 3:1 | 4.5:1+ |
| Icons/graphics | 3:1 | 4.5:1+ |

> "Dark surfaces paired with 100% white text should maintain a contrast ratio of at least 15.8:1 because elevated surfaces in dark mode become lighter."
>
> *Source: [Material Design](https://m2.material.io/design/color/dark-theme.html)*

### Testing Tools

| Tool | Use Case |
|------|----------|
| [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/) | Individual color pairs |
| [Stark](https://www.getstark.co/) | Figma/Sketch plugin |
| Chrome DevTools | In-browser testing |
| [Colour Contrast Analyser](https://www.tpgi.com/color-contrast-checker/) | Desktop app |

---

## Implementation

### CSS Custom Properties Approach

```css
/* Define color tokens */
:root {
  /* Light mode (default) */
  --bg-base: #ffffff;
  --bg-surface: #f4f4f5;
  --text-primary: #18181b;
  --text-secondary: #52525b;
  --accent: hsl(220, 90%, 50%);
}

/* Dark mode override */
@media (prefers-color-scheme: dark) {
  :root {
    --bg-base: #0f0f0f;
    --bg-surface: #171717;
    --text-primary: #e4e4e7;
    --text-secondary: #a1a1aa;
    --accent: hsl(220, 70%, 60%);
  }
}
```

### Manual Toggle Support

```css
/* System preference (default) */
:root {
  color-scheme: light dark;
}

/* Manual light mode */
[data-theme="light"] {
  --bg-base: #ffffff;
  /* ... light colors */
}

/* Manual dark mode */
[data-theme="dark"] {
  --bg-base: #0f0f0f;
  /* ... dark colors */
}
```

### JavaScript Theme Toggle

```javascript
// Preference cascade: localStorage > system > default
function getPreferredTheme() {
  const stored = localStorage.getItem('theme');
  if (stored) return stored;

  return window.matchMedia('(prefers-color-scheme: dark)').matches
    ? 'dark'
    : 'light';
}

// Apply theme immediately (in <head> to prevent flash)
document.documentElement.setAttribute('data-theme', getPreferredTheme());

// Toggle function
function toggleTheme() {
  const current = document.documentElement.getAttribute('data-theme');
  const next = current === 'dark' ? 'light' : 'dark';

  document.documentElement.setAttribute('data-theme', next);
  localStorage.setItem('theme', next);
}
```

> "To ensure that this code executes before rendering the page, put it in the `<head>` tag of your page."
>
> *Source: [web.dev](https://web.dev/articles/prefers-color-scheme)*

### Preventing Flash of Wrong Theme

```html
<!-- In <head>, BEFORE stylesheets -->
<script>
  (function() {
    const theme = localStorage.getItem('theme') ||
      (window.matchMedia('(prefers-color-scheme: dark)').matches ? 'dark' : 'light');
    document.documentElement.setAttribute('data-theme', theme);
  })();
</script>
```

---

## UI Component Adjustments

### Shadows in Dark Mode

| Light Mode | Dark Mode |
|------------|-----------|
| `box-shadow: 0 4px 6px rgba(0,0,0,0.1)` | `box-shadow: 0 4px 6px rgba(0,0,0,0.5)` |
| Soft, subtle shadows | Deeper, more pronounced |
| Black shadow color | Black or darker background |

**Alternative**: Use elevation through surface lightness instead of shadows.

### Borders

| Light Mode | Dark Mode |
|------------|-----------|
| `border: 1px solid #e4e4e7` | `border: 1px solid #2e2e2e` |
| Darker than background | Lighter than background |
| Subtle definition | Subtle definition |

### Images and Media

| Content | Adjustment |
|---------|------------|
| Photos | Generally fine, no change needed |
| Illustrations | May need lighter/desaturated variants |
| Icons | Ensure contrast, may need color swap |
| Logos | May need light variant |
| Screenshots | Consider dimming or borders |

```css
/* Dim images in dark mode (optional) */
[data-theme="dark"] img {
  filter: brightness(0.9);
}

/* Except hero images */
[data-theme="dark"] .hero img {
  filter: none;
}
```

---

## Accessibility Considerations

### Users Who Struggle with Dark Mode

> "Some users, especially those with astigmatism or certain visual impairments, may find it harder to read white text against a dark background. This contrast can cause blurred vision or visual distortions."
>
> *Source: [Smashing Magazine](https://www.smashingmagazine.com/2025/04/inclusive-dark-mode-designing-accessible-dark-themes/)*

| Condition | Issue with Dark Mode |
|-----------|---------------------|
| Astigmatism | Text appears to glow/blur |
| Dyslexia | Some prefer light backgrounds |
| Low vision | May need specific contrast |
| Light sensitivity | Actually benefits from dark mode |
| Migraine sufferers | Often prefer dark mode |

### Best Practice: Always Offer Choice

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Theme Preference                                               │
│                                                                 │
│  ○ Light                                                        │
│  ○ Dark                                                         │
│  ● System (follows your device settings)                       │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Anti-aliasing Issues

> "In dark mode, anti-aliasing has the problem of halo effects, where the edges of text appear blurred or overly luminous."
>
> *Source: [UX Design Institute](https://www.uxdesigninstitute.com/blog/dark-mode-design-practical-guide/)*

**Solutions:**
- Use medium font weights (400-500) instead of thin (300)
- Avoid very small text sizes
- Test rendering across browsers/OS

---

## Toggle Design Patterns

### Basic Toggle

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [☀️]─────●[🌙]                                                  │
│                                                                 │
│  Simple toggle with sun/moon icons                              │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Three-Way Selector

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Light] [Dark] [●System]                                      │
│                                                                 │
│  Explicit control with system default                          │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Icon Button

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Header:   Logo    Nav    Nav    [🌙]   User                   │
│                                                                 │
│  Click to toggle, icon changes to show current state            │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Placement

| Location | Pros | Cons |
|----------|------|------|
| Header | Always visible | Takes header space |
| Settings | Clean header | Hidden, extra clicks |
| Footer | Unobtrusive | Easy to miss |
| Floating button | Always accessible | Can obscure content |

---

## Color Palette Examples

### Neutral (Recommended Starting Point)

```
Light Mode                    Dark Mode
Background:   #ffffff   →    #0f0f0f
Surface:      #f4f4f5   →    #171717
Elevated:     #e4e4e7   →    #262626
Border:       #d4d4d8   →    #3f3f46
Text:         #18181b   →    #e4e4e7
Muted:        #71717a   →    #a1a1aa
```

### GitHub-Style (Blue Undertone)

```
Light Mode                    Dark Mode
Background:   #ffffff   →    #0d1117
Surface:      #f6f8fa   →    #161b22
Elevated:     #ffffff   →    #21262d
Border:       #d0d7de   →    #30363d
Text:         #24292f   →    #c9d1d9
Muted:        #57606a   →    #8b949e
```

### Discord-Style (Blurple Accent)

```
Light Mode                    Dark Mode
Background:   #ffffff   →    #313338
Surface:      #f2f3f5   →    #2b2d31
Elevated:     #ffffff   →    #1e1f22
Accent:       #5865f2   →    #5865f2  (same)
Text:         #060607   →    #f2f3f5
Muted:        #4e5058   →    #b5bac1
```

---

## Testing Checklist

### Visual Testing

- [ ] All text meets WCAG contrast requirements
- [ ] UI components have 3:1+ contrast
- [ ] No pure black backgrounds
- [ ] No pure white text
- [ ] Colors are appropriately desaturated
- [ ] Elevation is visible through surface lightness
- [ ] Images/media display appropriately

### Functional Testing

- [ ] Toggle works correctly
- [ ] System preference is respected
- [ ] User preference persists (localStorage)
- [ ] No flash of wrong theme on page load
- [ ] Transitions are smooth (no jarring changes)
- [ ] Works across all pages/routes

### Accessibility Testing

- [ ] Screen reader announces theme changes
- [ ] Toggle is keyboard accessible
- [ ] Focus states are visible in both modes
- [ ] Tested with color blindness simulators
- [ ] System preference option available

---

## Common Mistakes

| Mistake | Problem | Solution |
|---------|---------|----------|
| Pure black background | Harsh, hard to read | Use #121212 or similar |
| Pure white text | Glow effect, strain | Use #e4e4e7 or similar |
| Same saturation | Eye strain, vibration | Reduce saturation 20% |
| No elevation | Flat, no hierarchy | Use surface lightness |
| Forced dark mode | Accessibility issue | Always provide toggle |
| Slow theme detection | Flash of wrong theme | Inline script in `<head>` |
| Ignoring images | Logos disappear | Provide light/dark variants |

---

## Sources

- [Material Design - Dark Theme](https://m2.material.io/design/color/dark-theme.html)
- [web.dev - prefers-color-scheme](https://web.dev/articles/prefers-color-scheme)
- [Smashing Magazine - Inclusive Dark Mode](https://www.smashingmagazine.com/2025/04/inclusive-dark-mode-designing-accessible-dark-themes/)
- [UX Design Institute - Dark Mode Practical Guide](https://www.uxdesigninstitute.com/blog/dark-mode-design-practical-guide/)
- [Stéphanie Walter - Dark Mode Accessibility Myth](https://stephaniewalter.design/blog/dark-mode-accessibility-myth-debunked/)
- [Toptal - Dark UI Design](https://www.toptal.com/designers/ui/dark-ui-design)
- [Atmos - Dark Mode Best Practices](https://atmos.style/blog/dark-mode-ui-best-practices)
- [Design Studio UX - Dark Mode Principles](https://www.designstudiouiux.com/blog/dark-mode-ui-design-best-practices/)
- [MDN - prefers-color-scheme](https://developer.mozilla.org/en-US/docs/Web/CSS/Reference/At-rules/@media/prefers-color-scheme)
- [Ryan Feigenbaum - Dark Mode Toggle](https://ryanfeigenbaum.com/dark-mode/)
