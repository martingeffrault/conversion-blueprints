# Telehealth Platform Recipe

> **For**: Virtual care platforms, telehealth startups, remote consultation services
> **Key Challenges**: Technology trust, "as good as in-person" perception, privacy concerns, urgency conversion
> **Reference Sites**: Teladoc, Amwell, MDLive, PlushCare, Ro, Hims/Hers

---

## Site Architecture

```
/                         → Homepage (value prop + immediate access)
/how-it-works/            → Process explanation
/services/                → Services/conditions hub
├── /urgent-care/         → Urgent virtual care
├── /primary-care/        → Ongoing care
├── /mental-health/       → Therapy & psychiatry
├── /dermatology/         → Skin care
├── /[specialty]/         → Other specialties
/providers/               → Provider network
/pricing/                 → Cost/insurance info
/for-employers/           → B2B offering (if applicable)
/start-visit/             → Begin consultation (main CTA)
/patient-portal/          → Existing patient access
/faq/                     → Common questions
/privacy/                 → Privacy & HIPAA
/contact/                 → Support
```

---

## Homepage Blueprint

### Section Order

```
1. Hero (Conversion-Focused)
   └── Headline: Immediate value + accessibility
   └── Primary CTA: "Start Visit Now" or "See a Doctor Now"
   └── Trust: "Board-certified doctors" + "Average wait: X minutes"

2. How It Works (3-Step)
   └── Simple visual process
   └── Time expectation ("Done in 15 minutes")
   └── Technology requirements ("Works on any device")

3. What We Treat
   └── Condition grid with icons
   └── Most common conditions prominent
   └── "See full list" for SEO

4. Provider Trust
   └── Provider credentials summary
   └── Sample provider profiles
   └── "All board-certified, licensed in your state"

5. Why Virtual Care
   └── Benefits vs. in-person (convenience, cost, access)
   └── Stats: satisfaction rates, outcomes
   └── Use case scenarios

6. Pricing Transparency
   └── Clear pricing (or "from $X")
   └── Insurance accepted
   └── Employer/health plan coverage

7. Patient Stories
   └── Testimonials emphasizing convenience
   └── Video testimonials if possible
   └── Ratings from app stores

8. Technology Trust
   └── Security badges
   └── HIPAA compliance
   └── Platform screenshots/demo

9. Access CTA
   └── Multiple entry points
   └── 24/7 availability (if applicable)
   └── Emergency disclaimer
```

### Hero Pattern (Urgency-Focused)

```
┌────────────────────────────────────────────────────────────┐
│ HEADER: Logo | How it Works | Services | Pricing | Login | Start Visit │
├────────────────────────────────────────────────────────────┤
│                                                            │
│  See a Doctor in Minutes,                                  │
│  Not Hours                                                 │
│                                                            │
│  Board-certified doctors available 24/7 from your phone,  │
│  tablet, or computer. No appointments necessary.           │
│                                                            │
│  ┌─────────────────────────────────────────────────┐      │
│  │ What's bothering you?                           │      │
│  │ [Cold/Flu ▼] [Other symptoms...]               │      │
│  │                                                 │      │
│  │ [Start My Visit Now →]                         │      │
│  └─────────────────────────────────────────────────┘      │
│                                                            │
│  ⏱️ Avg wait: 7 min  │  ⭐ 4.8/5 rating  │  🔒 HIPAA secure │
│                                                            │
├────────────────────────────────────────────────────────────┤
│ ✓ 24/7 Availability  ✓ All 50 States  ✓ Prescriptions     │
│                         Sent to Your Pharmacy              │
└────────────────────────────────────────────────────────────┘
```

---

## Key Conversion Elements

### Immediate Action Design

Telehealth thrives on "right now" intent. Design for urgency.

**Above Fold Essentials**:
- Primary CTA visible without scroll
- Wait time indicator
- Simple first step (symptom selection)
- No account required to start

### Symptom-Based Entry

```
┌─────────────────────────────────────────────────────┐
│ What can we help you with today?                    │
│                                                     │
│ [🤒 Cold & Flu]  [😷 COVID-19]  [🤕 Allergies]     │
│                                                     │
│ [😰 Anxiety]     [💊 Rx Refill]  [👩‍⚕️ General]    │
│                                                     │
│ [See all conditions →]                             │
└─────────────────────────────────────────────────────┘
```

### Trust Acceleration

Users are skeptical of "online doctors." Overcome quickly.

| Concern | Solution |
|---------|----------|
| "Are these real doctors?" | Photo + credentials of each provider |
| "Is it secure?" | HIPAA badge, encryption messaging |
| "Will I get real help?" | Outcome stats, testimonials |
| "Can they prescribe?" | "Prescriptions sent to your pharmacy" |

---

## Technology & UX Patterns

### Pre-Visit Flow

```
STEP 1: Select Reason                    [1-2 min]
└── Symptom/condition selection
└── Brief questionnaire

STEP 2: Account/Payment                  [2-3 min]
└── Quick registration OR
└── Login existing account
└── Payment (or insurance verification)

STEP 3: Wait for Doctor                  [Show estimated wait]
└── Queue status
└── Option to get callback
└── Pre-visit instructions

STEP 4: Video/Chat Visit                 [5-15 min]
└── Video consult
└── Screen sharing for photos
└── Document upload

STEP 5: After Visit                      [Immediate]
└── Visit summary
└── Prescription sent
└── Follow-up scheduling
```

### Wait Time Display

Critical for user experience:

```
┌─────────────────────────────────────────┐
│ You're in line                          │
│                                         │
│ Estimated wait: 8 minutes               │
│ [████████░░░░░░░░] 3 ahead of you       │
│                                         │
│ While you wait:                         │
│ • Complete your health history          │
│ • Upload any photos                     │
│ • Review your symptoms                  │
│                                         │
│ [Get SMS when it's your turn]          │
└─────────────────────────────────────────┘
```

### Video Consult Interface

```
┌─────────────────────────────────────────────────────────┐
│ [Your Video]                    [Dr. Smith - Expanded] │
│ ┌─────┐                         ┌───────────────────┐  │
│ │ You │                         │                   │  │
│ └─────┘                         │    Doctor's       │  │
│                                 │    Video          │  │
│                                 │                   │  │
│                                 └───────────────────┘  │
├─────────────────────────────────────────────────────────┤
│ [🎤 Mute]  [📷 Camera]  [📎 Share]  [💬 Chat]  [❌ End] │
└─────────────────────────────────────────────────────────┘
```

---

## Pricing Page Patterns

### Transparent Pricing

```
┌─────────────────────────────────────────────────────────┐
│ Simple, Upfront Pricing                                 │
│                                                         │
│ ┌───────────────┐ ┌───────────────┐ ┌───────────────┐  │
│ │  URGENT CARE  │ │  PRIMARY CARE │ │ MENTAL HEALTH │  │
│ │     $75       │ │  $99/month    │ │    $199       │  │
│ │               │ │               │ │               │  │
│ │ Per visit     │ │ Unlimited     │ │ Initial       │  │
│ │ No membership │ │ visits        │ │ session       │  │
│ │               │ │               │ │               │  │
│ │ • Cold & flu  │ │ Everything in │ │ • Therapy     │  │
│ │ • Infections  │ │   Urgent +    │ │ • Psychiatry  │  │
│ │ • Rashes      │ │ • Preventive  │ │ • Counseling  │  │
│ │ • Rx refills  │ │ • Ongoing     │ │               │  │
│ │               │ │ • Specialist  │ │               │  │
│ │               │ │   referrals   │ │               │  │
│ │ [Start Visit] │ │ [Join Now]    │ │ [Book Session]│  │
│ └───────────────┘ └───────────────┘ └───────────────┘  │
│                                                         │
│ Have insurance? Many plans cover telehealth at no cost. │
│ [Check My Coverage]                                     │
└─────────────────────────────────────────────────────────┘
```

### Insurance Integration

```
┌─────────────────────────────────────────────────────────┐
│ Check Your Coverage                                     │
│                                                         │
│ Enter your insurance details to see your cost:         │
│                                                         │
│ Insurance carrier: [Aetna                   ▼]         │
│ Member ID:         [______________________ ]           │
│                                                         │
│ [Check Coverage]                                        │
│                                                         │
│ Accepted insurance:                                     │
│ [Aetna] [Cigna] [UHC] [BCBS] [+50 more]               │
└─────────────────────────────────────────────────────────┘
```

---

## Mobile-First Design

### App Store Presence

Many telehealth platforms are app-first:

```
┌─────────────────────────────────────────────────────────┐
│ Get care from anywhere                                  │
│                                                         │
│ [📱 App Screenshot]                                     │
│                                                         │
│ [Download on App Store]  [Get it on Google Play]       │
│                                                         │
│ Or start now at [platform].com on any browser          │
│                                                         │
│ ⭐⭐⭐⭐⭐ 4.8/5 on App Store (50K+ reviews)            │
└─────────────────────────────────────────────────────────┘
```

### Mobile Web Essentials

- Camera permission flow (for video)
- Simplified forms
- Click-to-call for support
- Browser notification for queue

---

## Specialty-Specific Patterns

### Mental Health

**Different approach needed**:
- Privacy emphasis even stronger
- Therapist matching vs. immediate access
- Ongoing relationship focus
- Stigma-reducing language

**Page modifications**:
```
Hero: "Talk to a therapist this week"
      "Private, confidential, and convenient"

Entry: Questionnaire-based matching
       "Tell us about yourself so we can find your ideal therapist"
```

### Prescription Services (Hims/Ro model)

**Direct-to-consumer health**:
- Condition-specific landing pages
- Subscription model emphasis
- Discreet packaging messaging
- Photo-based diagnosis

```
/erectile-dysfunction/
/hair-loss/
/anxiety/
/birth-control/
```

---

## Conversion Optimization

### Reduce Friction Points

| Friction Point | Solution |
|----------------|----------|
| Account creation | Guest checkout / Google SSO |
| Form length | Progressive disclosure |
| Payment upfront | Insurance check first |
| Privacy concerns | Security messaging throughout |
| Technical issues | Tech check before visit |

### Exit Intent for Healthcare

```
┌─────────────────────────────────────────────────────────┐
│ Still have questions?                                   │
│                                                         │
│ Not sure if telehealth is right for your needs?        │
│ Chat with our care team (human, not a bot).            │
│                                                         │
│ [💬 Chat Now]  [📧 Email Us]  [Continue Browsing]      │
│                                                         │
│ 🔒 Your information stays private.                     │
└─────────────────────────────────────────────────────────┘
```

---

## B2B / Employer Module

If offering to employers:

### Employer Landing Page

```
/for-employers/
├── Value proposition (reduce absenteeism, lower costs)
├── Integration with benefits
├── Case studies with ROI
├── Admin dashboard preview
├── Contact sales CTA
```

### Key B2B Messaging

- "Reduce employee sick days by X%"
- "Lower healthcare costs"
- "24/7 access increases utilization"
- "HIPAA compliant, SOC 2 certified"

---

## Compliance & Trust

### Required Elements

| Element | Placement | Notes |
|---------|-----------|-------|
| HIPAA badge | Header/footer, forms | Clickable to policy |
| State licensing | Footer, provider pages | Where licensed to practice |
| Emergency disclaimer | Every page footer | Cannot replace ER |
| Privacy policy | Footer, form pages | Healthcare-specific |
| Terms of service | Footer | Telehealth-specific terms |
| Prescription limitations | Service pages | What can/cannot prescribe |

### State-Specific Considerations

- Provider licensing varies by state
- "Available in all 50 states" (if true)
- Location detection for availability
- State-specific consent requirements

---

## Metrics to Track

| Metric | Target | Notes |
|--------|--------|-------|
| Visit start rate | >40% | Started intake from homepage |
| Visit completion | >80% | Completed visit once started |
| Wait time satisfaction | >4/5 | Post-visit survey |
| NPS | >50 | Net Promoter Score |
| Rx fill rate | >90% | Prescriptions filled |
| Return visit rate | >30% | Came back within 6 months |
| Employer activation | Varies | B2B metric |

---

## Reference Sites

### Pure Telehealth
- **Teladoc** — Market leader, comprehensive
- **Amwell** — Enterprise focus
- **MDLive** — Cigna-owned, integrated

### Consumer Health Brands
- **Ro** — Men's & women's health
- **Hims/Hers** — DTC health
- **Nurx** — Women's health

### Mental Health Focus
- **Talkspace** — Therapy platform
- **BetterHelp** — Counseling
- **Cerebral** — Psychiatry

### Urgent Care Digital
- **PlushCare** — Primary care focus
- **K Health** — AI-assisted triage

---

*See also: [Healthcare Recipe](./SITE.md) | [Healthcare Industry Patterns](../../library/industry/healthcare.md) | [Trust Elements](../../library/components/trust-elements.md)*
