# Media & Publishing Website Recipe

> **For**: News sites, digital magazines, blogs, content platforms, newsletters
> **Key Challenges**: Reader engagement, subscription conversion, ad revenue optimization, content discovery
> **Reference Sites**: The New York Times, The Atlantic, Substack, Medium, The Information, Morning Brew

---

## Site Architecture

### News / Magazine Site

```
/                           → Homepage (latest + featured)
/news/                      → News section hub
├── /[category]/            → Category pages (Politics, Tech, etc.)
├── /[article-slug]/        → Article pages
/opinion/                   → Opinion/Editorial section
/features/                  → Long-form features
/video/                     → Video content hub
/podcasts/                  → Podcast hub
/newsletters/               → Newsletter hub
├── /[newsletter-name]/     → Individual newsletters
/topics/                    → Topic tags index
├── /[topic]/               → Topic archive
/authors/                   → Authors index
├── /[author]/              → Author profile + articles
/subscribe/                 → Subscription page
/about/                     → About the publication
/contact/                   → Contact/tips
/search/                    → Search results
```

### Blog / Newsletter Platform

```
/                           → Homepage (recent posts)
/archive/                   → All posts archive
/category/                  → Category index
├── /[category]/            → Category archive
/[post-slug]/               → Individual posts
/about/                     → About the author/publication
/subscribe/                 → Newsletter signup
/members/                   → Member-only area (if applicable)
├── /login/                 → Member login
├── /dashboard/             → Member dashboard
/search/                    → Search
```

---

## Homepage Blueprint

### News Site Homepage

```
1. Header
   └── Logo + navigation
   └── Search
   └── Subscribe CTA
   └── Account/login

2. Breaking/Featured
   └── Lead story (large)
   └── 3-4 secondary stories
   └── "Just In" ticker (optional)

3. Section Hubs
   └── News, Opinion, Features tabs
   └── Or horizontal section strips
   └── Latest from each section

4. Newsletter Signup
   └── Inline signup form
   └── Value proposition
   └── Preview/sample

5. Trending / Popular
   └── Most read
   └── Most shared
   └── Editor's picks

6. Video / Multimedia
   └── Featured video
   └── Video playlist
   └── Podcast episodes

7. Opinion / Analysis
   └── Opinion pieces
   └── Analysis/explainers

8. Magazine / Long-form
   └── Featured features
   └── Photo essays
   └── Investigations

9. Subscription CTA
   └── Paywall preview
   └── Pricing
   └── Trial offer

10. Footer
    └── Section links
    └── Legal
    └── Social links
```

### Homepage Layout Pattern

```
┌────────────────────────────────────────────────────────────────────┐
│ [Logo]  News | Opinion | Features | Video | Podcasts  [🔍] [Subscribe] │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│  ┌────────────────────────────────┐  ┌───────────────────────┐    │
│  │                                │  │ • Secondary Story 1   │    │
│  │      LEAD STORY               │  ├───────────────────────┤    │
│  │      [Large Image]            │  │ • Secondary Story 2   │    │
│  │                                │  ├───────────────────────┤    │
│  │      Headline Here...         │  │ • Secondary Story 3   │    │
│  │      Deck text...             │  ├───────────────────────┤    │
│  │                                │  │ • Secondary Story 4   │    │
│  └────────────────────────────────┘  └───────────────────────┘    │
│                                                                    │
├────────────────────────────────────────────────────────────────────┤
│  LATEST NEWS                                        [See all →]   │
│  ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐                 │
│  │ Story 1 │ │ Story 2 │ │ Story 3 │ │ Story 4 │                 │
│  └─────────┘ └─────────┘ └─────────┘ └─────────┘                 │
│                                                                    │
├────────────────────────────────────────────────────────────────────┤
│  ┌──────────────────────────────────────────────────────────────┐ │
│  │  📧 The Daily Brief                                          │ │
│  │  Get the top stories delivered to your inbox every morning.  │ │
│  │  [email@example.com        ] [Subscribe - It's free]        │ │
│  └──────────────────────────────────────────────────────────────┘ │
│                                                                    │
├────────────────────────────────────────────────────────────────────┤
│  OPINION                            │  FEATURES                    │
│  ┌─────────────────────────────┐   │  ┌─────────────────────────┐ │
│  │ [Author] Opinion piece...   │   │  │ [Image] Feature story...│ │
│  └─────────────────────────────┘   │  └─────────────────────────┘ │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

---

## Article Page Patterns

### Standard Article Layout

```
┌────────────────────────────────────────────────────────────────────┐
│ HEADER (sticky on scroll)                                          │
│ [Logo] [Menu] [Search] [Subscribe]                                │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│  [Category] · [Topic tags]                                        │
│                                                                    │
│  Article Headline Goes Here in                                    │
│  Large Typography                                                 │
│                                                                    │
│  Deck/subtitle providing context and drawing reader in            │
│                                                                    │
│  [Author Photo] By Author Name · Jan 10, 2026 · 8 min read       │
│                                                                    │
│  [Share] [Save] [Listen] [Print]                                  │
│                                                                    │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│  [Full-width lead image with caption]                             │
│                                                                    │
├────────────────────────────────────────────────────────────────────┤
│ ┌──────────────────────────────────────┐  ┌─────────────────────┐ │
│ │                                      │  │ STICKY SIDEBAR      │ │
│ │  Article body text in optimal        │  │                     │ │
│ │  reading width (600-700px).          │  │ Related stories     │ │
│ │                                      │  │ Newsletter signup   │ │
│ │  [Inline images, videos]             │  │ Ad unit             │ │
│ │                                      │  │                     │ │
│ │  [Pull quotes]                       │  │                     │ │
│ │                                      │  │                     │ │
│ │  [Data visualizations]               │  │                     │ │
│ │                                      │  │                     │ │
│ │  [Embedded social posts]             │  │                     │ │
│ │                                      │  │                     │ │
│ └──────────────────────────────────────┘  └─────────────────────┘ │
│                                                                    │
├────────────────────────────────────────────────────────────────────┤
│  [Tags]                                                           │
│  [Share buttons]                                                  │
│  [Author bio with links]                                         │
│                                                                    │
├────────────────────────────────────────────────────────────────────┤
│  COMMENTS                                                         │
│  [Comment form] [Community guidelines]                           │
│  [Existing comments threaded]                                    │
│                                                                    │
├────────────────────────────────────────────────────────────────────┤
│  RELATED STORIES                                                  │
│  ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐                 │
│  │ Related │ │ Related │ │ Related │ │ Related │                 │
│  └─────────┘ └─────────┘ └─────────┘ └─────────┘                 │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

### Typography Best Practices

| Element | Recommendation |
|---------|----------------|
| Body text | 18-21px, serif or clean sans-serif |
| Line height | 1.5-1.7 |
| Line length | 60-75 characters (600-700px) |
| Paragraph spacing | 1.5-2em between paragraphs |
| Headline | 32-48px for article titles |
| Deck/subtitle | 20-24px, lighter weight |

### Long-Form Article Enhancements

```
┌────────────────────────────────────────────────────────────────────┐
│ Progress bar (reading progress indicator at top)                   │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│ CHAPTER 1: Introduction                                           │
│                                                                    │
│ [Full-width immersive image]                                      │
│                                                                    │
│ [Article text...]                                                 │
│                                                                    │
│ [Sidebar: Table of contents - sticky]                             │
│ ├── Chapter 1                                                     │
│ ├── Chapter 2                                                     │
│ └── Chapter 3                                                     │
│                                                                    │
│ [Data visualization: Interactive chart]                           │
│                                                                    │
│ [Pull quote with author attribution]                              │
│                                                                    │
│ [Audio option: Listen to this article]                            │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

---

## Subscription & Paywall Patterns

### Paywall Types

| Type | Description | Best For |
|------|-------------|----------|
| **Hard paywall** | All content behind paywall | Premium/exclusive content (The Information) |
| **Metered paywall** | X free articles/month | General interest news (NYT, WSJ) |
| **Freemium** | Some free, premium content paid | Mix of general + exclusive |
| **Registration wall** | Free after signup | Building email list, ad-supported |
| **Donations/Tips** | Content free, support optional | Independent journalism |

### Metered Paywall Flow

```
VISIT 1-3               VISIT 4-5              VISIT 6+
   │                       │                      │
   ▼                       ▼                      ▼
Full access            Soft prompt            Hard block
(No interruption)      "3 articles left"      "Subscribe to continue"

DESIGN:                DESIGN:                DESIGN:
No paywall UI          Banner notification    Modal overlay
                       Sticky footer          Article fades out
                       Exit intent            Clear value prop
```

### Subscription Page Pattern

```
┌────────────────────────────────────────────────────────────────────┐
│ Journalism that matters.                                          │
│ Subscribe to [Publication].                                       │
│                                                                    │
│ Get unlimited access to award-winning journalism,                │
│ exclusive newsletters, and member-only events.                   │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│ ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐ │
│ │                  │  │  RECOMMENDED     │  │                  │ │
│ │  MONTHLY         │  │                  │  │  ANNUAL          │ │
│ │                  │  │  ANNUAL          │  │  + PREMIUM       │ │
│ │  $15/month       │  │                  │  │                  │ │
│ │                  │  │  $10/month       │  │  $25/month       │ │
│ │                  │  │  billed annually │  │  billed annually │ │
│ │  • Unlimited     │  │  ($120/year)     │  │  ($300/year)     │ │
│ │    access        │  │                  │  │                  │ │
│ │  • Newsletters   │  │  Everything in   │  │  Everything in   │ │
│ │  • App access    │  │  Monthly, plus:  │  │  Annual, plus:   │ │
│ │                  │  │                  │  │                  │ │
│ │                  │  │  • 33% savings   │  │  • Events access │ │
│ │                  │  │  • Gift a sub    │  │  • Archive       │ │
│ │                  │  │                  │  │  • Print edition │ │
│ │                  │  │                  │  │                  │ │
│ │  [Subscribe]     │  │  [Subscribe]     │  │  [Subscribe]     │ │
│ └──────────────────┘  └──────────────────┘  └──────────────────┘ │
│                                                                    │
│ Already a subscriber? [Log in]                                   │
│ Student/educator? [Special rate]                                 │
│ Group/corporate? [Contact us]                                    │
│                                                                    │
├────────────────────────────────────────────────────────────────────┤
│ Why subscribe?                                                    │
│                                                                    │
│ ✓ [X] journalists covering [topics]                              │
│ ✓ [X] Pulitzer prizes                                            │
│ ✓ Trusted by [X] million readers                                 │
│ ✓ No ads in subscriber experience                                │
│                                                                    │
├────────────────────────────────────────────────────────────────────┤
│ "This is the journalism we need." — Reader testimonial           │
│                                                                    │
│ [See what subscribers are saying]                                │
│                                                                    │
├────────────────────────────────────────────────────────────────────┤
│ FAQ                                                               │
│ • Can I cancel anytime?                                          │
│ • What payment methods?                                          │
│ • Do you offer refunds?                                          │
└────────────────────────────────────────────────────────────────────┘
```

### Newsletter Signup Patterns

**Placement Options**:

| Placement | Conversion Rate | Notes |
|-----------|-----------------|-------|
| Inline in article | 0.5-1% | Low friction, contextual |
| End of article | 1-3% | Reader engaged, content complete |
| Pop-up (exit intent) | 1-4% | Higher friction, higher conversion |
| Sticky footer | 0.3-0.5% | Persistent, low interruption |
| Dedicated page | 5-15% | High intent visitors |

**Signup Form Pattern**:

```
┌────────────────────────────────────────────────────────────────────┐
│  📧 The Morning Brief                                             │
│                                                                    │
│  Start your day with the news that matters.                       │
│  Delivered weekdays at 6am.                                       │
│                                                                    │
│  [your@email.com                    ] [Subscribe]                 │
│                                                                    │
│  ✓ 250,000+ subscribers | ⭐ 4.8 rating | Free                    │
│                                                                    │
│  [See a sample edition →]                                         │
└────────────────────────────────────────────────────────────────────┘
```

---

## Content Discovery Patterns

### Related Content Algorithm

| Method | Description | When to Use |
|--------|-------------|-------------|
| **Same category** | Articles in same section | Always include |
| **Same tags/topics** | Shared topic tags | Topic-heavy content |
| **Same author** | More from this writer | Personality-driven content |
| **Popular** | Most read recently | General engagement |
| **Personalized** | Based on reading history | Logged-in users |
| **Editorially curated** | Staff picks | Premium feel |

### Recirculation Modules

```
END OF ARTICLE:
┌─────────────────────────────────────────────────────────┐
│ More from [Author Name]                                 │
│ ┌─────────┐ ┌─────────┐ ┌─────────┐                    │
│ │ Article │ │ Article │ │ Article │                    │
│ └─────────┘ └─────────┘ └─────────┘                    │
└─────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────┐
│ Related Stories in [Category]                          │
│ ┌─────────┐ ┌─────────┐ ┌─────────┐ ┌─────────┐       │
│ │ Article │ │ Article │ │ Article │ │ Article │       │
│ └─────────┘ └─────────┘ └─────────┘ └─────────┘       │
└─────────────────────────────────────────────────────────┘

┌─────────────────────────────────────────────────────────┐
│ Most Read This Week                                    │
│ 1. Article headline...                                 │
│ 2. Article headline...                                 │
│ 3. Article headline...                                 │
│ 4. Article headline...                                 │
│ 5. Article headline...                                 │
└─────────────────────────────────────────────────────────┘
```

---

## Author/Byline Patterns

### Author Profile Page

```
┌────────────────────────────────────────────────────────────────────┐
│                                                                    │
│  [Author Photo]                                                   │
│                                                                    │
│  Sarah Johnson                                                     │
│  Senior Technology Reporter                                       │
│                                                                    │
│  Bio text about the author, their beat, background, and          │
│  what they cover for the publication...                          │
│                                                                    │
│  [Twitter] [LinkedIn] [Email]                                     │
│                                                                    │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│  Articles by Sarah Johnson                    [Filter by topic ▼] │
│                                                                    │
│  [Article card with image, headline, date]                       │
│  [Article card with image, headline, date]                       │
│  [Article card with image, headline, date]                       │
│  ...                                                              │
│                                                                    │
│  [Load more]                                                      │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

### In-Article Byline

```
Standard:
[Photo] By Author Name · Category · Jan 10, 2026 · 5 min read

Expanded (hover/click):
┌─────────────────────────────────────────────┐
│ [Photo]  Author Name                        │
│          Tech Reporter                      │
│          [Twitter] [Email]                  │
│          [See all articles →]               │
└─────────────────────────────────────────────┘
```

---

## Advertising Patterns

### Ad Placement Best Practices

| Placement | Impact on UX | Revenue | Notes |
|-----------|--------------|---------|-------|
| **Leaderboard (top)** | Medium | High | Standard, expected |
| **Sidebar (sticky)** | Low | Medium | Stays in view |
| **In-article (native)** | Low if done well | High | Matches content |
| **Interstitial** | High (negative) | Very High | Use sparingly |
| **Footer** | Very Low | Low | Often ignored |

### Ad Layout Pattern

```
┌────────────────────────────────────────────────────────────────────┐
│ [HEADER]                                                          │
├────────────────────────────────────────────────────────────────────┤
│ [LEADERBOARD AD - 728x90]                                         │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│  ARTICLE CONTENT              │  SIDEBAR                          │
│                               │  [AD - 300x250]                   │
│  [Paragraphs...]              │                                   │
│                               │  [Related]                        │
│  [IN-ARTICLE AD - native]     │                                   │
│                               │  [AD - 300x600 sticky]            │
│  [More paragraphs...]         │                                   │
│                               │                                   │
│                                                                    │
├────────────────────────────────────────────────────────────────────┤
│ [FOOTER AD - 728x90]                                              │
├────────────────────────────────────────────────────────────────────┤
│ [FOOTER]                                                          │
└────────────────────────────────────────────────────────────────────┘
```

### Subscriber Ad-Free Experience

Highlight ad-free as a subscription benefit:

```
┌─────────────────────────────────────────────┐
│ ⚡ Reading with ads?                        │
│                                             │
│ Subscribers enjoy an ad-free experience    │
│ plus unlimited access.                     │
│                                             │
│ [Subscribe for $10/mo]                     │
└─────────────────────────────────────────────┘
```

---

## Mobile Optimization

### Mobile Article Experience

```
┌────────────────────┐
│ [Logo] [≡] [Sub]  │
├────────────────────┤
│                    │
│ Category           │
│                    │
│ Headline Here     │
│ On Mobile         │
│                    │
│ Deck text...      │
│                    │
│ By Author         │
│ Jan 10 · 5 min    │
│                    │
│ [Share] [Save]    │
│                    │
├────────────────────┤
│ [Lead Image]      │
├────────────────────┤
│                    │
│ Article body...   │
│                    │
│ [In-article ad]   │
│                    │
│ More text...      │
│                    │
├────────────────────┤
│ KEEP READING      │
│ [Related cards]   │
└────────────────────┘

[Sticky bottom bar:]
┌────────────────────┐
│ [Share][Save][Top]│
└────────────────────┘
```

### Mobile Newsletter Prompt

```
Bottom sheet (scroll trigger):
┌────────────────────────────┐
│ 📧 Like what you're       │
│ reading?                   │
│                            │
│ Get our best stories in   │
│ your inbox.               │
│                            │
│ [email        ][Subscribe]│
│                            │
│ [Maybe later]             │
└────────────────────────────┘
```

---

## Performance Considerations

### Core Web Vitals Priority

| Metric | Target | Notes |
|--------|--------|-------|
| LCP | <2.5s | Optimize hero images |
| FID | <100ms | Defer non-critical JS |
| CLS | <0.1 | Reserve space for ads |

### Optimization Strategies

- Lazy load below-fold images
- Placeholder for ad slots (prevent CLS)
- Optimize web fonts (system fonts for body text as fallback)
- Cache aggressively (CDN)
- Infinite scroll vs pagination (test both)

---

## Metrics to Track

| Metric | Target | Notes |
|--------|--------|-------|
| Pageviews per session | >2 | Recirculation effectiveness |
| Time on page | >2 min | Content quality |
| Scroll depth | >70% | Content engagement |
| Newsletter signup rate | 1-3% | Email capture |
| Subscription conversion | 2-5% | From paywall |
| Churn rate | <5%/month | Retention |
| Return visitor rate | >30% | Habit formation |
| Search share | Track | SEO success |

---

## Reference Sites

### Premium News
- **The New York Times** — Paywall + newsletter strategy
- **The Washington Post** — Digital innovation
- **The Atlantic** — Long-form excellence
- **The Information** — Hard paywall, premium

### Digital-First Publishers
- **Axios** — Format innovation
- **Morning Brew** — Newsletter-first
- **The Verge** — Tech coverage design
- **Vox** — Explainer journalism

### Newsletter Platforms
- **Substack** — Creator-focused
- **Medium** — Content platform
- **Ghost** — Publishing platform

---

*See also: [Media Industry Patterns](../../library/industry/media.md) | [Social Proof Patterns](../../library/conversion/social-proof-patterns.md) | [Psychology](../../library/conversion/psychology.md)*
