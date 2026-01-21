# Legal Compliance for Websites

> **Purpose**: Understand and implement legal requirements for websites
> **Scope**: Privacy (GDPR, CCPA), accessibility (ADA), cookie consent, disclosures
> **Disclaimer**: This is educational guidance — consult legal counsel for compliance

---

## Privacy Regulations

### GDPR (General Data Protection Regulation)

**Scope**: EU residents' data, regardless of business location

**Key Requirements**:

| Requirement | Description |
|-------------|-------------|
| Lawful basis | Need legitimate reason to collect data |
| Consent | Must be freely given, specific, informed, unambiguous |
| Right to access | Users can request their data |
| Right to deletion | Users can request data deletion |
| Right to portability | Users can export their data |
| Data breach notification | 72-hour notification requirement |
| Privacy by design | Build privacy into systems |

**Lawful Bases for Processing**:
1. **Consent** — User explicitly agrees
2. **Contract** — Necessary for contract performance
3. **Legal obligation** — Required by law
4. **Vital interests** — Protect someone's life
5. **Public task** — Official authority function
6. **Legitimate interests** — Business interest (balanced against user rights)

**Cookie Consent Requirements**:
- Cookies blocked until consent given
- Easy to accept AND reject
- Granular options (necessary, analytics, marketing)
- Easy to withdraw consent
- Record of consent

**Privacy Policy Must Include**:
- Identity of data controller
- What data is collected
- How data is used
- Legal basis for processing
- Data retention periods
- Third parties receiving data
- User rights and how to exercise them
- Right to lodge complaint with authority

**GDPR Fines**:
- Up to €20 million or 4% of global annual revenue (whichever is higher)

### CCPA (California Consumer Privacy Act)

**Scope**: California residents, businesses meeting thresholds

**Thresholds** (any one of):
- Annual gross revenue > $25 million
- Buy/sell/share 100,000+ California residents' data
- 50%+ revenue from selling personal information

**Key Requirements**:

| Right | Description |
|-------|-------------|
| Right to know | What data is collected and how used |
| Right to delete | Request deletion of personal data |
| Right to opt-out | Opt out of data sale |
| Right to non-discrimination | Can't penalize for exercising rights |

**Required Disclosures**:
- Categories of personal info collected
- Purposes for collection
- Categories of third parties shared with
- Specific pieces of personal info collected
- Whether personal info is sold

**"Do Not Sell My Personal Information"**:
- Clear, conspicuous link on homepage
- Cannot require account creation to opt out
- Process requests within 45 days

### CPRA (California Privacy Rights Act)

**Updates to CCPA** (effective 2023):
- New category: sensitive personal information
- Right to correct inaccurate information
- Right to limit use of sensitive info
- Data minimization requirements
- Purpose limitation requirements

### Other Privacy Regulations

| Regulation | Region | Key Points |
|------------|--------|------------|
| **LGPD** | Brazil | Similar to GDPR |
| **PIPEDA** | Canada | Consent-based, reasonable purposes |
| **UK GDPR** | UK | Post-Brexit GDPR equivalent |
| **POPIA** | South Africa | GDPR-like framework |

---

## Accessibility Law

### ADA (Americans with Disabilities Act)

**Scope**: "Places of public accommodation" — includes websites

**Key Points**:
- No explicit technical standard in law
- Courts increasingly apply WCAG 2.1 AA
- Applies to businesses open to the public
- No safe harbor — lawsuits can occur anytime

**ADA Lawsuit Trends**:
- 4,000+ lawsuits per year
- Retail, food service, hospitality most targeted
- Settlements range from $10,000 to $100,000+

### Section 508

**Scope**: US federal agencies and contractors

**Requirements**:
- WCAG 2.0 AA compliance
- Applies to all electronic content
- Includes documents, software, websites

### European Accessibility Act (EAA)

**Scope**: Products and services in EU (effective 2025)

**Covered Services**:
- E-commerce websites
- Banking services
- E-books
- Transport services
- Telecommunications

**Requirements**:
- WCAG 2.1 AA equivalent
- EN 301 549 standard

### Other Accessibility Laws

| Law | Region | Standard |
|-----|--------|----------|
| **AODA** | Ontario, Canada | WCAG 2.0 AA |
| **ACA** | Canada (federal) | WCAG 2.1 AA |
| **Equality Act 2010** | UK | Reasonable adjustments |
| **DDA** | Australia | WCAG 2.0 AA |

---

## Cookie Consent Implementation

### Cookie Categories

| Category | Description | Consent Required |
|----------|-------------|------------------|
| **Strictly Necessary** | Essential for site function | No |
| **Functional** | Enhanced features, preferences | Yes (GDPR) |
| **Analytics** | Usage statistics | Yes |
| **Marketing** | Advertising, tracking | Yes |

### Cookie Banner Requirements

**GDPR-Compliant Banner**:

| Requirement | Description |
|-------------|-------------|
| Pre-consent blocking | Non-essential cookies blocked until consent |
| Clear options | Accept all / Reject all / Customize |
| Granular control | Choose by category |
| Easy withdrawal | Easy access to change preferences |
| No dark patterns | Reject must be as easy as accept |
| Record keeping | Store proof of consent |

**Banner Elements**:
1. Clear purpose explanation
2. Link to cookie policy
3. Accept all button
4. Reject all button (equally prominent)
5. Customize preferences option
6. List of cookie categories

**Example Banner Structure**:
```
┌─────────────────────────────────────────────────────────────────┐
│  🍪 We use cookies                                              │
│                                                                 │
│  We use cookies to enhance your experience. You can accept      │
│  all cookies or customize your preferences.                     │
│                                                                 │
│  [Learn more]                                                   │
│                                                                 │
│  ☑ Necessary (always active)                                   │
│  ☐ Analytics                                                   │
│  ☐ Marketing                                                   │
│                                                                 │
│  [Reject All]  [Accept Selected]  [Accept All]                 │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Cookie Policy Contents

- What cookies are used
- Purpose of each cookie
- First-party vs third-party
- Duration/expiry
- How to manage/delete cookies
- Third-party links for their policies

---

## Required Legal Pages

### Privacy Policy

**Must Include**:
- Business identity and contact
- Data collected and purposes
- Legal basis (GDPR)
- Data sharing and recipients
- Data retention periods
- User rights
- Security measures
- International transfers
- Children's privacy (if applicable)
- Changes notification process
- Effective date

### Terms of Service

**Should Include**:
- Acceptance of terms
- Use of service
- User accounts and responsibilities
- Intellectual property rights
- Prohibited activities
- Content ownership
- Disclaimers and warranties
- Limitation of liability
- Indemnification
- Termination
- Governing law
- Dispute resolution
- Changes to terms
- Contact information

### Cookie Policy

**Should Include**:
- What cookies are
- Types of cookies used (see categories)
- Specific cookies (name, purpose, duration)
- Third-party cookies
- How to manage cookies
- Consent mechanism
- Updates to policy

### Accessibility Statement

**Should Include**:
- Commitment to accessibility
- Standards followed (WCAG 2.1 AA)
- Known limitations
- Feedback mechanism
- Contact information
- Third-party content disclaimer
- Update date

**Example Statement**:
```
Accessibility Statement

[Company Name] is committed to ensuring digital accessibility
for people with disabilities. We continually improve the user
experience for everyone and apply relevant accessibility standards.

Standards: We aim to conform to WCAG 2.1 Level AA.

Feedback: If you encounter accessibility barriers, please contact
us at accessibility@company.com. We take your feedback seriously.

Last updated: [Date]
```

---

## E-Commerce Compliance

### Required Disclosures

| Disclosure | Requirement |
|------------|-------------|
| Business identity | Legal name, address, contact |
| Pricing | Total price including taxes |
| Shipping | Costs and delivery times |
| Returns | Policy clearly stated |
| Payment methods | Accepted forms of payment |
| Terms of sale | Before purchase completion |

### Consumer Rights

**Right of Withdrawal (EU)**:
- 14-day cooling-off period
- Full refund within 14 days of return
- Must inform customers of this right
- Exceptions: custom goods, perishables, digital content

**Pricing Requirements**:
- Show total price
- Include all taxes
- Show currency
- No hidden fees at checkout

### Payment Security

**PCI DSS Compliance**:
- Secure cardholder data
- Maintain secure systems
- Implement access controls
- Monitor and test networks
- Information security policy

---

## Affiliate Disclosure Requirements

### FTC Guidelines (US)

**Requirement**: Clear and conspicuous disclosure of material connections

**Must Disclose**:
- Affiliate relationships
- Compensation for reviews
- Free products received
- Employee relationships

**Disclosure Placement**:
- Before affiliate links
- Near the top of content
- Cannot be hidden in footer only
- Must be visible without clicking

**Example Disclosures**:
```
"This article contains affiliate links. If you make a purchase, we may
earn a commission at no extra cost to you."

"Disclosure: We received this product for free in exchange for a review.
All opinions are our own."

"Sponsored post: This content is sponsored by [Brand]."
```

### ASA Guidelines (UK)

Similar to FTC:
- Use #ad for social media
- Clear "Advertisement" labels
- Conspicuous disclosure

---

## Email Marketing Compliance

### CAN-SPAM (US)

| Requirement | Description |
|-------------|-------------|
| No deceptive headers | From, To, Reply-To must be accurate |
| No deceptive subject | Must reflect content |
| Identify as ad | If applicable |
| Physical address | Include valid postal address |
| Opt-out mechanism | Honor within 10 business days |
| No purchased lists | With opted-in requirement |

### GDPR Email Requirements

- Prior consent required (not opt-out)
- Easy unsubscribe in every email
- Record of consent
- Purpose limitation

### CASL (Canada)

- Express consent required
- Clear identification
- Contact information
- Unsubscribe mechanism
- 10-day opt-out processing

---

## Compliance Checklist

### Privacy
- [ ] Privacy policy published and accessible
- [ ] Data processing lawfully based
- [ ] User consent properly collected
- [ ] Data subject rights processes in place
- [ ] Data breach procedures documented
- [ ] International transfer safeguards (if applicable)

### Cookies
- [ ] Cookie consent banner implemented
- [ ] Non-essential cookies blocked until consent
- [ ] Granular consent options provided
- [ ] Cookie policy published
- [ ] Consent records stored

### Accessibility
- [ ] WCAG 2.1 AA compliance
- [ ] Accessibility statement published
- [ ] Feedback mechanism in place
- [ ] Regular accessibility audits

### E-Commerce
- [ ] Clear pricing displayed
- [ ] Return policy visible
- [ ] Terms of sale before checkout
- [ ] Secure payment processing
- [ ] Consumer rights information

### Email
- [ ] Consent before marketing emails
- [ ] Unsubscribe in every email
- [ ] Physical address included
- [ ] Opt-outs honored promptly

### Disclosures
- [ ] Affiliate relationships disclosed
- [ ] Sponsored content labeled
- [ ] Material connections clear

---

## Disclaimer

> **This document provides educational guidance only and does not constitute legal advice. Compliance requirements vary by jurisdiction, business type, and specific circumstances. Consult with qualified legal counsel to ensure your website meets all applicable legal requirements.**

---

## Sources

- [GDPR Official Text](https://gdpr-info.eu/)
- [California Attorney General - CCPA](https://oag.ca.gov/privacy/ccpa)
- [FTC Endorsement Guides](https://www.ftc.gov/business-guidance/resources/ftcs-endorsement-guides)
- [W3C WCAG 2.1](https://www.w3.org/TR/WCAG21/)
- [ADA.gov](https://www.ada.gov/)
- [ICO UK GDPR Guidance](https://ico.org.uk/for-organisations/guide-to-data-protection/guide-to-the-general-data-protection-regulation-gdpr/)
- [CNIL (French DPA)](https://www.cnil.fr/en)
