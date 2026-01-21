# Newsletter Business Recipe

> **For**: Newsletter-first publishers, creator newsletters, niche content businesses
> **Key Challenges**: Subscriber acquisition, open rate optimization, monetization, churn reduction
> **Reference Sites**: Morning Brew, The Hustle, Milk Road, Stratechery, Lenny's Newsletter, Not Boring

---

## Site Architecture

### Simple Newsletter Site

```
/                           → Landing page (signup focused)
/archive/                   → Past issues
/about/                     → About the newsletter/author
/subscribe/                 → Dedicated signup page
/sponsorship/               → Advertiser info
```

### Multi-Newsletter Platform

```
/                           → Homepage (all newsletters)
/[newsletter-name]/         → Individual newsletter landing
├── /archive/               → Past issues of this newsletter
├── /subscribe/             → Subscribe to this newsletter
/about/                     → About the platform
/jobs/                      → Job board (if applicable)
/events/                    → Events (if applicable)
/advertise/                 → Sponsor information
```

### Paid Newsletter Site

```
/                           → Landing page
/archive/                   → Free archive (samples)
/subscribe/                 → Free subscription
/premium/                   → Paid tier info
├── /pricing/               → Pricing details
├── /faq/                   → Paid FAQ
/members/                   → Member area
├── /login/                 → Login
├── /account/               → Account settings
├── /archive/               → Premium archive
/about/                     → About
```

---

## Homepage / Landing Page Blueprint

### Free Newsletter Landing

```
1. Hero (Conversion-Focused)
   └── Clear value proposition
   └── Email signup form (prominent)
   └── Social proof (subscriber count, testimonials)

2. What You Get
   └── Newsletter preview/format
   └── Topics covered
   └── Delivery frequency

3. Sample Content
   └── Preview of actual newsletter
   └── Or highlights from past issues

4. Social Proof
   └── Subscriber testimonials
   └── Press mentions
   └── Reader quotes

5. About the Author/Team
   └── Credibility builders
   └── Personal connection

6. Secondary Signup
   └── Reinforce signup CTA
   └── FAQ about signup
```

### Hero Pattern (Newsletter)

```
┌────────────────────────────────────────────────────────────────────┐
│ [Logo]                                          [Archive] [About] │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│  The daily newsletter for                                         │
│  busy professionals                                               │
│                                                                    │
│  Join 500,000+ readers getting smarter about                     │
│  [topic] in just 5 minutes a day.                                │
│                                                                    │
│  ┌────────────────────────────────────────────────────┐          │
│  │ [your@email.com                    ] [Subscribe]   │          │
│  └────────────────────────────────────────────────────┘          │
│                                                                    │
│  ✓ Free  ✓ Daily  ✓ 5-minute read  ✓ Unsubscribe anytime        │
│                                                                    │
├────────────────────────────────────────────────────────────────────┤
│ "Finally, a newsletter I actually read."  — Reader, Company      │
│                                                                    │
│ Featured in: [Forbes] [TechCrunch] [NYT] [WSJ]                   │
└────────────────────────────────────────────────────────────────────┘
```

### Paid Newsletter Landing

```
┌────────────────────────────────────────────────────────────────────┐
│ [Logo]                               [Free] [Premium] [About]     │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│  Deep analysis on [topic] that                                    │
│  you can't get anywhere else                                      │
│                                                                    │
│  Weekly insights from [Author] — trusted by executives at        │
│  [Company], [Company], and [Company].                            │
│                                                                    │
│  ┌───────────────────┐  ┌───────────────────┐                    │
│  │ FREE              │  │ PREMIUM           │                    │
│  │ Weekly digest     │  │ $15/month         │                    │
│  │                   │  │                   │                    │
│  │ [Subscribe free]  │  │ [Start 7-day      │                    │
│  │                   │  │  free trial]      │                    │
│  └───────────────────┘  └───────────────────┘                    │
│                                                                    │
│  ⭐⭐⭐⭐⭐ "Best newsletter on [topic]" — 10,000+ subscribers    │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

---

## Signup Form Patterns

### Simple Email Capture

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│  [email@example.com                    ] [Subscribe]        │
│                                                             │
│  Join 100,000+ readers. Unsubscribe anytime.               │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### With Name (for personalization)

```
┌─────────────────────────────────────────────────────────────┐
│                                                             │
│  First name (optional)  [John                   ]          │
│  Email address          [john@example.com        ]          │
│                                                             │
│  [Subscribe for Free]                                       │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

### Topic Selection (multi-newsletter)

```
┌─────────────────────────────────────────────────────────────┐
│ Which newsletters interest you?                             │
│                                                             │
│ ☑ Daily Brief (Mon-Fri)                                    │
│ ☐ Weekly Deep Dive (Sat)                                   │
│ ☐ Breaking News Alerts                                     │
│ ☑ Weekend Edition                                          │
│                                                             │
│ Email: [john@example.com        ]                          │
│                                                             │
│ [Subscribe]                                                 │
└─────────────────────────────────────────────────────────────┘
```

---

## Sample Content Display

### Newsletter Preview Pattern

Show what subscribers actually receive:

```
┌────────────────────────────────────────────────────────────────────┐
│ Here's what you'll get:                                           │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│ ┌────────────────────────────────────────────────────────────┐    │
│ │ 📧 SAMPLE NEWSLETTER                        Jan 10, 2026   │    │
│ ├────────────────────────────────────────────────────────────┤    │
│ │                                                            │    │
│ │ Good morning! Here's what you need to know today:         │    │
│ │                                                            │    │
│ │ 📈 MARKETS                                                 │    │
│ │ S&P 500 hits new high as tech rallies...                  │    │
│ │                                                            │    │
│ │ 🏢 BIG STORY                                              │    │
│ │ Why [Company] is betting big on [thing]...                │    │
│ │                                                            │    │
│ │ 💡 QUICK HITS                                             │    │
│ │ • Bullet point insight one                                │    │
│ │ • Bullet point insight two                                │    │
│ │ • Bullet point insight three                              │    │
│ │                                                            │    │
│ │ 😂 MEME OF THE DAY                                        │    │
│ │ [Image placeholder]                                       │    │
│ │                                                            │    │
│ └────────────────────────────────────────────────────────────┘    │
│                                                                    │
│ [Read full sample →]                                              │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

### Archive Display

```
┌────────────────────────────────────────────────────────────────────┐
│ Archive                                        [Search] [Filter]  │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│ ┌────────────────────────────────────────────────────────────┐    │
│ │ Jan 10, 2026                                 [Free] [Read] │    │
│ │ Headline of this newsletter edition                        │    │
│ │ Brief preview text of the content...                       │    │
│ └────────────────────────────────────────────────────────────┘    │
│                                                                    │
│ ┌────────────────────────────────────────────────────────────┐    │
│ │ Jan 9, 2026                              [Premium] [🔒]    │    │
│ │ Headline of premium edition                                │    │
│ │ Brief preview... [Subscribe to read]                       │    │
│ └────────────────────────────────────────────────────────────┘    │
│                                                                    │
│ [Load more]                                                       │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

---

## Social Proof Patterns

### Subscriber Count

```
Join 500,000+ professionals ← Best if large number
Join readers from Google, Apple, Meta... ← Best if notable companies
Trusted by executives at Fortune 500 companies ← Best for B2B
```

### Testimonial Display

```
┌────────────────────────────────────────────────────────────────────┐
│ What readers are saying                                           │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│ ┌──────────────────┐  ┌──────────────────┐  ┌──────────────────┐ │
│ │ "The only email  │  │ "I've tried      │  │ "Saves me hours  │ │
│ │ I open first     │  │ dozens of        │  │ every week."     │ │
│ │ every morning."  │  │ newsletters.     │  │                  │ │
│ │                  │  │ This is the      │  │ — Sarah K.       │ │
│ │ — John D.        │  │ one I actually   │  │   VP Marketing   │ │
│ │   CEO, StartupX  │  │ read."           │  │   TechCorp       │ │
│ │                  │  │                  │  │                  │ │
│ │                  │  │ — Mike R.        │  │                  │ │
│ │                  │  │   Founder        │  │                  │ │
│ └──────────────────┘  └──────────────────┘  └──────────────────┘ │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

### Press/Media Mentions

```
┌────────────────────────────────────────────────────────────────────┐
│ As featured in:                                                   │
│                                                                    │
│ [Forbes logo] [TechCrunch] [The Verge] [NYT] [WSJ]               │
│                                                                    │
│ "The newsletter that's reshaping how [industry] gets news"       │
│ — Forbes                                                          │
└────────────────────────────────────────────────────────────────────┘
```

---

## Monetization Patterns

### Sponsorship Model

**Sponsorship Page Content**:

```
┌────────────────────────────────────────────────────────────────────┐
│ Partner with [Newsletter Name]                                    │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│ Reach 500,000+ [audience description]                            │
│                                                                    │
│ OUR AUDIENCE                                                       │
│ ├── 70% director-level or above                                  │
│ ├── Average HHI: $200K+                                          │
│ ├── Top industries: Tech, Finance, Consulting                    │
│ └── 45% open rate (industry avg: 21%)                            │
│                                                                    │
│ SPONSORSHIP OPTIONS                                               │
│ ├── Primary Sponsor: [Lead placement] — $X,XXX                   │
│ ├── Secondary Sponsor: [Below fold] — $X,XXX                     │
│ └── Classified: [Text only] — $XXX                               │
│                                                                    │
│ PAST SPONSORS                                                     │
│ [Logo] [Logo] [Logo] [Logo] [Logo]                               │
│                                                                    │
│ [Download Media Kit]  [Contact Sales]                            │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

### Paid Subscription Tiers

```
┌────────────────────────────────────────────────────────────────────┐
│ Choose your plan                                                  │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│ ┌──────────────────────────┐  ┌──────────────────────────┐       │
│ │ FREE                     │  │ PREMIUM                  │       │
│ │                          │  │                          │       │
│ │ $0/month                 │  │ $15/month or $150/year  │       │
│ │                          │  │ (save 17%)              │       │
│ │ ✓ Weekly digest          │  │                          │       │
│ │ ✓ Breaking news          │  │ Everything in Free, plus:│       │
│ │ ✓ Public archive         │  │                          │       │
│ │                          │  │ ✓ Daily deep dives       │       │
│ │                          │  │ ✓ Premium archive        │       │
│ │                          │  │ ✓ Member Discord         │       │
│ │                          │  │ ✓ Exclusive events       │       │
│ │                          │  │ ✓ Direct author access   │       │
│ │                          │  │                          │       │
│ │ [Subscribe Free]         │  │ [Start Free Trial]       │       │
│ └──────────────────────────┘  └──────────────────────────┘       │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

---

## Referral Program

### Referral Program Page

```
┌────────────────────────────────────────────────────────────────────┐
│ Share [Newsletter] and earn rewards                               │
├────────────────────────────────────────────────────────────────────┤
│                                                                    │
│ Your referral link:                                               │
│ [newsletter.com/ref/abc123            ] [Copy] [Share]            │
│                                                                    │
│ YOUR PROGRESS                                                      │
│ ████████████░░░░░░░░ 12/25 referrals                              │
│ Next reward: Exclusive merch (25 referrals)                       │
│                                                                    │
│ REWARDS                                                           │
│ ├── 3 referrals: Exclusive sticker pack                          │
│ ├── 10 referrals: [Newsletter] t-shirt                           │
│ ├── 25 referrals: Limited edition merch box                      │
│ ├── 50 referrals: 1-on-1 call with founder                       │
│ └── 100 referrals: Lifetime premium access                        │
│                                                                    │
│ [Share on Twitter] [Share on LinkedIn] [Copy Link]               │
│                                                                    │
└────────────────────────────────────────────────────────────────────┘
```

---

## Email-Specific Optimization

### Welcome Email Sequence

| Day | Email | Purpose |
|-----|-------|---------|
| 0 | Welcome + sample | Confirm subscription, show value |
| 1 | "What to expect" | Set expectations |
| 3 | Best past content | Show back catalog |
| 7 | Referral invite | Growth |
| 14 | Paid upgrade (if applicable) | Monetization |

### Re-Engagement Triggers

| Trigger | Action |
|---------|--------|
| No opens in 30 days | Win-back email |
| No opens in 60 days | Final re-engagement |
| No opens in 90 days | Remove from list |

---

## Growth Tactics

### Viral Growth Elements

1. **Referral program** with tangible rewards
2. **Share buttons** in every email
3. **Forward-friendly** content
4. **Social content** that drives to signup
5. **Podcast/content** partnerships
6. **Cross-promotions** with other newsletters

### Conversion Points

| Point | Conversion Rate | Notes |
|-------|-----------------|-------|
| Twitter profile link | 0.1-0.5% | Low intent |
| Twitter thread CTA | 1-3% | Higher intent |
| Guest podcast | 2-5% | High trust |
| Partner shoutout | 3-8% | Warm intro |
| Landing page (cold) | 20-40% | Intent varies |
| Landing page (warm) | 40-60% | Referral traffic |

---

## Metrics to Track

| Metric | Target | Notes |
|--------|--------|-------|
| Open rate | 40%+ | Industry avg is 21% |
| Click rate | 5%+ | On CTAs within email |
| Subscriber growth | 5-10%/month | Net of churn |
| Churn rate | <2%/month | Keep low |
| Referral rate | 10%+ | Of subscribers refer |
| Paid conversion | 5-10% | Free to paid |
| Sponsor fill rate | 80%+ | If ad-supported |
| Revenue per subscriber | Track | LTV calculation |

---

## Reference Sites

### Free Newsletters (Ad-Supported)
- **Morning Brew** — Business daily
- **The Hustle** — Business/tech
- **Milk Road** — Crypto
- **TLDR** — Tech

### Paid Newsletters
- **Stratechery** — Tech analysis
- **Lenny's Newsletter** — Product
- **The Generalist** — Business strategy
- **Not Boring** — Business/tech

### Newsletter Platforms
- **Substack** — Creator newsletters
- **beehiiv** — Newsletter business
- **ConvertKit** — Creator economy
- **Ghost** — Publishing platform

---

*See also: [Media Recipe](./SITE.md) | [Media Industry Patterns](../../library/industry/media.md) | [Form Optimization](../../library/conversion/form-optimization.md)*
