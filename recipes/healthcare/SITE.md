# Healthcare Website Recipe

> **For**: Medical practices, telehealth platforms, health systems, and health tech companies
> **Key Challenges**: Trust & credentialing, HIPAA compliance, patient anxiety reduction, appointment conversion
> **Reference Sites**: Cleveland Clinic, One Medical, Zocdoc, Teladoc, Carbon Health

---

## Site Architecture

### Minimum Viable Site

```
/                     → Homepage (triage to services/conditions)
/services/            → Services hub
/services/[service]/  → Individual service pages
/providers/           → Provider directory
/providers/[name]/    → Individual provider profiles
/locations/           → Location finder
/appointments/        → Book appointment (main conversion)
/patient-portal/      → Patient portal login
/contact/             → Contact & emergency info
```

### Full Healthcare Site

```
/                           → Homepage
/about/                     → About the practice/system
/services/                  → Services hub
├── /primary-care/          → Primary care
├── /specialty-name/        → Specialty services
└── /telehealth/            → Virtual care options
/conditions/                → Conditions we treat (SEO)
├── /condition-name/        → Individual condition pages
/providers/                 → Provider directory
├── /[name]/                → Provider profile
/locations/                 → Location finder
├── /[location]/            → Individual location
/patients/                  → Patient resources hub
├── /new-patients/          → New patient info
├── /insurance/             → Insurance accepted
├── /forms/                 → Patient forms
├── /portal/                → Patient portal
├── /faq/                   → Patient FAQ
/blog/                      → Health articles (SEO)
├── /[article]/             → Individual articles
/appointments/              → Book appointment
/contact/                   → Contact page
/careers/                   → Careers (if applicable)
/privacy/                   → Privacy policy (HIPAA)
```

---

## Homepage Blueprint

### Section Order

```
1. Hero
   └── Value prop + primary CTA (Book/Find Provider)
   └── Trust badges (certifications, awards, ratings)

2. Services Overview
   └── 4-6 primary services with icons
   └── Quick links to most-sought services

3. Why Choose Us
   └── 3-4 differentiators (technology, approach, outcomes)
   └── Credentials bar (board certifications, affiliations)

4. Provider Spotlight
   └── Featured providers with photos
   └── Credentials and specialties
   └── Direct booking buttons

5. Patient Experience
   └── Testimonials (video if possible)
   └── Patient satisfaction scores
   └── Google/Healthgrades ratings

6. Locations
   └── Map with multiple locations
   └── Hours and contact for each
   └── "Find nearest" functionality

7. Insurance & Access
   └── Insurance logos accepted
   └── Self-pay options
   └── Financial assistance info

8. CTA Section
   └── Book appointment
   └── Emergency contact info
   └── Patient portal link

9. Footer
   └── Compliance info (HIPAA, non-discrimination)
   └── Emergency disclaimer
   └── Quick links to key pages
```

### Hero Pattern

```
┌────────────────────────────────────────────────────────┐
│  HEADER: Logo | Services | Providers | Locations | Portal | Book Appt │
├────────────────────────────────────────────────────────┤
│                                                        │
│  [Trust Badges: Board Certified | Accepting Patients]  │
│                                                        │
│  Compassionate Care,                                   │
│  Advanced Medicine                                     │
│                                                        │
│  Subtitle: Primary and specialty care for the whole    │
│  family. In-person and virtual appointments available. │
│                                                        │
│  [Book Appointment]  [Find a Provider]                 │
│                                                        │
│  [4.8★ on Google]  [Healthgrades Recognition]         │
│                                                        │
├────────────────────────────────────────────────────────┤
│ ⚡ New Patients  │ 📍 3 Locations │ 💻 Telehealth    │
│    Welcome       │   [City Name]  │   Available       │
└────────────────────────────────────────────────────────┘
```

---

## Key Pages Deep Dive

### Provider Profile Page

Critical for healthcare — patients choose providers, not just practices.

**Must-Have Elements**:

| Element | Purpose | Placement |
|---------|---------|-----------|
| Professional photo | Trust, human connection | Top, prominent |
| Name & credentials | Authority | Below photo |
| Specialties | Relevance | Above fold |
| Board certifications | Trust | With credentials |
| Education & training | Authority | Expandable section |
| Languages spoken | Accessibility | Quick facts |
| Hospital affiliations | Trust, context | Credentials section |
| Patient ratings | Social proof | Prominent |
| Bio (personal voice) | Connection | Main content |
| Conditions treated | SEO + relevance | Detailed section |
| Locations & hours | Convenience | Sidebar or tabs |
| Book button (sticky) | Conversion | Always visible |

**Profile Layout**:

```
┌─────────────────────────────────────────────────────┐
│ [Photo]   Dr. Sarah Chen, MD, FACP                  │
│           Internal Medicine                          │
│           ★★★★★ 4.9 (127 reviews)                   │
│                                                     │
│           [Book with Dr. Chen]                      │
├─────────────────────────────────────────────────────┤
│ Quick Facts:                                        │
│ • Board Certified: Internal Medicine               │
│ • Education: Stanford Medical School               │
│ • Languages: English, Mandarin                     │
│ • Accepting: New patients                          │
├─────────────────────────────────────────────────────┤
│ About Dr. Chen                                      │
│ [Personal bio in first person...]                  │
├─────────────────────────────────────────────────────┤
│ Conditions Treated    │  Procedures Offered        │
│ • Diabetes            │  • Annual physicals        │
│ • Hypertension        │  • Chronic disease mgmt    │
│ • Heart disease       │  • Preventive care         │
├─────────────────────────────────────────────────────┤
│ Patient Reviews                                     │
│ [Testimonials with verified patient badge]         │
├─────────────────────────────────────────────────────┤
│ Locations & Availability                           │
│ [Calendar widget or location cards]                │
└─────────────────────────────────────────────────────┘
```

### Service/Condition Page

Dual purpose: SEO for condition searches + conversion to appointment.

**Structure**:

```
1. Hero
   └── Condition/service name
   └── "We can help" messaging
   └── Book appointment CTA

2. Overview
   └── What is this condition/service
   └── Symptoms or use cases
   └── When to see a doctor

3. Our Approach
   └── How we diagnose/treat
   └── Technology/methods used
   └── What to expect

4. Provider Specialists
   └── Doctors who treat this
   └── Their specific expertise
   └── Direct booking links

5. Patient Resources
   └── Preparation tips
   └── FAQ
   └── Related conditions

6. Testimonials
   └── Patient stories (condition-specific)

7. CTA
   └── Book appointment
   └── Contact for questions
```

### Appointment Booking Page

The core conversion point. Reduce friction, increase confidence.

**Optimization Principles**:

| Principle | Implementation |
|-----------|----------------|
| Reduce friction | Minimal required fields |
| Build confidence | Show provider before booking |
| Offer flexibility | Multiple appointment types |
| Enable urgency | Show next available |
| Provide alternatives | Phone number if form fails |

**Booking Flow Options**:

**Option A: Provider-First**
```
Select Provider → Select Reason → Select Time → Confirm
```

**Option B: Reason-First** (recommended for specialists)
```
Select Reason/Service → Match to Provider → Select Time → Confirm
```

**Option C: Time-First** (for urgent care)
```
Select Location → Show Next Available → Select → Confirm
```

---

## Trust & Compliance Patterns

### Essential Trust Elements

| Element | Placement | Implementation |
|---------|-----------|----------------|
| Board certifications | Provider pages, about | Verified badges |
| Hospital affiliations | Footer, about | Logo display |
| Insurance accepted | Homepage, dedicated page | Logo carousel |
| Patient ratings | Throughout | Aggregate + individual |
| HIPAA compliance | Forms, footer | Privacy badge |
| Awards/recognition | Homepage, about | Badge display |
| Accreditations | Footer, about | Official logos |

### HIPAA Compliance UI

**Form Requirements**:

- Privacy notice link before submit
- Secure form indicators (lock icon, "Secure Form" badge)
- Clear data usage statement
- Consent checkbox where required

**Example Form Footer**:

```
┌────────────────────────────────────────────────────┐
│ 🔒 Your information is protected                   │
│                                                    │
│ We're committed to protecting your privacy.        │
│ See our [Privacy Policy] and [HIPAA Notice].      │
│                                                    │
│ □ I consent to [practice name] contacting me      │
│   regarding my healthcare.                         │
│                                                    │
│ [Submit Request]                                   │
└────────────────────────────────────────────────────┘
```

### Emergency Disclaimers

Required on healthcare sites:

```
┌────────────────────────────────────────────────────┐
│ ⚠️ Medical Emergency?                              │
│ If you're experiencing a medical emergency,        │
│ call 911 or go to your nearest emergency room.    │
│                                                    │
│ This website does not provide emergency services.  │
└────────────────────────────────────────────────────┘
```

---

## Copywriting Framework: CARE

Healthcare-specific framework for patient communication.

### C - Compassion

Lead with understanding, not clinical language.

| Instead of | Use |
|------------|-----|
| "Symptom management" | "Relief for what you're experiencing" |
| "Patient intake" | "Getting to know you" |
| "Diagnose and treat" | "Understand and help" |

### A - Authority

Establish credibility without intimidation.

**Good**: "Dr. Chen has 15 years of experience and has helped thousands of patients manage their diabetes."

**Avoid**: "Dr. Chen is a leading expert in endocrinology with publications in multiple peer-reviewed journals..."

### R - Reassurance

Address the anxiety inherent in healthcare decisions.

**Include**:
- What to expect language
- "You're in good hands" messaging
- Outcome statistics when available
- Patient testimonials

### E - Ease

Make taking action feel simple.

**Simplify**:
- "Book in 60 seconds"
- "Same-day appointments available"
- "We handle insurance for you"
- "Easy online check-in"

---

## Patient Journey Mapping

### New Patient Journey

```
AWARENESS                    CONSIDERATION              DECISION
    │                             │                        │
    ▼                             ▼                        ▼
Searches "doctor              Visits website           Books appointment
near me" or symptom           Reviews providers        Confirms details
                              Checks insurance
                              Reads reviews

TOUCHPOINTS:                  TOUCHPOINTS:             TOUCHPOINTS:
• Google listing             • Homepage               • Booking form
• Healthgrades               • Provider profiles      • Confirmation email
• Referral                   • Insurance page         • Pre-visit info
• Blog content               • Patient reviews

OPTIMIZE:                    OPTIMIZE:                OPTIMIZE:
• Local SEO                  • Provider pages         • Form simplicity
• Review management          • Trust signals          • Confirmation clarity
• Content for symptoms       • Clear navigation       • Pre-visit prep
```

### Returning Patient Journey

```
NEED                         ACCESS                    ENGAGE
  │                            │                         │
  ▼                            ▼                         ▼
Needs appointment          Uses patient portal       Completes visit
or information             or booking system         Receives follow-up

TOUCHPOINTS:               TOUCHPOINTS:              TOUCHPOINTS:
• Email reminder           • Portal login            • Post-visit summary
• Direct phone             • Mobile app              • Prescription info
• Website return           • Online scheduling       • Follow-up booking

OPTIMIZE:                  OPTIMIZE:                 OPTIMIZE:
• Easy portal access       • Simplified login        • Clear summaries
• Prominent phone          • Quick rebooking         • Easy follow-up
• Saved preferences        • Appointment history     • Wellness content
```

---

## Mobile Optimization

Healthcare has high mobile usage (60%+ in many markets).

### Mobile Priorities

| Priority | Implementation |
|----------|----------------|
| Click-to-call | Sticky phone button |
| Quick booking | Simplified mobile form |
| Location/directions | Maps integration |
| Provider photos | Optimized images |
| Portal access | Prominent login |
| Emergency info | Always visible |

### Mobile Header Pattern

```
┌────────────────────────────────────────────┐
│ [Logo]              [☰ Menu]  [📞 Call]   │
└────────────────────────────────────────────┘

[Sticky bottom bar on scroll:]
┌────────────────────────────────────────────┐
│ [📞 Call]    [📅 Book]    [📍 Locations] │
└────────────────────────────────────────────┘
```

---

## Conversion Optimization

### Healthcare-Specific CTAs

| Action | Primary CTA | Secondary CTA |
|--------|-------------|---------------|
| New patient | "Book Appointment" | "Call to Schedule" |
| Existing patient | "Patient Portal" | "Request Refill" |
| Research phase | "Find a Provider" | "Learn About [Condition]" |
| Urgent need | "See Next Available" | "Virtual Visit Now" |

### Form Optimization

**Minimum Fields** (initial contact):
- Name
- Phone or email
- Reason for visit (dropdown)
- Preferred provider (optional)
- Insurance (optional at first touch)

**Progressive Collection**:
Collect additional info after initial contact:
- Full demographics
- Insurance details
- Medical history
- Consent forms

---

## SEO Strategy

### Content Pillars

| Pillar | Content Type | Keywords Target |
|--------|--------------|-----------------|
| Conditions | Detailed guides | "[condition] symptoms/treatment" |
| Providers | Profile pages | "[specialty] doctor near me" |
| Locations | Location pages | "[city] [specialty]" |
| Services | Service pages | "[procedure/service] near me" |
| Wellness | Blog content | Health questions, prevention |

### Local SEO Critical

- Google Business Profile optimization
- Location pages with unique content
- Review generation and management
- Local schema markup

### Schema Markup Required

```
- LocalBusiness / MedicalBusiness
- Physician schema
- MedicalCondition schema
- FAQPage schema
- Review schema
```

---

## Technology Requirements

### Integrations

| System | Purpose | Priority |
|--------|---------|----------|
| EHR/EMR | Patient records | Essential |
| Scheduling system | Online booking | Essential |
| Patient portal | Secure access | Essential |
| Telehealth platform | Virtual visits | High |
| Payment processing | Bill pay | High |
| Review platform | Reputation | Medium |
| Marketing automation | Nurturing | Medium |

### Compliance Requirements

| Requirement | Implementation |
|-------------|----------------|
| HIPAA | Secure forms, BAA with vendors, encryption |
| ADA | Full accessibility compliance |
| SSL | Site-wide HTTPS |
| Privacy Policy | Healthcare-specific language |
| Cookie consent | If using tracking |

---

## Reference Sites to Study

### Health Systems
- **Cleveland Clinic** — World-class content, clean navigation
- **Mayo Clinic** — Patient education excellence
- **Kaiser Permanente** — Integrated experience

### Modern Medical Practices
- **One Medical** — Consumer-friendly healthcare
- **Carbon Health** — Modern urgent care
- **Forward** — Tech-forward primary care

### Telehealth
- **Teladoc** — Virtual care leader
- **Amwell** — Enterprise telehealth
- **PlushCare** — Consumer virtual care

### Healthcare Marketplaces
- **Zocdoc** — Provider discovery/booking
- **Healthgrades** — Provider ratings

---

## Variants

### Multi-Location Health System

Additional pages needed:
- System overview page
- Location comparison tool
- Centralized provider directory
- Service line landing pages

### Single Provider Practice

Simplified structure:
- Provider IS the brand (personal homepage)
- Fewer navigation items
- More personal approach
- Direct contact emphasis

### Telehealth-First

Emphasize:
- Technology ease ("works on any device")
- Privacy and security
- How virtual visits work
- When in-person needed

---

*See also: [Healthcare Industry Patterns](../../library/industry/healthcare.md) | [Trust Elements](../../library/components/trust-elements.md) | [Form Optimization](../../library/conversion/form-optimization.md)*
