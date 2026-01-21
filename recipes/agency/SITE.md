# Agency / Portfolio Website Recipe

> **Business Type**: Creative agency, design studio, marketing agency, consulting firm
> **Primary Goals**: Showcase work, attract clients, establish credibility, generate leads
> **Revenue Model**: Project-based, retainers, consulting
> **Reference Sites**: Pentagram, IDEO, Work & Co, Fantasy, Buck

---

## Site Architecture

### Core Pages (Must Have)

```
/                       Homepage (agency positioning)
├── /work/              Portfolio hub
│   └── /work/[project]/ Individual case studies
├── /services/          Services overview
│   └── /services/[service]/ Individual service pages
├── /about/             Team and culture
├── /contact/           Contact + inquiry form
└── /careers/           Job openings (if applicable)
```

### Content & Trust Pages

```
├── /blog/              Insights hub
│   └── /blog/[post]/   Individual posts
├── /case-studies/      Deep-dive case studies (if separate from /work/)
├── /clients/           Client logos and testimonials
└── /awards/            Recognition and press
```

### Legal Pages

```
├── /privacy/           Privacy policy
├── /terms/             Terms of service
└── /cookies/           Cookie policy
```

---

## Page Hierarchy Diagram

```
                    ┌─────────────┐
                    │  HOMEPAGE   │
                    └──────┬──────┘
                           │
        ┌──────────────────┼──────────────────┐
        │                  │                  │
   ┌────▼────┐       ┌────▼────┐        ┌────▼────┐
   │  WORK   │       │ SERVICES│        │  ABOUT  │
   └────┬────┘       └────┬────┘        └────┬────┘
        │                 │                  │
   ┌────┼────┐       ┌────┼────┐        ┌────┼────┐
   │    │    │       │    │    │        │    │    │
Case  Case  Case  Service Service     Team  Culture  Contact
Study Study Study  Page   Page
```

---

## Navigation Structure

### Primary Navigation

Keep it minimal — agencies sell on work, not navigation.

```
[Logo]    Work    Services    About    [Contact]
                                         ↑ CTA button
```

### Mega Menu (Optional - For Larger Agencies)

```
WORK                    SERVICES             ABOUT
────                    ────────             ─────
Featured Projects       Branding             Our Story
By Industry            Web Design           Team
By Service             Digital Marketing    Culture
                       Strategy             Careers
                       Content              Press
```

### Footer Navigation

```
WORK              SERVICES          COMPANY           CONNECT
────              ────────          ───────           ───────
All Projects      Branding          About             Instagram
Case Studies      Web Design        Team              LinkedIn
Industries        Marketing         Careers           Twitter
Clients           Consulting        Press             Newsletter

© 2024 Agency Name | Privacy | Terms | [Back to Top]
```

---

## Homepage Structure

### Recommended Sections

```
1. Hero
   └── Bold statement, portfolio preview, primary CTA

2. Selected Work
   └── 3-6 featured projects

3. Services Overview
   └── What you do (brief)

4. Clients
   └── Logo cloud of notable clients

5. Testimonial
   └── Client quote (impactful)

6. About Preview
   └── Team intro, culture glimpse

7. Awards/Press (optional)
   └── Recognition

8. CTA
   └── Start a project / Get in touch

9. Blog Preview (optional)
   └── Latest insights
```

### Hero Patterns

**Pattern 1: Statement + Work Preview**
```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│         We design brands that                                   │
│         people remember.                                        │
│                                                                 │
│         [See Our Work]                                          │
│                                                                 │
│  ┌─────────────┐ ┌─────────────┐ ┌─────────────┐               │
│  │ [Project]   │ │ [Project]   │ │ [Project]   │               │
│  │  Preview    │ │  Preview    │ │  Preview    │               │
│  └─────────────┘ └─────────────┘ └─────────────┘               │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Pattern 2: Full-Screen Project**
```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│         [Full-width featured project image/video]               │
│                                                                 │
│         Project Name — Client                                   │
│                                                                 │
│         [View Case Study]                                       │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Pattern 3: Reel/Showreel**
```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│              [Autoplay video reel of work]                      │
│                                                                 │
│         Agency Name                                             │
│         Digital Product Studio                                  │
│                                                                 │
│         [Play Reel]  [Start a Project]                          │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Work/Portfolio Page

The most critical page for any agency.

> "Portfolio and agency website templates should showcase your work and attract clients, featuring sleek project galleries, team bios, and case study sections to help highlight your expertise."
>
> *Source: [Webflow](https://webflow.com/templates/category/portfolio-and-agency-websites)*

### Portfolio Layout Options

**Grid Layout**
```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Our Work                          [Filter: All ▼]              │
│                                                                 │
│  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐ │
│  │                 │  │                 │  │                 │ │
│  │  [Project 1]    │  │  [Project 2]    │  │  [Project 3]    │ │
│  │                 │  │                 │  │                 │ │
│  │  Client Name    │  │  Client Name    │  │  Client Name    │ │
│  │  Service        │  │  Service        │  │  Service        │ │
│  └─────────────────┘  └─────────────────┘  └─────────────────┘ │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Masonry Layout**
Varied sizes for visual interest

**List Layout**
```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Project Name                     Client    Branding   2024    │
│  ─────────────────────────────────────────────────────────────  │
│  Project Name                     Client    Web Design  2024   │
│  ─────────────────────────────────────────────────────────────  │
│  Project Name                     Client    Campaign   2023    │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Filtering & Organization

> "One fundamental strategy for showcasing services effectively is to organize projects thoughtfully. By grouping projects based on service type or industry, design agencies can streamline navigation."
>
> *Source: [Stan Vision](https://www.stan.vision/journal/creating-a-portfolio-that-sells-for-design-agencies)*

**Filter Options**:
- By service (Branding, Web, Marketing)
- By industry (Tech, Finance, Healthcare)
- By year
- By project type (Campaign, Product, Identity)

---

## Case Study Page

### Structure

```
1. Hero
   └── Project title, client, service, hero image/video

2. Overview
   └── Brief, challenge, solution summary

3. The Challenge
   └── Client problem, context

4. The Approach
   └── Process, strategy, collaboration

5. The Work
   └── Deliverables with visuals

6. Results
   └── Metrics, outcomes, impact

7. Testimonial
   └── Client feedback

8. Credits (optional)
   └── Team members

9. Next Project
   └── Navigation to next case study
```

### Case Study Layout

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  [Full-width hero image]                                        │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Project Name                                                   │
│                                                                 │
│  Client: Company          Services: Branding, Web               │
│  Year: 2024               Industry: Technology                  │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  The Challenge                                                  │
│                                                                 │
│  [Description of the problem the client faced]                  │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  [Full-width work image]                                        │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  The Approach                                                   │
│                                                                 │
│  [Process description]                                          │
│                                                                 │
│  [Work images in grid]                                          │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  The Results                                                    │
│                                                                 │
│  [40%]        [3x]           [100K+]                            │
│  Increase     Revenue        Users                              │
│  in traffic   Growth         Reached                            │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  "Working with [Agency] transformed our brand..."               │
│  — Client Name, Title, Company                                  │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Next Project: [Project Name] →                                 │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Content Requirements

> "While stunning visuals can grab attention, clear and concise descriptions provide essential context and insight into each project's objectives, processes, and outcomes."
>
> *Source: [Stan Vision](https://www.stan.vision/journal/creating-a-portfolio-that-sells-for-design-agencies)*

**Must Include**:
- High-quality project visuals
- Problem/challenge statement
- Solution approach
- Measurable results (when available)
- Client testimonial

---

## Services Page

### Overview Page Structure

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  What We Do                                                     │
│                                                                 │
│  We help ambitious brands solve complex problems                │
│  through strategy, design, and technology.                      │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌─────────────────┐  ┌─────────────────┐  ┌─────────────────┐ │
│  │                 │  │                 │  │                 │ │
│  │  Branding       │  │  Digital        │  │  Strategy       │ │
│  │                 │  │  Products       │  │                 │ │
│  │  Brand identity │  │  Web design     │  │  Brand strategy │ │
│  │  Visual systems │  │  App design     │  │  Marketing      │ │
│  │  Guidelines     │  │  UX/UI          │  │  Consulting     │ │
│  │                 │  │                 │  │                 │ │
│  │  [Learn More]   │  │  [Learn More]   │  │  [Learn More]   │ │
│  └─────────────────┘  └─────────────────┘  └─────────────────┘ │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Our Process                                                    │
│                                                                 │
│  [1. Discover] → [2. Define] → [3. Design] → [4. Deliver]      │
│                                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  [Start a Project]                                              │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Individual Service Page Structure

1. Hero (service name, brief description)
2. What we do (detailed service description)
3. Our approach/process
4. Related work (projects using this service)
5. FAQ (service-specific questions)
6. CTA (Get started)

---

## About Page

### Structure

```
1. Hero
   └── Mission statement, team photo

2. Our Story
   └── Agency history, founding story

3. What We Believe
   └── Values, principles

4. The Team
   └── Team members with photos

5. Culture
   └── Working style, environment

6. Clients
   └── Logo cloud, testimonials

7. Awards (optional)
   └── Recognition, press

8. Careers CTA
   └── Join us link
```

### Team Section

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Our Team                                                       │
│                                                                 │
│  ┌─────────┐  ┌─────────┐  ┌─────────┐  ┌─────────┐            │
│  │ [Photo] │  │ [Photo] │  │ [Photo] │  │ [Photo] │            │
│  │         │  │         │  │         │  │         │            │
│  │ Name    │  │ Name    │  │ Name    │  │ Name    │            │
│  │ Title   │  │ Title   │  │ Title   │  │ Title   │            │
│  │ [in]    │  │ [in]    │  │ [in]    │  │ [in]    │            │
│  └─────────┘  └─────────┘  └─────────┘  └─────────┘            │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Contact Page

### Elements

```
1. Headline
   └── "Let's work together" / "Start a project"

2. Introduction
   └── Brief, welcoming copy

3. Contact Form
   └── Project inquiry fields

4. Alternative Contact
   └── Email, phone, address

5. Office Info (optional)
   └── Location, map, hours

6. FAQ
   └── Process questions
```

### Contact Form Fields

| Field | Required | Notes |
|-------|----------|-------|
| Name | Yes | Full name |
| Email | Yes | Business email preferred |
| Company | Yes | To qualify leads |
| Phone | No | For urgent projects |
| Budget Range | Recommended | Dropdown or range |
| Project Type | Recommended | Checkbox or dropdown |
| Timeline | Recommended | When they need it |
| Project Description | Yes | Textarea |
| How did you hear about us? | No | For attribution |

---

## Trust & Credibility

### Social Proof Elements

> "Client feedback or testimonials play a crucial role in validating the agency's capabilities and building trust with potential future clients."
>
> *Source: [Gain Blog](https://blog.gainapp.com/creative-agency-portfolio/)*

**Types**:
- Client logos
- Testimonials with photos/titles
- Case study results (metrics)
- Awards and recognition
- Press mentions
- Client video testimonials

### Client Logo Cloud

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Trusted by innovative brands                                   │
│                                                                 │
│  [Logo] [Logo] [Logo] [Logo] [Logo] [Logo]                     │
│  [Logo] [Logo] [Logo] [Logo] [Logo] [Logo]                     │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Testimonial Display

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  "The team at [Agency] didn't just deliver a website—           │
│   they transformed how we think about our brand."               │
│                                                                 │
│   [Photo]  Sarah Chen                                           │
│            VP of Marketing, TechCorp                            │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

---

## Key User Journeys

### Journey 1: New Prospect

```
[Search/Referral] → Homepage → Work → Case Study → Contact
```

### Journey 2: Research Phase

```
[Direct] → Homepage → Services → About → Work → Contact
```

### Journey 3: Specific Need

```
[Search "branding agency"] → Services/Branding → Work (Branding) → Contact
```

### Journey 4: Talent

```
[Job Board] → Careers → About → Work → Apply
```

---

## SEO Strategy

### High-Intent Keywords

- "[Service] agency [location]"
- "Best [service] agency"
- "[Industry] design agency"

### Content Keywords

- "[Service] process"
- "[Industry] branding examples"
- "How to [topic]" (blog)

### Technical SEO

- Fast load times (work images optimized)
- Schema for Organization, LocalBusiness
- Project schema for case studies
- Image alt text on all work
- Clean URLs

---

## Implementation Checklist

### Foundation
- [ ] Homepage with work preview
- [ ] Work/portfolio page
- [ ] Services overview
- [ ] About page
- [ ] Contact with form

### Portfolio
- [ ] 5-10 case studies minimum
- [ ] High-quality project images
- [ ] Results/metrics where available
- [ ] Client testimonials

### Trust
- [ ] Client logos (8-12)
- [ ] Testimonials (3+)
- [ ] Team photos
- [ ] Awards/press (if applicable)

### Lead Generation
- [ ] Contact form working
- [ ] Email notifications set up
- [ ] CRM integration (optional)
- [ ] Lead qualification fields

### Content
- [ ] Blog with 5+ posts
- [ ] Service descriptions
- [ ] Process explanation
- [ ] FAQ content

---

## Sources

- [Webflow - Portfolio & Agency Templates](https://webflow.com/templates/category/portfolio-and-agency-websites)
- [Stan Vision - Creating a Portfolio for Design Agencies](https://www.stan.vision/journal/creating-a-portfolio-that-sells-for-design-agencies)
- [Gain Blog - Creative Agency Portfolio Tips](https://blog.gainapp.com/creative-agency-portfolio/)
- [Awwwards - Agency Portfolios](https://www.awwwards.com/awwwards/collections/agency-portfolios/)
- [DesignRush - Best Portfolio Website Examples](https://www.designrush.com/best-designs/websites/trends/portfolio-website-examples)
