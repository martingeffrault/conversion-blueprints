# Testing & Experimentation Library

> **Purpose**: Data-driven methodologies for validating assumptions, optimizing conversions, and making informed decisions through systematic testing.

---

## Why Testing Matters

Without testing, you're guessing. With testing, you're learning.

> "Only about 33% of A/B tests produce statistically significant winners—but A/B tests help make a clearly right decision 66% of the time."
>
> *Source: [Analytics-Toolkit](https://blog.analytics-toolkit.com/2022/what-can-be-learned-from-1001-a-b-tests/)*

### Testing ROI

| Metric | Impact | Source |
|--------|--------|--------|
| Companies using A/B testing | 60% (34% more planning to) | VWO |
| Tests stopped before significance | 80% | Industry research |
| Typical test win rate | 10-33% | Multiple sources |
| Median lift from winning tests | 7.5% | Analytics-Toolkit |
| Companies running 2+ tests/month | 71% | Convert |

---

## Testing Framework Overview

### The Testing Stack

```
1. A/B TESTING
   └── Compare two versions to find winners
   └── [ab-testing.md](ab-testing.md)

2. MULTIVARIATE TESTING
   └── Test multiple variables simultaneously
   └── [multivariate.md](multivariate.md)

3. USER TESTING
   └── Qualitative feedback on experiences
   └── [user-testing.md](user-testing.md)

4. HEATMAP ANALYSIS
   └── Visual behavior analysis
   └── [heatmaps.md](heatmaps.md)
```

---

## Quick Start: Which Testing Method?

### By Goal

| Goal | Testing Method | When to Use |
|------|---------------|-------------|
| **Validate a specific change** | A/B Test | Clear hypothesis, sufficient traffic |
| **Find optimal combination** | Multivariate | Multiple elements to test together |
| **Understand user behavior** | User Testing | Qualitative insights needed |
| **See where users click** | Heatmap Analysis | Behavior visualization |

### By Traffic Level

| Monthly Visitors | Recommended Approach |
|-----------------|---------------------|
| **<10,000** | Focus on qualitative research, big changes only |
| **10,000-50,000** | A/B test major changes, 2-4 week durations |
| **50,000-500,000** | Regular A/B testing program possible |
| **500,000+** | Full experimentation program, multivariate viable |

---

## Testing Files

| File | Description |
|------|-------------|
| [ab-testing.md](ab-testing.md) | Complete A/B testing methodology |
| [multivariate.md](multivariate.md) | Multivariate testing guide |
| [user-testing.md](user-testing.md) | User testing protocols |
| [heatmaps.md](heatmaps.md) | Heatmap analysis guide |

---

## Key Principles

### 1. Statistical Rigor

> "Peeking at ongoing experiments inflates Type I error rates. After 2000 samples with continuous peeking, there is a combined 55% chance of incorrectly concluding one variation is better."
>
> *Source: [Evan Miller](https://www.evanmiller.org/how-not-to-run-an-ab-test.html)*

### 2. Test Big Changes First

Start with high-impact changes that can show significant results with smaller sample sizes.

### 3. Document Everything

Every test teaches something—even the losers. Build a knowledge base.

### 4. Prioritize Ruthlessly

Use frameworks like PXL to focus on tests most likely to impact the business.

---

## Sources

- [VWO - A/B Testing Statistics](https://vwo.com/blog/ab-testing-statistics/)
- [CXL - A/B Test Calculator](https://cxl.com/ab-test-calculator/)
- [Evan Miller - How Not to Run an A/B Test](https://www.evanmiller.org/how-not-to-run-an-ab-test.html)
- [Analytics-Toolkit - What Can Be Learned from 1001 A/B Tests](https://blog.analytics-toolkit.com/2022/what-can-be-learned-from-1001-a-b-tests/)
- [Convert - A/B Testing Stats](https://www.convert.com/blog/a-b-testing/ab-testing-stats/)
