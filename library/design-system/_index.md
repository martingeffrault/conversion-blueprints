# Design System Library

> **Purpose**: Establish visual foundations for consistent, scalable design
> **Usage**: Reference during design, development, and brand alignment phases
> **Principle**: Constraints enable creativity — systems create consistency at scale

---

## Available Guides

### [M3 Design Tokens](./m3-tokens.md)
**Comprehensive** Material 3-based token architecture. Three-tier system (Reference → System → Component), color schemes with light/dark modes, typography roles, spacing scales, shadows, transitions, DNA system, and industry-specific adjustments.

### [Design Tokens](./design-tokens.md)
The foundation of visual consistency. Covers color systems, typography scales, spacing systems, elevation (shadows), border radius, and breakpoints. Includes naming conventions and token architecture.

### [Spacing & Layout](./spacing-layout.md)
Layout foundations for predictable, harmonious designs. Covers spacing scales, grid systems, container patterns, section rhythms, and responsive spacing strategies.

### [Visual Hierarchy](./visual-hierarchy.md)
Creating clear information priority through design. Covers type hierarchy, size relationships, contrast principles, and visual weight distribution.

### [Dark Mode](./dark-mode.md)
Design inclusive, accessible dark themes. Covers background colors (avoid pure black), text colors (avoid pure white), color desaturation, elevation through surface lightness, CSS implementation, toggle patterns, and accessibility considerations.

---

## Quick Reference

### The 8-Point Grid

> "Using a consistent spacing scale based on 8px multiples creates visual harmony and faster development."
>
> *— Google Material Design*

Base unit: 8px. Scale: 4, 8, 12, 16, 24, 32, 48, 64, 96, 128...

### Design Token Hierarchy

```
Global Tokens (primitives)
    ↓
Semantic Tokens (purpose-driven)
    ↓
Component Tokens (scoped to components)
```

### Golden Ratio in Design

1.618 — Use for proportional relationships between elements.

---

## Cross-References

- **Typography patterns**: See [Visual Hierarchy](./visual-hierarchy.md)
- **Component styling**: See [Components Library](../components/_index.md)
- **Accessibility requirements**: See [Accessibility](../accessibility/_index.md)

---

## Sources

All guides based on standards from:
- Google Material Design 3
- Apple Human Interface Guidelines
- Tailwind CSS Design System
- Nathan Curtis (EightShapes)
- Brad Frost (Atomic Design)
