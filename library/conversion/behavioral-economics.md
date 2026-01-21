# Advanced Behavioral Economics for Conversion

> **Purpose**: Deep dive into decision science, cognitive biases, and nudge theory for conversion optimization
> **Level**: Advanced—builds on the [Psychology](./psychology.md) guide fundamentals
> **Application**: Choice architecture, pricing, checkout, onboarding, retention
> **Note**: This guide focuses on the science; for practical implementation, see related guides

---

## System 1 & System 2 Thinking

Nobel laureate Daniel Kahneman's framework from *Thinking, Fast and Slow* is foundational to understanding how users make decisions on websites.

> "System 1 and System 2 are so central to the story that I must make it absolutely clear that they are fictitious characters... [They] highlight that human behavior is partially driven by reasoned, controlled cognition and partially by inherent biases, heuristics, and prior experience."
>
> *Source: [Daniel Kahneman](https://www.marketingsociety.com/think-piece/system-1-and-system-2-thinking)*

### The Two Systems

| System 1 (Fast) | System 2 (Slow) |
|-----------------|-----------------|
| Automatic, intuitive | Controlled, analytical |
| Effortless | Requires energy and attention |
| Bias-prone | Logic-based |
| Guides 95% of daily decisions | Filters automatic instincts |
| Responsible for brand recall | Handles complex calculations |

### Marketing Applications by System

| Strategy | System 1 Approach | System 2 Approach |
|----------|-------------------|-------------------|
| **Content** | Engaging stories, visuals | Thought leadership, data |
| **Email** | Curiosity-sparking subjects | Value-driven body content |
| **Pricing** | Price anchoring, decoys | ROI calculators, comparisons |
| **Social proof** | Star ratings at glance | Detailed case studies |
| **CTAs** | Emotional appeals | Feature/benefit analysis |

### Design Principles by System

**For System 1 (Quick decisions)**:
- Strong visual hierarchy
- Familiar patterns and conventions
- Emotional imagery and faces
- Clear, prominent CTAs
- Social proof at a glance

**For System 2 (Considered decisions)**:
- Comparison tables
- Detailed specifications
- Pricing calculators
- Long-form content
- FAQ sections

> **Key insight**: Most B2C purchases are System 1 (low-value, everyday items). Most B2B purchases engage System 2 (high-value, complex decisions). Design accordingly.
>
> *Source: [Yellow Pebble](https://www.yellowpebble.co/post/daniel-kahnemans-systems-1-and-2-a-b2b-marketing-perspective)*

---

## Loss Aversion & The Endowment Effect

Loss aversion is one of the most powerful forces in decision-making.

### The 2:1 Ratio

> "Empirically, losses tend to be treated as if they were twice as large as an equivalent gain. Loss aversion was first proposed by Amos Tversky and Daniel Kahneman as an important component of prospect theory."
>
> *Source: [BehavioralEconomics.com](https://www.behavioraleconomics.com/resources/mini-encyclopedia-of-be/loss-aversion/)*

| Framing | Psychological Impact | Effectiveness |
|---------|---------------------|---------------|
| "Save $50" (gain) | Moderate | Baseline |
| "Stop losing $50" (loss) | Strong (2x) | +40-60% response |
| "Don't miss your discount" | Fear of loss | High conversion |
| "Your cart will expire" | Ownership + loss | Very high urgency |

### The Endowment Effect

> "The endowment effect, also known as divestiture aversion, is the finding that people are more likely to retain an object they own than acquire that same object when they do not own it."
>
> *Source: [Wikipedia](https://en.wikipedia.org/wiki/Endowment_effect)*

**How to create psychological ownership**:

| Tactic | Implementation | Effect |
|--------|----------------|--------|
| Free trials | "Your free trial" language | Users feel they "own" it |
| Customization | "Your personalized plan" | Investment = ownership |
| Progress saving | Saved cart, wishlist | Fear of losing progress |
| Virtual ownership | "Hold this in your cart" | Temporary possession |
| Time-limited cart | 30-minute reservation | Urgency + ownership |

### Conversion Statistics

| Tactic | Conversion Impact | Source |
|--------|-------------------|--------|
| Free trial (ownership effect) | Up to +66% B2B conversion | [Togai](https://www.togai.com/blog/increasing-saas-free-trial-conversion-rate/) |
| Loss-framed pricing | Up to +32% CVR | [Journal of Marketing Research via Invesp](https://www.invespcro.com/blog/13-loss-aversion-marketing-strategies-to-increase-conversions/) |
| Reverse trial (premium first) | +10-40% freemium→paid | [Userpilot](https://userpilot.com/blog/saas-reverse-trial/) |
| 30-day trial vs free product | 28x more effective | [App Developer Magazine](https://appdevelopermagazine.com/free-trials-have-high-customer-conversion-rate/)

**Implementation patterns**:

```
❌ "Get access to our premium features"
✅ "Don't lose access to your premium features"

❌ "Sign up for our newsletter"
✅ "Don't miss exclusive insights"

❌ "Buy now"
✅ "Claim your spot" (suggests scarcity + ownership)
```

---

## Present Bias & Hyperbolic Discounting

> "Hyperbolic discounting is our inclination to choose immediate rewards over rewards that come later in the future, even when these immediate rewards are smaller."
>
> *Source: [The Decision Lab](https://thedecisionlab.com/biases/hyperbolic-discounting)*

### The Science

When offered $50 now versus $100 in a year, many choose $50 now. But given $50 in 5 years versus $100 in 6 years, almost everyone chooses $100—even though it's the same trade-off at a distance.

**Brain regions involved**: Ventral striatum, medial prefrontal cortex, orbitofrontal cortex—all associated with immediate reward expectation.

### Marketing Applications

| Strategy | Implementation | Why It Works |
|----------|----------------|--------------|
| **Instant rewards** | Points immediately added | Immediate gratification |
| **Buy Now, Pay Later** | Afterpay, Klarna | Immediate gain, deferred pain |
| **Milestone rewards** | Progress badges | Small immediate wins |
| **Breaking down costs** | "Just £0.82/day" vs "£300/year" | Makes commitment feel smaller |
| **Same-day delivery** | Amazon Prime | Eliminates wait time |

### Practical Tactics

**1. Make future benefits present**:
```
❌ "You'll save 20% over the year"
✅ "Start saving 20% today"
```

**2. Break down commitments**:
```
❌ "Annual plan: $299/year"
✅ "Less than $1 per day"
```

**3. Gamify progress**:
- Show progress bars
- Award badges immediately
- Unlock features progressively
- Celebrate micro-milestones

**4. Reduce time to value**:
- Instant account creation
- Pre-filled forms
- One-click purchases
- Immediate access after payment

> "Consumers are far more likely to stick with brands that cut down on waiting times, ease onboarding, or offer instant feedback."
>
> *Source: [Cognitive Clicks](https://cognitive-clicks.com/blog/hyperbolic-discounting/)*

---

## The Sunk Cost Fallacy & Commitment Escalation

### Definition

> "The Sunk Cost Fallacy is the tendency for people to continue investing in a decision based on previously invested resources (time, money, or effort), even if they do not have desirable outcomes."
>
> *Source: [The Decision Lab](https://thedecisionlab.com/biases/the-sunk-cost-fallacy)*

### Ethical Applications

| Tactic | Example | Effect |
|--------|---------|--------|
| **Loyalty points** | Accumulated rewards | More purchases to reach tier |
| **Progress indicators** | "Profile 80% complete" | Investment drives completion |
| **Achievements** | Badges, streaks | Reluctance to start over |
| **Personalization** | Custom settings, playlists | Switching cost |
| **Learning curves** | Skill-based products | Time invested = retention |

### Implementation Strategies

**Loyalty Programs**:
- Show accumulated points prominently
- Display progress to next tier
- Remind users of earned status
- Highlight what they'd lose by leaving

**Progress & Achievements**:
```
┌─────────────────────────────────────────────────────────────────┐
│  Your Profile                                                    │
│                                                                 │
│  ████████████████████░░░░░  80% Complete                       │
│                                                                 │
│  You've invested 45 minutes setting up your workspace.          │
│  Just 3 more steps to unlock all features!                     │
│                                                                 │
│  Achievements: 🏆 Early Adopter  📊 Data Pro  🎯 Goal Setter   │
└─────────────────────────────────────────────────────────────────┘
```

**Upsell Framing**:
```
❌ "Upgrade to Pro for more storage"
✅ "You've used 4.2GB. Keep your files safe—upgrade now."
```

### Retention Applications

| Signal | User Response |
|--------|---------------|
| "You've been with us 2 years" | Anniversary acknowledgment |
| "Your playlist has 500 songs" | Content investment |
| "You've completed 47 courses" | Learning investment |
| "14,000 connections would miss you" | Social investment |

---

## Choice Architecture & Nudge Theory

### The Framework

> "A nudge is any aspect of the choice architecture that alters people's behavior in a predictable way without forbidding any options or significantly changing their economic incentives."
>
> *Source: Richard Thaler & Cass Sunstein, [The Decision Lab](https://thedecisionlab.com/reference-guide/psychology/nudge-theory)*

### Key Nudge Techniques

| Technique | Description | Application |
|-----------|-------------|-------------|
| **Defaults** | Pre-selected options | Annual billing pre-checked |
| **Simplification** | Reduce complexity | Fewer form fields |
| **Social norms** | Show what others do | "Most popular" badge |
| **Salience** | Make info prominent | Highlight recommended plan |
| **Framing** | Present same info differently | "95% success" vs "5% fail" |
| **Feedback** | Real-time information | Password strength meter |

### The Default Effect in Detail

> "If an online form has a box already checked to receive newsletters, most people would not uncheck it, thereby opting in by default."
>
> *Source: [Number Analytics](https://www.numberanalytics.com/blog/ultimate-guide-nudge-theory-user-psychology)*

**Powerful default applications**:

| Context | Default Setting | Impact |
|---------|-----------------|--------|
| Pricing pages | Highlight recommended tier | +20-30% selection of target |
| Billing cycle | Pre-select annual | +40% annual subscriptions |
| Add-ons | Include popular option | +15-25% add-on revenue |
| Consent | Opt-in pre-checked | +300% newsletter signups |
| Quantity | Default to multi-pack | +25% average order value |

**Ethical considerations**:
- GDPR requires explicit opt-in for marketing (EU)
- Dark patterns with defaults erode trust
- Users should easily be able to change defaults

### The Paradox of Choice

> "The famous jam study (2000) showed that while 24 jam varieties attracted more interest, 6 varieties led to significantly more purchases (30% vs. 3% conversion rate)."
>
> *Source: [Convertize](https://www.convertize.com/paradox-of-choice/)*

**Key statistics**:

| Finding | Source |
|---------|--------|
| 69.57% cart abandonment rate | Baymard Institute |
| 40% abandon due to overwhelming options | Forrester 2024 |
| Conversion peaks at 4-6 options | Multiple studies |
| 10% sales increase when P&G cut shampoo from 26 to 15 | P&G |
| 38% higher email revenue with 3 vs 5 products | Dr. Scholl's |

**Optimal option counts by context**:

| Context | Optimal Count | Rationale |
|---------|---------------|-----------|
| Pricing tiers | 3-4 | Easy comparison |
| Product variants | 4-6 | Sufficient variety |
| Email products | 3 | Focused attention |
| Menu items | 7-9 per category | Gordon Ramsay principle |
| Social share buttons | 3-4 | Reduces decision fatigue |

---

## Scarcity & FOMO Psychology

### The Science of Urgency

> "Authentic urgency and scarcity leverage psychological principles (loss aversion, FOMO, reactance) accelerating purchase decisions and improving conversion 15-35%."
>
> *Source: [CXL](https://cxl.com/blog/creating-urgency/)*

### FOMO Statistics

| Statistic | Source |
|-----------|--------|
| 69% of millennials experience FOMO | OptinMonster |
| 68% make purchases within 24 hours due to FOMO | OptinMonster |
| 60% make reactive purchases after FOMO | Consumer research |
| 73% buy viral products to fit in | Deloitte 2023 |
| 40-70% reduction in purchase probability without urgency | Behavioral economics research |

### Types of Scarcity (What Works Best)

> "Demand-based scarcity worked best for utilitarian products. Supply-based scarcity had the greatest influence on experiences. Time-based scarcity improved conversion of high-involvement products."
>
> *Source: [NEURO Business School](https://eunbs.com/the-scarcity-effect-and-fear-of-missing-out-fomo-how-the-psychology-of-urgency-drives-sales/)*

| Scarcity Type | Best For | Example |
|---------------|----------|---------|
| **Demand-based** | Utilitarian products | "15 people viewing now" |
| **Supply-based** | Experiences, events | "Only 3 tickets left" |
| **Time-based** | High-involvement purchases | "Offer ends in 2 hours" |
| **Exclusive** | Premium products | "Members only" |

### Conversion Impact Data

| Tactic | Conversion Lift |
|--------|-----------------|
| Flash sales | +35% vs standard promotions |
| Stock level display | +20% conversion |
| Social proof widgets (Booking.com) | +18% conversion |
| Time-limited offers | Up to +332% conversion |
| Targeted urgency vs universal | +30-60% |

### Implementation by Product Type

```
┌─────────────────────────────────────────────────────────────────┐
│  UTILITARIAN (everyday items)                                   │
│  Use: Demand-based scarcity                                     │
│  "47 people bought this today"                                  │
│  "Selling fast—restock in 2 weeks"                              │
├─────────────────────────────────────────────────────────────────┤
│  EXPERIENCES (travel, events)                                   │
│  Use: Supply-based scarcity                                     │
│  "Only 3 seats at this price"                                   │
│  "8 rooms left on your dates"                                   │
├─────────────────────────────────────────────────────────────────┤
│  HIGH-INVOLVEMENT (insurance, SaaS annual)                      │
│  Use: Time-based scarcity                                       │
│  "Lock in 2024 pricing—increases Jan 1"                        │
│  "Founding member rate expires Friday"                          │
├─────────────────────────────────────────────────────────────────┤
│  LUXURY/PREMIUM                                                 │
│  Use: Exclusivity scarcity                                      │
│  "Limited edition—never restocked"                              │
│  "Invitation only"                                              │
└─────────────────────────────────────────────────────────────────┘
```

### Warning: Manipulation Backfires

> "In situations where consumers perceive scarcity as manipulative or inauthentic, high FoMO individuals may experience decision fatigue or regret, leading to avoidance rather than purchase."
>
> *Source: [Springer](https://link.springer.com/article/10.1007/s43621-025-01830-5)*

**Signs your scarcity is backfiring**:
- High bounce rates on scarcity pages
- Negative reviews mentioning pressure
- Low repeat purchase rates
- Social media complaints
- Increased returns/cancellations

---

## The Peak-End Rule

### The Science

> "The Peak-End Rule, developed by Nobel laureate Daniel Kahneman, states that our memory of an event is not an average of every moment. Instead, we disproportionately remember the most emotionally intense moment (the 'peak') and the final moment (the 'end')."
>
> *Source: [Laws of UX](https://lawsofux.com/peak-end-rule/)*

### The Original Study

In Kahneman's 1993 study, participants experienced two versions of discomfort:
1. Hand in 14°C water for 60 seconds
2. Hand in 14°C water for 60 seconds, then 15°C for 30 more seconds

**Result**: Participants preferred to repeat Trial 2 (longer discomfort!) because the ending was slightly better.

### Application to Customer Experience

| Journey Stage | Peak Opportunity | End Opportunity |
|---------------|------------------|-----------------|
| **Onboarding** | Surprise welcome gift | Success celebration |
| **Purchase** | Unexpected upgrade/bonus | Beautiful confirmation |
| **Support** | Exceeding expectations | Follow-up check-in |
| **Checkout** | Free shipping threshold | Thank you + next steps |
| **Delivery** | Unboxing experience | Handwritten note |

### Real-World Example: Delta Airlines

> "Delta saw that customers dissatisfied with luggage wait were less likely to be satisfied with the overall trip. They made the luggage carousel farther from the gate—longer walk, but less wait at the carousel. Result: Baggage satisfaction and trip satisfaction went up."
>
> *Source: [CMSWire](https://www.cmswire.com/customer-experience/using-the-peak-end-rule-for-better-customer-journeys/)*

### Design for Peak & End

**Creating positive peaks**:
- Unexpected upgrades
- Milestone celebrations ("Your 100th order!")
- Surprise discounts
- Personalized recommendations that delight
- Exceptional support interactions

**Optimizing endings**:
```
┌─────────────────────────────────────────────────────────────────┐
│  Order Confirmed! 🎉                                            │
│                                                                 │
│  Thanks for being awesome, Sarah.                               │
│                                                                 │
│  Your package arrives: Thursday, Dec 12                         │
│                                                                 │
│  We've added a little surprise to your order.                   │
│  (You'll see it when you open the box!)                         │
│                                                                 │
│  [Track Your Order]                                             │
│                                                                 │
│  Questions? We're here 24/7 → support@brand.com                 │
└─────────────────────────────────────────────────────────────────┘
```

### What to Avoid

> "Many sites prioritize clicks and conversions over long-term loyalty. Designers should avoid using 'please-don't-go' pop-ups that beg users not to leave. These interface elements irritate users and contribute to a negative impression later on."
>
> *Source: [Nielsen Norman Group](https://www.nngroup.com/articles/peak-end-rule/)*

---

## Framing Effects

### The Core Principle

> "The framing effect is a cognitive bias in which people make decisions based on how the information is presented. If we frame the same information differently, it may lead to different outcomes."
>
> *Source: [Lyssna](https://www.lyssna.com/blog/cognitive-biases-in-ux/)*

### Framing Techniques

| Frame Type | Example A | Example B (Same Info) | Impact |
|------------|-----------|----------------------|--------|
| **Gain vs Loss** | "Save $50" | "Stop wasting $50/month" | Loss frame +40% |
| **Relative** | "$290" | "$400 ~~$290~~ (Save $110)" | Anchored +25% |
| **Percentage vs Absolute** | "20% off" | "Save $50" | Context-dependent |
| **Positive vs Negative** | "95% satisfied" | "5% complained" | Positive +15% |
| **Per unit** | "$299/year" | "$0.82/day" | Per-day +30% uptake |

### Semantic Reframing Statistics

> "Semantic reframing strategies can influence purchasing decisions by changing how prices are perceived — such as showing daily costs instead of annual, or absolute savings instead of percentages."
>
> *Source: [ResearchGate - Price Reframing Tactics](https://www.researchgate.net/publication/244478492_Consumer_Evaluations_of_Temporal_Reframing_of_Prices)*

### When to Use Each Frame

| Context | Recommended Frame | Rationale |
|---------|-------------------|-----------|
| **High price** | Per-day/unit | Makes cost seem smaller |
| **Discounts <20%** | Absolute ($) | Feels more tangible |
| **Discounts >20%** | Percentage (%) | Looks bigger |
| **Risk communication** | Gain frame | Less anxiety |
| **Action motivation** | Loss frame | Creates urgency |
| **Annual vs monthly** | Monthly for price, annual for savings | Best of both |

### Price Framing Psychology

```
Standard Display:
$29/month

Better (anchoring):
$49/month → $29/month
Save 41%!

Best (full psychology):
────────────────────────────
Most Popular
────────────────────────────
$49/month → $29/month
That's less than $1/day!
✓ Cancel anytime
✓ 30-day money-back guarantee
────────────────────────────
[Start Free Trial]
────────────────────────────
```

---

## Anchoring in Practice

### The Science

> "The 'Anchoring Effect' is a cognitive bias where people rely heavily on the first piece of information they receive. For instance, the first price a user sees can serve as an anchor for their perception of value."
>
> *Source: [ContentBloom](https://contentbloom.com/blog/cognitive-bias-in-ux-designing-for-objective-decision-making/)*

### Strategic Anchor Placement

| Context | Anchor Strategy | Implementation |
|---------|-----------------|----------------|
| **Pricing page** | Show highest tier first | Enterprise → Pro → Basic |
| **Negotiations** | Start high | "Similar services cost $10k+" |
| **Discounts** | Show original price prominently | ~~$500~~ $299 |
| **Value prop** | State the value before price | "Worth $2,000 → Yours for $497" |
| **Comparisons** | Use competitor pricing | "Others charge $99. We're $29" |

### Pricing Page Anchoring

```
┌─────────────────────────────────────────────────────────────────┐
│                                                                 │
│  Enterprise        Pro               Basic                     │
│  $299/mo          $99/mo ★          $29/mo                    │
│  (ANCHOR)         (TARGET)           (Entry)                   │
│                                                                 │
│  Seeing $299 first makes $99 feel like a deal                  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Anchoring + Decoy Effect

Add an inferior option to make the target look better:

```
Basic:        $29/mo   |  5 users
Pro:          $49/mo   |  10 users    ← DECOY (poor value)
Business:     $59/mo   |  50 users    ← TARGET (great value by comparison)
```

The Pro tier is intentionally poor value, making Business look exceptional.

---

## Reciprocity Deep Dive

### The Research

> "In the study, giving diners a single mint at the end of their meal typically increased tips by around 3%. If the gift is doubled and two mints are provided, tips don't double—they quadruple (a 14% increase)."
>
> *Source: [Robert Cialdini via Influence At Work](https://www.influenceatwork.com/7-principles-of-persuasion/)*

### The Three Keys to Effective Reciprocity

> "The key to using the Principle of Reciprocity is to be the first to give and to ensure that what you give is personalized and unexpected."
>
> *Source: [Cognitigence](https://www.cognitigence.com/blog/principle-of-reciprocity-norm)*

| Key | Application | Example |
|-----|-------------|---------|
| **First** | Give before asking | Free tool → then email capture |
| **Personalized** | Tailored to recipient | "Based on your industry..." |
| **Unexpected** | Surprise element | Bonus chapter, unannounced feature |

### Reciprocity Ladder

| Value Given | Ask In Return | Conversion |
|-------------|---------------|------------|
| Blog post (low) | Social share | Low |
| Free guide (medium) | Email address | Medium |
| Free tool (high) | Account creation | High |
| Free consultation (very high) | Sales call | Very high |
| Free trial (highest) | Credit card / Purchase | Highest |

### Implementation Patterns

**Content-to-Email**:
```
Step 1: Valuable blog post (free, no gate)
Step 2: "Want the complete checklist? Enter email"
Step 3: Deliver more value than promised
Step 4: Nurture with valuable content
Step 5: Eventually ask for the sale
```

**Surprise & Delight**:
```
Expected: Order confirmation
Delivered: Order confirmation + surprise 10% off next order

Expected: Basic report
Delivered: Report + bonus analysis + personalized recommendations
```

---

## Implementation Checklist

### Pre-Launch

- [ ] Audit current framing (gain vs loss, anchor placement)
- [ ] Identify peak moments in user journey
- [ ] Map ending experiences for each flow
- [ ] Review choice architecture (defaults, option count)
- [ ] Plan reciprocity sequence

### Quick Wins

- [ ] Add loss-framed alternatives to key headlines
- [ ] Implement "most popular" badge on target pricing tier
- [ ] Pre-select recommended/annual option
- [ ] Add progress indicators to multi-step flows
- [ ] Show stock levels or social proof numbers

### Advanced Implementation

- [ ] A/B test gain vs loss framing on key pages
- [ ] Implement scarcity by product type (demand/supply/time)
- [ ] Design peak moments at key journey points
- [ ] Optimize all ending screens (confirmation, thank you)
- [ ] Build loyalty program with sunk cost mechanics

### Ethical Guardrails

- [ ] All scarcity is based on real limitations
- [ ] Users can easily change defaults
- [ ] No fake urgency (countdown resets, false stock)
- [ ] Transparent pricing (no hidden fees revealed late)
- [ ] Clear cancellation process

---

## Cross-References

- **Basic psychology principles**: See [Psychology](./psychology.md)
- **Pricing psychology**: See [Pricing Patterns](./pricing-patterns.md)
- **FOMO in popups**: See [Popup Optimization](./popup-optimization.md)
- **Trust building**: See [Social Proof Patterns](./social-proof-patterns.md)
- **Testing hypotheses**: See [A/B Testing](./ab-testing.md)

---

## Sources

- [Daniel Kahneman - Thinking, Fast and Slow](https://www.yellowpebble.co/post/daniel-kahnemans-systems-1-and-2-a-b2b-marketing-perspective)
- [BehavioralEconomics.com - Loss Aversion](https://www.behavioraleconomics.com/resources/mini-encyclopedia-of-be/loss-aversion/)
- [The Decision Lab - Hyperbolic Discounting](https://thedecisionlab.com/biases/hyperbolic-discounting)
- [The Decision Lab - Sunk Cost Fallacy](https://thedecisionlab.com/biases/the-sunk-cost-fallacy)
- [The Decision Lab - Nudge Theory](https://thedecisionlab.com/reference-guide/psychology/nudge-theory)
- [Laws of UX - Peak-End Rule](https://lawsofux.com/peak-end-rule/)
- [Nielsen Norman Group - Peak-End Rule](https://www.nngroup.com/articles/peak-end-rule/)
- [CXL - Creating Urgency](https://cxl.com/blog/creating-urgency/)
- [CXL - Cialdini's Principles](https://cxl.com/blog/cialdinis-principles-persuasion/)
- [Convertize - Paradox of Choice](https://www.convertize.com/paradox-of-choice/)
- [Growth.Design - 106 Cognitive Biases](https://growth.design/psychology)
- [Influence At Work - 7 Principles](https://www.influenceatwork.com/7-principles-of-persuasion/)
- [OptinMonster - FOMO Statistics](https://optinmonster.com/fomo-statistics/)
- [HubSpot - Hyperbolic Discounting](https://blog.hubspot.com/sales/hyperbolic-discounting)
- [Lyssna - Cognitive Biases in UX](https://www.lyssna.com/blog/cognitive-biases-in-ux/)
