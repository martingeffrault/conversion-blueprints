# User Testing (Usability Testing) Guide

> **Purpose**: Observe real users interacting with your site to find conversion barriers
> **Impact**: 5-7 participants can reveal 85% of usability issues
> **Principle**: Watch what users do, not just what they say

---

## Why User Testing Matters

### The Cost of Skipping

> "Identifying and resolving issues during the development phase is much costlier because changes are more complex and can disrupt existing code. Addressing problems early in the design phase is more cost-effective and less disruptive."
>
> *Source: [VWO](https://vwo.com/blog/usability-testing-statistics/)*

### Key Statistics

| Insight | Data Point |
|---------|------------|
| Issues found with 5-7 users | ~85% |
| Qualitative test sample | 5-10 participants |
| Quantitative test sample | 20-40 participants |
| Average SUS score benchmark | 68/100 |
| Card sorting participants | 15-30 |

---

## Types of User Testing

### By Moderation

| Type | Description | Best For |
|------|-------------|----------|
| **Moderated** | Researcher guides in real-time | Complex products, deep insights |
| **Unmoderated** | Participants work independently | Scale, cost-efficiency, natural behavior |

> "Moderated testing allows for direct observation, follow-up questions, and in-depth feedback. Unmoderated testing is cost-effective, scalable, and minimizes bias."
>
> *Source: [Full Scale](https://fullscale.io/blog/usability-testing/)*

### By Location

| Type | Pros | Cons |
|------|------|------|
| **In-person** | Body language, tech control | Expensive, limited reach |
| **Remote** | Wider access, convenience | Technical issues, less control |
| **Lab** | Controlled environment | Artificial setting |
| **Field** | Natural context | Distractions, logistics |

### By Approach

| Method | Purpose | Participants |
|--------|---------|--------------|
| **Task-based** | Can users complete key actions? | 5-10 |
| **Think-aloud** | What's the user thinking? | 5-8 |
| **5-Second test** | First impressions | 20-50 |
| **Card sorting** | Information architecture | 15-30 |
| **Tree testing** | Navigation validation | 20-50 |
| **First-click** | Do users start correctly? | 20-50 |
| **Preference test** | A vs B preference | 20-50 |

---

## Planning User Tests

### Test Plan Components

> "A usability testing plan defines clear objectives, methodologies, and expected outcomes. It ensures all stakeholders understand the testing scope, timeline, and resource requirements."
>
> *Source: [UX Tigers](https://www.uxtigers.com/post/user-testing)*

```
USABILITY TEST PLAN

1. Objectives
   └── What questions are we answering?

2. Participants
   ├── Who are we testing with?
   ├── How many participants?
   └── Recruitment criteria

3. Methodology
   ├── Moderated or unmoderated?
   ├── In-person or remote?
   └── Tasks to complete

4. Metrics
   ├── Task completion rate
   ├── Time on task
   ├── Error rate
   └── Satisfaction score

5. Timeline & Resources
   ├── Test dates
   ├── Analysis time
   └── Team responsibilities
```

### Participant Recruitment

| Criteria | Considerations |
|----------|----------------|
| **Demographics** | Age, location, income, role |
| **Behavioral** | Product usage, shopping habits |
| **Technical** | Device, browser, comfort level |
| **Experience** | New vs existing users |

#### Sample Size Guidelines

| Test Type | Participants | Purpose |
|-----------|--------------|---------|
| Qualitative (find issues) | 5-10 per segment | Problem discovery |
| Quantitative (measure) | 20-40 per segment | Statistical comparison |
| Card sorting | 15-30 | IA validation |
| 5-second tests | 20-50 | First impressions |

---

## Writing Test Tasks

### Task Design Principles

| Principle | Example |
|-----------|---------|
| **Realistic** | "Find a gift for your niece's birthday" |
| **Goal-based** | Not "Click the search button" |
| **Non-leading** | Don't mention specific UI elements |
| **Specific** | Clear success criteria |

### Task Examples by Page Type

**Homepage Tasks**
- "What does this company do?"
- "How would you get help if you had a question?"
- "Find the pricing information"

**Product Page Tasks**
- "You need [product]. Find one that fits your needs."
- "Compare these two options and decide which to buy"
- "Add this item to your cart"

**Checkout Tasks**
- "Complete this purchase"
- "Apply this discount code: SAVE20"
- "Change the shipping address"

**Account Tasks**
- "Create an account"
- "Find your order history"
- "Update your payment method"

### Post-Task Questions

| Question Type | Example |
|---------------|---------|
| **Difficulty** | "How easy or difficult was that? (1-5)" |
| **Confidence** | "How confident are you that you completed it correctly?" |
| **Expectation** | "Did the site work as you expected?" |
| **Improvement** | "What would make this easier?" |

---

## Running Test Sessions

### Moderated Session Structure

```
TYPICAL 45-60 MINUTE SESSION

Pre-Session (5 min)
├── Welcome and introduction
├── Explain recording/confidentiality
└── Answer questions

Warm-Up (5 min)
├── Background questions
├── Experience with similar products
└── Comfort level with technology

Tasks (30-40 min)
├── 4-8 tasks
├── Think-aloud protocol
├── Neutral facilitation
└── Probing questions

Wrap-Up (10 min)
├── Overall impressions
├── Post-test questionnaire (SUS)
└── Thank and incentive
```

### Facilitator Best Practices

| Do | Don't |
|----|-------|
| Observe silently | Lead the user |
| Ask "What are you thinking?" | Ask "Why didn't you click X?" |
| Let users struggle (briefly) | Jump in to help immediately |
| Take notes on behavior | Only record verbal feedback |
| Stay neutral | React to success/failure |

### Probing Questions

| Situation | Question |
|-----------|----------|
| User hesitates | "What are you looking for?" |
| User seems confused | "What did you expect to happen?" |
| User makes error | "Walk me through your thinking there" |
| User completes task | "How did that feel?" |
| User expresses frustration | "Tell me more about that" |

---

## Metrics & Measurement

### Core Usability Metrics

| Metric | Measurement | Benchmark |
|--------|-------------|-----------|
| **Task success rate** | % completing task | >78% good |
| **Time on task** | Seconds/minutes | Context-dependent |
| **Error rate** | Errors per task | <1 average |
| **Lostness** | Navigation confusion | Lower is better |
| **Satisfaction** | Post-task rating | >4/5 |

### System Usability Scale (SUS)

> "The SUS has become an industry standard. The average SUS score is 68."
>
> *Source: [Dscout](https://www.dscout.com/people-nerds/11-usability-testing-metrics)*

| Score Range | Interpretation |
|-------------|----------------|
| 85+ | Excellent |
| 68-84 | Good (above average) |
| 51-67 | OK (below average) |
| <51 | Poor |

**SUS Questions** (10 questions, 1-5 scale):
1. I think I would like to use this system frequently
2. I found the system unnecessarily complex
3. I thought the system was easy to use
4. I would need support to use this system
5. I found the functions well integrated
6. I thought there was too much inconsistency
7. Most people would learn this quickly
8. I found the system cumbersome to use
9. I felt confident using the system
10. I needed to learn a lot before getting going

### Task-Level Metrics

| Metric | Calculation |
|--------|-------------|
| **Completion rate** | Successful completions / Total attempts |
| **Efficiency** | Optimal clicks / Actual clicks |
| **Learnability** | Time on task 1 vs task N |
| **Errors** | Critical, non-critical, recovered |

---

## Analyzing Results

### Issue Severity Rating

| Severity | Definition | Action |
|----------|------------|--------|
| **Critical** | Blocks completion, affects many | Fix immediately |
| **Major** | Causes significant difficulty | Fix before launch |
| **Minor** | Causes slight difficulty | Fix when possible |
| **Cosmetic** | Aesthetic or preference | Nice to fix |

### From Observations to Recommendations

> "Reports must propose clear, specific solutions, not just identify issues. 'Users find navigation confusing' is an observation floating in space. 'Change Resources to Help Center since 80% of users looked there for support' is an actionable answer."
>
> *Source: [UX Tigers](https://www.uxtigers.com/post/user-testing)*

| Observation | Issue | Recommendation |
|-------------|-------|----------------|
| 4/5 users missed CTA button | Low visibility | Increase contrast, add whitespace |
| Users clicked logo expecting home | Mental model mismatch | Make logo clickable |
| Average task time 3x expected | High friction | Reduce steps, add progress indicator |
| 60% abandon at form | Form too long | Reduce fields or add progressive disclosure |

### Analysis Framework

```
FOR EACH ISSUE:

1. Observation
   └── What happened? (Behavior)

2. Impact
   ├── How many affected?
   ├── Severity level?
   └── Business impact?

3. Cause
   └── Why did this happen?

4. Recommendation
   ├── Specific change
   ├── Expected improvement
   └── Implementation effort
```

---

## Continuous Testing

### Building a Testing Cadence

> "Teams that make user contact routine (weekly or per sprint) ship better experiences, faster."
>
> *Source: [UX Tigers](https://www.uxtigers.com/post/user-testing)*

| Frequency | Focus |
|-----------|-------|
| **Weekly** | Quick tests on current sprint work |
| **Monthly** | Deeper dive on key flows |
| **Quarterly** | Competitive benchmarking |
| **Major release** | Full usability audit |

### Lightweight Testing Methods

| Method | Time | Cost |
|--------|------|------|
| Hallway testing | 15 min | Free |
| Unmoderated remote | 30 min | $50-100/participant |
| First-click test | 5 min | Minimal |
| 5-second test | 5 min | Minimal |

---

## Tools for User Testing

### Testing Platforms

| Tool | Type | Best For |
|------|------|----------|
| **UserTesting** | Moderated/Unmoderated | Full-service testing |
| **Maze** | Unmoderated | Quick prototype tests |
| **Lookback** | Moderated remote | Live observation |
| **UsabilityHub** | Quick tests | 5-second, first-click |
| **Optimal Workshop** | IA testing | Card sorts, tree tests |
| **Hotjar** | Recordings | Session replays |
| **Dscout** | Mobile diary | In-context research |

### Recording & Analysis

| Tool | Purpose |
|------|---------|
| **Zoom/Teams** | Remote session recording |
| **Loom** | Async video sharing |
| **Dovetail** | Research repository |
| **EnjoyHQ** | Insight management |
| **Notion/Airtable** | Analysis organization |

---

## Accessibility in User Testing

> "Designers have to produce things for all people, regardless of age, ability, or origin. Voice command and screen reader features are now the new standard."
>
> *Source: [Shakuro](https://shakuro.com/blog/usability-testing-methods)*

### Inclusive Testing Practices

| Consideration | Action |
|---------------|--------|
| Screen readers | Test with JAWS, NVDA, VoiceOver |
| Motor impairments | Test keyboard-only navigation |
| Visual impairments | Test with color blindness simulators |
| Cognitive load | Test with diverse cognitive abilities |
| Older adults | Include 55+ participants |

---

## Reporting Results

### Report Structure

```
USABILITY TEST REPORT

1. Executive Summary
   ├── Key findings (3-5)
   ├── Overall usability score
   └── Priority recommendations

2. Methodology
   ├── Participants (n, demographics)
   ├── Tasks tested
   └── Metrics collected

3. Findings by Task
   ├── Success rate
   ├── Common issues
   └── User quotes

4. Prioritized Recommendations
   ├── Critical (fix now)
   ├── Major (fix soon)
   └── Minor (backlog)

5. Appendix
   ├── Full task scripts
   ├── Participant profiles
   └── Raw data
```

### Making Reports Actionable

| Include | Why |
|---------|-----|
| Video clips | Show, don't tell |
| User quotes | Build empathy |
| Specific recommendations | Clear next steps |
| Severity ratings | Prioritization |
| Metrics comparison | Track progress |

---

## Key Takeaways

1. **Start small**: 5 users reveal 85% of issues
2. **Watch behavior**: Actions reveal more than opinions
3. **Stay neutral**: Don't lead participants
4. **Be specific**: "Change X to Y" beats "improve navigation"
5. **Test continuously**: Make user contact routine

---

## Sources

- [UX Tigers - 12 Steps for Usability Testing](https://www.uxtigers.com/post/user-testing)
- [Shakuro - Usability Testing Methods](https://shakuro.com/blog/usability-testing-methods)
- [Full Scale - Ultimate Guide to Usability Testing](https://fullscale.io/blog/usability-testing/)
- [VWO - Usability Testing Statistics](https://vwo.com/blog/usability-testing-statistics/)
- [Contentsquare - Usability Testing Methods](https://contentsquare.com/guides/usability-testing/methods/)
- [Dscout - 11 Usability Testing Metrics](https://www.dscout.com/people-nerds/11-usability-testing-metrics)
- [Looppanel - Usability Testing Guide](https://www.looppanel.com/blog/usability-testing-guide)
