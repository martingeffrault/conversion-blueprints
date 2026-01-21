# WCAG Guidelines Implementation

> **Purpose**: Implement Web Content Accessibility Guidelines for inclusive websites
> **Standard**: WCAG 2.1 AA (industry standard minimum)
> **Principle**: Design for everyone — accessibility benefits all users

---

## Understanding WCAG

### What Is WCAG?

> "Web Content Accessibility Guidelines (WCAG) is developed through the W3C process in cooperation with individuals and organizations around the world, with a goal of providing a single shared standard for web content accessibility."
>
> *Source: [W3C WAI](https://www.w3.org/WAI/standards-guidelines/wcag/)*

### Conformance Levels

| Level | Description | Requirement |
|-------|-------------|-------------|
| **A** | Minimum | Basic accessibility |
| **AA** | Mid-range | Industry standard, legally required |
| **AAA** | Highest | Enhanced, not always feasible |

**Target: WCAG 2.1 AA** — This is the legal standard in most jurisdictions.

---

## The POUR Principles

### Perceivable

*Users must be able to perceive the information being presented.*

### Operable

*Users must be able to operate the interface.*

### Understandable

*Users must be able to understand the information and operation.*

### Robust

*Content must be robust enough to work with current and future technologies.*

---

## Perceivable (Principle 1)

### 1.1 Text Alternatives

**Requirement**: Provide text alternatives for non-text content.

| Content Type | Text Alternative |
|--------------|------------------|
| Informative images | Descriptive alt text |
| Decorative images | Empty alt (`alt=""`) |
| Complex images | Long description |
| Form inputs | Labels |
| Audio/Video | Transcripts, captions |
| Icons with meaning | Alt text or aria-label |

**Alt Text Best Practices**:

| Good | Bad |
|------|-----|
| "Woman working on laptop in coffee shop" | "Image" |
| "Chart showing 50% growth in Q3" | "Chart" |
| "" (for decorative) | "Blue decorative line" |
| "Submit form" (for icon button) | No alt at all |

**Pattern**:
```html
<!-- Informative image -->
<img src="team.jpg" alt="Our team of 12 developers in the NYC office">

<!-- Decorative image -->
<img src="divider.svg" alt="" role="presentation">

<!-- Complex image -->
<figure>
  <img src="chart.png" alt="Revenue chart showing 50% growth">
  <figcaption>Q3 2024 revenue increased 50% year-over-year...</figcaption>
</figure>

<!-- Icon button -->
<button aria-label="Close dialog">
  <svg>...</svg>
</button>
```

### 1.2 Time-Based Media

**Requirement**: Provide alternatives for audio and video.

| Media Type | Requirements |
|------------|--------------|
| Pre-recorded audio | Transcript |
| Pre-recorded video | Captions + audio description |
| Live audio | Captions |
| Live video | Captions |

**Captions vs Subtitles**:
- **Captions**: Include all audio (speech, sound effects, music cues)
- **Subtitles**: Speech only, for language translation

### 1.3 Adaptable

**Requirement**: Content can be presented in different ways without losing meaning.

**Semantic HTML**:
```html
<!-- Use proper heading hierarchy -->
<h1>Page Title</h1>
  <h2>Section</h2>
    <h3>Subsection</h3>

<!-- Use lists for lists -->
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
</ul>

<!-- Use tables for tabular data -->
<table>
  <caption>Monthly sales</caption>
  <thead><tr><th scope="col">Month</th>...</tr></thead>
  <tbody>...</tbody>
</table>

<!-- Use landmarks -->
<header>...</header>
<nav>...</nav>
<main>...</main>
<aside>...</aside>
<footer>...</footer>
```

**Form Structure**:
```html
<form>
  <fieldset>
    <legend>Shipping Address</legend>

    <label for="street">Street</label>
    <input type="text" id="street" name="street">

    <label for="city">City</label>
    <input type="text" id="city" name="city">
  </fieldset>
</form>
```

### 1.4 Distinguishable

**Requirement**: Make content easy to see and hear.

**Color Contrast Requirements**:

| Text Type | Minimum Contrast |
|-----------|------------------|
| Normal text (<18px) | 4.5:1 |
| Large text (18px+ bold, 24px+ regular) | 3:1 |
| UI components | 3:1 |
| Graphical objects | 3:1 |

**Don't Rely on Color Alone**:

| Bad | Good |
|-----|------|
| "Required fields in red" | "Required fields marked with *" |
| Red/green for error/success | Icon + color + text |
| Links only differentiated by color | Links underlined or bold + color |

**Text Sizing**:
- Base font: 16px minimum
- Text resizable to 200% without loss of content
- Line height: 1.5 minimum for body text
- Paragraph spacing: 2x font size
- Letter spacing adjustable

**Pattern**:
```css
body {
  font-size: 16px;
  line-height: 1.5;
}

p {
  margin-bottom: 1.5em; /* 2x line spacing minimum */
}

/* Allow text resizing */
html {
  font-size: 100%; /* Respect user preferences */
}
```

---

## Operable (Principle 2)

### 2.1 Keyboard Accessible

**Requirement**: All functionality available via keyboard.

**Keyboard Navigation**:

| Key | Action |
|-----|--------|
| Tab | Move to next focusable element |
| Shift + Tab | Move to previous element |
| Enter | Activate links, buttons |
| Space | Activate buttons, checkboxes |
| Arrow keys | Navigate within components |
| Escape | Close dialogs, cancel |

**Focus Order**:
```html
<!-- Natural tab order follows DOM order -->
<nav>
  <a href="/">Home</a>
  <a href="/about">About</a>
  <a href="/contact">Contact</a>
</nav>

<!-- Use tabindex="0" to make non-interactive elements focusable -->
<div tabindex="0" role="button" onclick="...">Custom Button</div>

<!-- Never use positive tabindex (disrupts natural order) -->
<!-- BAD: <input tabindex="3"> -->
```

**Focus Trap for Modals**:
```javascript
// When modal opens, focus first focusable element
// Tab should cycle within modal
// Escape closes modal
// Focus returns to trigger element on close
```

### 2.2 Enough Time

**Requirement**: Users have enough time to read and use content.

**Time Limits**:
- Allow users to turn off, adjust, or extend time limits
- Auto-updating content can be paused
- No content that requires timing (unless essential)

**Session Timeouts**:
- Warn users before timeout (e.g., 20 minutes before)
- Allow extension
- Save progress

### 2.3 Seizures and Physical Reactions

**Requirement**: Don't design content that causes seizures.

| Rule | Limit |
|------|-------|
| Flashing content | < 3 flashes per second |
| Red flash | Especially dangerous |
| Animation | Provide pause/disable option |

**Pattern**:
```css
/* Respect user motion preferences */
@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    animation-duration: 0.01ms !important;
    transition-duration: 0.01ms !important;
  }
}
```

### 2.4 Navigable

**Requirement**: Help users navigate and find content.

**Skip Links**:
```html
<body>
  <a href="#main" class="skip-link">Skip to main content</a>
  <header>...</header>
  <nav>...</nav>
  <main id="main">...</main>
</body>

<style>
.skip-link {
  position: absolute;
  left: -9999px;
}
.skip-link:focus {
  left: 0;
  z-index: 9999;
  background: #000;
  color: #fff;
  padding: 8px 16px;
}
</style>
```

**Page Titles**:
```html
<!-- Descriptive, unique titles -->
<title>Contact Us - Company Name</title>
<title>About Our Team - Company Name</title>
```

**Heading Hierarchy**:
- Only one `<h1>` per page
- Don't skip levels (h1 → h3)
- Headings describe content below them

**Focus Visible**:
```css
/* Never remove outlines without replacement */
:focus {
  outline: 2px solid #005fcc;
  outline-offset: 2px;
}

/* Enhanced focus for keyboard users */
:focus-visible {
  outline: 3px solid #005fcc;
  outline-offset: 2px;
}

/* Remove for mouse users (optional) */
:focus:not(:focus-visible) {
  outline: none;
}
```

### 2.5 Input Modalities

**Requirement**: Support various input methods.

**Touch Targets**:
```css
/* Minimum 44x44px touch targets */
button, a, input[type="checkbox"], input[type="radio"] {
  min-width: 44px;
  min-height: 44px;
}
```

**Pointer Cancellation**:
- Allow cancellation of pointer actions (e.g., drag off to cancel)
- Use `onclick`, not `onmousedown`

**Motion Actuation**:
- Don't require device motion (shake, tilt) for functionality
- Provide button alternatives

---

## Understandable (Principle 3)

### 3.1 Readable

**Requirement**: Text content is readable and understandable.

**Language Declaration**:
```html
<html lang="en">

<!-- For multilingual content -->
<p>The French word for hello is <span lang="fr">bonjour</span>.</p>
```

**Reading Level**:
- Write at 8th-grade level when possible
- Provide simpler summaries for complex content
- Define jargon and abbreviations

```html
<!-- Define abbreviations -->
<abbr title="Web Content Accessibility Guidelines">WCAG</abbr>

<!-- Or provide glossary link -->
<a href="/glossary#wcag">WCAG</a>
```

### 3.2 Predictable

**Requirement**: Pages operate in predictable ways.

**Consistent Navigation**:
- Navigation appears in same location on every page
- Links in same relative order
- Same terminology throughout

**No Unexpected Changes**:
```html
<!-- BAD: Auto-submit on selection -->
<select onchange="this.form.submit()">

<!-- GOOD: Explicit submit -->
<select name="country">...</select>
<button type="submit">Apply Filter</button>
```

### 3.3 Input Assistance

**Requirement**: Help users avoid and correct mistakes.

**Error Identification**:
```html
<label for="email">Email *</label>
<input
  type="email"
  id="email"
  aria-describedby="email-error"
  aria-invalid="true"
>
<p id="email-error" class="error">
  Please enter a valid email address (e.g., name@example.com)
</p>
```

**Labels and Instructions**:
```html
<label for="phone">Phone Number</label>
<input
  type="tel"
  id="phone"
  aria-describedby="phone-hint"
>
<p id="phone-hint" class="hint">Format: (123) 456-7890</p>
```

**Error Prevention**:
- Confirm before destructive actions
- Allow undo
- Review before final submission

---

## Robust (Principle 4)

### 4.1 Compatible

**Requirement**: Maximize compatibility with current and future technologies.

**Valid HTML**:
- Use valid HTML5
- Close all tags
- Unique IDs
- Proper nesting

**ARIA Usage**:
```html
<!-- First rule: Don't use ARIA if native HTML works -->
<!-- BAD -->
<div role="button" tabindex="0">Click me</div>

<!-- GOOD -->
<button>Click me</button>

<!-- ARIA for enhanced components -->
<button aria-expanded="false" aria-controls="menu">
  Menu
</button>
<ul id="menu" hidden>...</ul>
```

**Status Messages**:
```html
<!-- Announce dynamic content to screen readers -->
<div role="status" aria-live="polite">
  Your message has been sent.
</div>

<div role="alert" aria-live="assertive">
  Error: Payment failed.
</div>
```

---

## Common ARIA Patterns

### Expandable Sections

```html
<button
  aria-expanded="false"
  aria-controls="section1"
  onclick="toggleSection(this)"
>
  Section Title
</button>
<div id="section1" hidden>
  Section content...
</div>
```

### Tabs

```html
<div role="tablist">
  <button role="tab" aria-selected="true" aria-controls="panel1" id="tab1">
    Tab 1
  </button>
  <button role="tab" aria-selected="false" aria-controls="panel2" id="tab2">
    Tab 2
  </button>
</div>

<div role="tabpanel" id="panel1" aria-labelledby="tab1">
  Panel 1 content
</div>
<div role="tabpanel" id="panel2" aria-labelledby="tab2" hidden>
  Panel 2 content
</div>
```

### Modal Dialog

```html
<div role="dialog" aria-modal="true" aria-labelledby="dialog-title">
  <h2 id="dialog-title">Confirm Action</h2>
  <p>Are you sure you want to delete this item?</p>
  <button>Cancel</button>
  <button>Delete</button>
</div>
```

### Navigation Landmark

```html
<nav aria-label="Main navigation">
  <ul>
    <li><a href="/">Home</a></li>
    <li><a href="/about">About</a></li>
  </ul>
</nav>

<nav aria-label="Footer navigation">
  <ul>...</ul>
</nav>
```

---

## WCAG 2.1 AA Checklist

### Perceivable

- [ ] All images have appropriate alt text
- [ ] Video has captions
- [ ] Audio has transcripts
- [ ] Color contrast meets 4.5:1 for text
- [ ] Color alone doesn't convey information
- [ ] Text can resize to 200% without loss
- [ ] Content reflows at 320px width

### Operable

- [ ] All functionality works via keyboard
- [ ] Focus order is logical
- [ ] Focus indicator is visible
- [ ] No keyboard traps
- [ ] Skip link provided
- [ ] Page titles are descriptive
- [ ] Link text is descriptive
- [ ] Touch targets are 44x44px minimum
- [ ] No content flashes more than 3x/second

### Understandable

- [ ] Page language is declared
- [ ] Navigation is consistent
- [ ] Form labels are present
- [ ] Error messages are clear
- [ ] Instructions are provided where needed

### Robust

- [ ] HTML is valid
- [ ] ARIA is used correctly
- [ ] Status messages use live regions
- [ ] Works across browsers/assistive tech

---

## Sources

- [W3C Web Content Accessibility Guidelines 2.1](https://www.w3.org/TR/WCAG21/)
- [WebAIM WCAG 2 Checklist](https://webaim.org/standards/wcag/checklist)
- [MDN Accessibility](https://developer.mozilla.org/en-US/docs/Web/Accessibility)
- [Deque University](https://dequeuniversity.com/)
- [A11y Project Checklist](https://www.a11yproject.com/checklist/)
- [Inclusive Components](https://inclusive-components.design/)
