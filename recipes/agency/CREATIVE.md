# Creative / Design Agency Recipe

> **Variant Focus**: Visual design, branding, creative work
> **Examples**: Pentagram, Sagmeister & Walsh, Collins, Mucho, Porto Rocha
> **Key Differentiator**: Portfolio-first, visual storytelling, design craft
> **Revenue Model**: Project-based, retainers for brand work
> **Target Clients**: Companies seeking brand identity, visual systems, creative direction

---

## How This Differs from Generic Agency

| Aspect | Generic Agency | Creative Agency |
|--------|----------------|-----------------|
| Homepage hero | Text + work preview | Full-screen visual/project |
| Navigation | Standard menu | Minimal, design-forward |
| Portfolio | Grid with filters | Curated, editorial |
| Content | Blog posts | Process essays, design thinking |
| Case studies | Results-focused | Process + craft-focused |
| Team page | Headshots | Creative portraits, personality |

---

## Site Architecture

### Core Pages

```
/                       Homepage (immersive, visual-first)
├── /work/              Portfolio (curated, no filters)
│   └── /work/[project]/ Case studies (visual essays)
├── /studio/            About, team, culture (not "about")
├── /services/          What we do (may be minimal)
├── /contact/           Start a project
└── /journal/           Process, thoughts (optional)
```

### Design Agency Navigation Philosophy

> "Award-winning design agency sites like Collins and Pentagram often use minimal navigation that gets out of the way of the work. The work is the hero."
>
> *Pattern from: [Awwwards Agency Collections](https://www.awwwards.com/awwwards/collections/agency-portfolios/)*

**Minimal Nav Pattern**:
```
[Logo]                               Work    Studio    Contact
```

**Hidden Nav Pattern** (more experimental):
```
[Logo]                                              [Menu ☰]

                  [Full-screen project]
```

---

## Homepage: Visual-First

### Pattern 1: Full-Screen Project Carousel

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│         [Full-screen hero image/video - Current project]        │
│                                                                 │
│                                                                 │
│                                                                 │
│                                                                 │
│                         Project Title                           │
│                     Client — Branding                           │
│                                                                 │
│                      [View Project]                             │
│                                                                 │
│  [○] [●] [○] [○] [○]                                           │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Pattern 2: Showreel Hero

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│              [Autoplay video reel of best work]                 │
│                                                                 │
│                                                                 │
│                                                                 │
│                      [STUDIO NAME]                              │
│                      Brand & Digital                            │
│                                                                 │
│              [▶ Play Reel]    [See Work]                       │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Pattern 3: Work Grid Hero (Editorial)

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  ┌───────────────────────────┐  ┌───────────────────────────┐  │
│  │                           │  │                           │  │
│  │   [Large Project 1]       │  │   [Project 2]             │  │
│  │                           │  │                           │  │
│  │   Client — Type           │  ├───────────────────────────┤  │
│  │                           │  │   [Project 3]             │  │
│  └───────────────────────────┘  └───────────────────────────┘  │
│                                                                 │
│  ┌────────────────┐  ┌────────────────┐  ┌────────────────┐    │
│  │ [Project 4]    │  │ [Project 5]    │  │ [Project 6]    │    │
│  └────────────────┘  └────────────────┘  └────────────────┘    │
│                                                                 │
│                         [See All Work]                          │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Portfolio / Work Page

### Curation Over Quantity

> "A portfolio is a curated collection, not a complete archive. Show your best work, not all your work."
>
> *Design principle from: [AIGA - Portfolio Best Practices](https://www.aiga.org/resources/portfolio-best-practices)*

**Recommendations**:
- 8-15 projects maximum
- Best work only (no filler)
- Variety of project types
- Recent work prioritized
- No filtering (curated order matters)

### Layout: Editorial Grid

Unlike marketing agencies, creative agencies often use asymmetric, editorial layouts:

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Selected Work                                                  │
│                                                                 │
│  ┌─────────────────────────────────────────┐  ┌──────────────┐ │
│  │                                         │  │              │ │
│  │    [Large featured project]             │  │  [Project 2] │ │
│  │                                         │  │              │ │
│  │    Client                               │  │  Client      │ │
│  │    Branding                             │  │  Digital     │ │
│  │                                         │  │              │ │
│  └─────────────────────────────────────────┘  └──────────────┘ │
│                                                                 │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────────────┐  │
│  │              │  │              │  │                      │  │
│  │  [Project 3] │  │  [Project 4] │  │  [Project 5]         │  │
│  │              │  │              │  │                      │  │
│  └──────────────┘  └──────────────┘  └──────────────────────┘  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Case Study: Visual Essay Format

### Creative Case Study Structure

Unlike results-focused case studies, creative case studies are visual essays about the work:

```
1. Hero
   └── Full-bleed project imagery, project title, client, year

2. The Brief
   └── What the client needed (1-2 paragraphs max)

3. The Work (primary focus)
   └── Large, beautiful imagery with minimal captions
   └── Show the craft, details, system

4. Process (optional)
   └── Sketches, explorations, iterations

5. In Context
   └── Applications, real-world usage

6. Credits
   └── Team members, roles

7. Next Project
   └── Link to next case study
```

### Visual Essay Layout

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│         [Full-bleed hero image - the main visual]               │
│                                                                 │
│                                                                 │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Project Title                                                  │
│  Client Name — Year                                             │
│                                                                 │
│  Brief description of what we created. One paragraph.           │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│         [Full-bleed work image]                                 │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│         [Full-bleed work image]                                 │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌──────────────────────────┐  ┌──────────────────────────┐    │
│  │ [Detail image]           │  │ [Detail image]           │    │
│  └──────────────────────────┘  └──────────────────────────┘    │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│         [Full-bleed application shot]                           │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Credits:                                                       │
│  Creative Direction: Name    Design: Name, Name                 │
│  Photography: Name           Client Team: Names                 │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Next Project                                                   │
│  [Large preview of next project] →                              │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Studio Page (About)

### Creative Agency About

Less corporate, more personality:

```
1. Hero
   └── Philosophy/manifesto, team photo or illustration

2. What We Do
   └── Brief, poetic description of services

3. Team
   └── Creative portraits, titles, personality

4. Clients
   └── Logo cloud (selective, relevant)

5. Recognition (optional)
   └── Awards, press

6. Culture/Values
   └── How we work, beliefs

7. Careers
   └── Join us (if hiring)
```

### Team Section Style

Creative agencies show personality:

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  The Team                                                       │
│                                                                 │
│  ┌───────────────┐  ┌───────────────┐  ┌───────────────┐       │
│  │               │  │               │  │               │       │
│  │  [Creative    │  │  [Creative    │  │  [Creative    │       │
│  │   portrait]   │  │   portrait]   │  │   portrait]   │       │
│  │               │  │               │  │               │       │
│  │  Name         │  │  Name         │  │  Name         │       │
│  │  "The one who │  │  "Makes       │  │  "Obsessed    │       │
│  │   draws"      │  │   things move"│  │   with type"  │       │
│  └───────────────┘  └───────────────┘  └───────────────┘       │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Services (Minimal Approach)

Creative agencies often keep services minimal to avoid commoditization:

**Anti-Pattern (Avoid)**:
- Detailed pricing
- Package tiers
- Feature checklists

**Better Approach**:

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  What We Do                                                     │
│                                                                 │
│  We design brand identities, digital experiences,               │
│  and creative campaigns for companies who want to               │
│  stand out.                                                     │
│                                                                 │
│  ──────────────────────────────────────────────────────────     │
│                                                                 │
│  Brand Identity         Digital Products         Campaigns      │
│                                                                 │
│  [Start a Conversation]                                         │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Visual Design Principles

### Typography

- Large, confident type
- High-quality typefaces (no system fonts)
- Generous white space
- Minimal text, maximum impact

### Imagery

- Full-bleed images
- High resolution, high quality
- No stock photos
- Project imagery as hero

### Interaction

- Subtle, refined animations
- Smooth scroll
- Hover states that reveal craft
- Performance-conscious

---

## SEO Considerations

### Limited SEO Focus

Creative agencies typically:
- Rely on referrals and reputation
- Rank for brand name searches
- Don't compete on "branding agency" keywords

**Do optimize for**:
- Brand name searches
- "[Studio name] portfolio"
- "[Studio name] work"

**Don't over-optimize for**:
- "best branding agency" (rarely how clients find design studios)
- Generic service keywords

### Content for Authority

Instead of SEO content, create:
- Process posts (Medium, own journal)
- Speaking at design conferences
- Design publications (Eye, AIGA Eye on Design)
- Award submissions (for backlinks and credibility)

---

## Implementation Checklist

### Visual Foundation
- [ ] High-quality project photography
- [ ] Custom typography (licensed fonts)
- [ ] Animation/interaction design
- [ ] Mobile-first responsive

### Portfolio
- [ ] 8-15 curated projects
- [ ] Visual essay case studies
- [ ] High-res imagery throughout
- [ ] Next/previous project navigation

### About
- [ ] Studio philosophy
- [ ] Creative team portraits
- [ ] Client logos (selective)
- [ ] Culture/values section

### Contact
- [ ] Simple inquiry form
- [ ] Direct email prominent
- [ ] Location (if relevant)

---

## Sources

- [Pentagram](https://www.pentagram.com/) - Reference for minimal, work-forward approach
- [Collins](https://www.wearecollins.com/) - Reference for editorial case studies
- [Sagmeister & Walsh](https://sagmeisterwalsh.com/) - Reference for personality in design
- [Awwwards - Agency Portfolios](https://www.awwwards.com/awwwards/collections/agency-portfolios/)
- [AIGA - Portfolio Best Practices](https://www.aiga.org/resources/portfolio-best-practices)
- [Design Week - Agency Website Trends](https://www.designweek.co.uk/)
