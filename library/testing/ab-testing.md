# A/B Testing Methodology

> **Purpose**: Run statistically valid experiments to make data-driven decisions about website changes.
> **Time investment**: 2-6 weeks per test (minimum 2 weeks)
> **Output**: Validated learnings that compound over time

---

## What is A/B Testing?

A/B testing (split testing) compares two versions of a page or element to determine which performs better against a defined metric. It's the gold standard for validating changes before full rollout.

> "60% of companies already use A/B testing and another 34% plan to use it, making it the number one method used by marketers to optimize conversion rates."
>
> *Source: [VWO](https://vwo.com/blog/ab-testing-statistics/)*

### Why A/B Test?

| Benefit | Description |
|---------|-------------|
| **Reduce risk** | Validate changes before full implementation |
| **Data-driven decisions** | Remove opinion from optimization |
| **Compound learning** | Each test builds institutional knowledge |
| **Measurable ROI** | Quantify impact of changes |

### Success Rate Reality

| Metric | Value | Source |
|--------|-------|--------|
| Tests with significant winners | ~33% | Analytics-Toolkit |
| Median lift from winners | 7.5% | Analytics-Toolkit |
| Mean lift from winners | 15.9% | Analytics-Toolkit |
| Mature site win rate | 10-20% | [VWO](https://vwo.com/blog/ab-testing-statistics/) |
| New optimization win rate | 25-33% | [Convert](https://www.convert.com/blog/a-b-testing/ab-testing-stats/) |

> "While tests only win 33% of the time, A/B tests help make a clearly right decision about 66% of the time—shipping a product that won (33%) is a win, but so is not shipping a product that lost (another 33%)."
>
> *Source: [GrowthBook](https://docs.growthbook.io/open-guide-to-ab-testing.v1.0.pdf)*

---

## Statistical Foundations

### Key Concepts

| Concept | Definition | Standard Value |
|---------|------------|----------------|
| **Statistical Significance** | Confidence that result isn't random | 95% (p < 0.05) |
| **Statistical Power** | Probability of detecting real effect | 80% |
| **Minimum Detectable Effect (MDE)** | Smallest lift you can reliably detect | 5-20% relative |
| **Sample Size** | Number of visitors per variation | Calculated |
| **False Positive Rate** | Chance of seeing effect that isn't there | 5% (at 95% confidence) |
| **False Negative Rate** | Chance of missing real effect | 20% (at 80% power) |

### The Sample Size Formula

Sample size depends on:
1. **Baseline conversion rate** - Higher = smaller sample needed
2. **Minimum detectable effect** - Smaller effect = larger sample needed
3. **Statistical significance** - Higher confidence = larger sample
4. **Statistical power** - Higher power = larger sample

> "If the MDE drops from 8% to 7%, the sample size requirement increases significantly. The smaller the effect size, the larger the sample size needed."
>
> *Source: [Cro Metrics](https://crometrics.com/blog/ab-testing-sample-size/)*

### Sample Size Reference Table

| Baseline CVR | 10% MDE | 5% MDE | 2% MDE |
|--------------|---------|--------|--------|
| 1% | 39,000 | 156,000 | 976,000 |
| 3% | 13,000 | 51,000 | 320,000 |
| 5% | 7,600 | 31,000 | 192,000 |
| 10% | 3,600 | 15,000 | 92,000 |
| 20% | 1,700 | 6,700 | 42,000 |

*Per variation, at 95% confidence and 80% power*

### Recommended Calculators

- [Optimizely Sample Size Calculator](https://www.optimizely.com/sample-size-calculator/)
- [CXL A/B Test Calculator](https://cxl.com/ab-test-calculator/)
- [AB Tasty Calculator](https://www.abtasty.com/sample-size-calculator/)
- [Speero A/B Test Calculator](https://speero.com/ab-test-calculator)

---

## The Peeking Problem

The most common mistake in A/B testing is "peeking"—checking results before the test reaches required sample size.

> "Repeated significance testing always increases the rate of false positives. If you peek at an ongoing experiment ten times, what you think is 1% significance is actually just 5% significance."
>
> *Source: [Evan Miller](https://www.evanmiller.org/how-not-to-run-an-ab-test.html)*

### Why Peeking Fails

| Peeking Behavior | Actual False Positive Rate |
|------------------|---------------------------|
| No peeking (proper test) | 5% |
| Weekly peeking | 15-20% |
| Daily peeking | 25-35% |
| Continuous monitoring | 40-55% |

> "After 2000 samples with continuous peeking, there is a combined 55% chance of incorrectly concluding that one variation is better than the other—over five times the expected false positive rate."
>
> *Source: [Lucidchart](https://www.lucidchart.com/blog/the-fatal-flaw-of-ab-tests-peeking)*

### Solutions to Peeking

1. **Pre-calculate duration** - Commit to running for X weeks
2. **Sequential testing** - Use methods designed for continuous monitoring
3. **Bayesian testing** - Different statistical approach without peeking penalty
4. **Lock yourself out** - Literally don't look until completion

---

## The Multiple Testing Problem

Testing many metrics or variations inflates false positive rates.

> "If you test the same hypothesis at a 5% level of significance for 20 different metrics, the probability of finding at least one statistically significant result by chance alone is around 64%."
>
> *Source: [GrowthBook](https://docs.growthbook.io/using/experimentation-problems)*

### Correction Methods

| Method | Description | When to Use |
|--------|-------------|-------------|
| **Bonferroni correction** | Divide alpha by number of tests | Conservative, few metrics |
| **Benjamini-Hochberg** | Controls false discovery rate | Many metrics |
| **Pre-register primary metric** | Declare one metric that matters | Best practice |

### Best Practice

1. Define ONE primary metric before test starts
2. Pre-register secondary metrics (insights only)
3. Apply correction if multiple comparisons required

---

## Test Duration Guidelines

### Minimum Duration Rules

> "Even with sufficient traffic, run your A/B test for at least 1-2 weeks to account for potential fluctuations in user behavior."
>
> *Source: [Guess the Test](https://guessthetest.com/calculating-sample-size-in-a-b-testing-everything-you-need-to-know/)*

| Rule | Minimum Duration |
|------|------------------|
| Baseline | 2 weeks (capture day-of-week variation) |
| E-commerce | Full business cycle (often 4 weeks) |
| B2B | 3-4 weeks (longer decision cycles) |
| With promotions | Extend past promotional period |

### Maximum Duration

> "The ideal testing time period is generally between 2-6 weeks. Anything longer and other factors may start to confound and muddy test results."
>
> *Source: [Statsig](https://www.statsig.com/perspectives/ab-testing-methodology)*

**Stop tests after 6 weeks because:**
- External factors change (seasonality, competitors, market)
- History effects contaminate results
- Opportunity cost of not testing something else

---

## Hypothesis Framework

### The Hypothesis Formula

```
If [we change X]
For [audience Y]
Then [metric Z will improve]
Because [reasoning based on evidence]
```

### Good vs. Bad Hypotheses

| Bad Hypothesis | Good Hypothesis |
|---------------|-----------------|
| "A bigger button will increase clicks" | "If we increase CTA size from 40px to 60px on mobile product pages, we'll increase add-to-cart clicks by 10% because heatmaps show 40% of users miss the current button" |
| "Red converts better than blue" | "If we change the CTA from blue to high-contrast orange on the pricing page, sign-ups will increase by 5% because the current button doesn't meet WCAG contrast ratios" |
| "Social proof helps conversions" | "If we add 3 customer testimonials above the fold on the landing page, trial starts will increase by 15% because user interviews revealed trust is the #1 barrier" |

### Hypothesis Sources

1. **Analytics** - Where are drop-offs happening?
2. **Heatmaps** - What are users clicking (or missing)?
3. **User interviews** - What do customers say?
4. **Support tickets** - What confuses people?
5. **Competitor analysis** - What are others doing?
6. **Best practices** - What does research recommend?

---

## Prioritization Frameworks

### PIE Framework (Chris Goward)

| Factor | Question | Scale |
|--------|----------|-------|
| **P**otential | How much improvement is possible? | 1-10 |
| **I**mportance | How valuable is this traffic? | 1-10 |
| **E**ase | How easy is implementation? | 1-10 |

*Score = Average of P + I + E*

**Pros**: Simple, fast
**Cons**: Highly subjective

### ICE Framework (Sean Ellis)

| Factor | Question | Scale |
|--------|----------|-------|
| **I**mpact | What's the potential impact? | 1-10 |
| **C**onfidence | How sure are you it will work? | 1-10 |
| **E**ase | How easy to implement? | 1-10 |

*Score = I × C × E*

**Pros**: Accounts for confidence
**Cons**: Still subjective

### PXL Framework (CXL)

More rigorous, uses binary (yes/no) scoring:

| Factor | Question | Points |
|--------|----------|--------|
| Above the fold? | Yes/No | +2 |
| Noticeable in 5 seconds? | Yes/No | +2 |
| Adding/removing element? | Yes/No | +2 |
| Running on high-traffic page? | Yes/No | +2 |
| Addressing known problem? | Yes/No | +2 |
| Based on user feedback? | Yes/No | +1 |
| Based on qualitative research? | Yes/No | +1 |
| Based on quantitative data? | Yes/No | +1 |
| Ease of implementation | Low/Med/High | +3/+2/+1 |

> "PXL was developed to eliminate as much subjectivity as possible while maintaining customizability."
>
> *Source: [CXL](https://cxl.com/blog/better-way-prioritize-ab-tests/)*

### Framework Comparison

| Framework | Subjectivity | Complexity | Best For |
|-----------|--------------|------------|----------|
| PIE | High | Low | Quick prioritization |
| ICE | High | Low | Growth experiments |
| PXL | Low | Medium | CRO programs |

---

## Test Documentation Template

### Pre-Test

```markdown
## Test Name: [Descriptive name]

### Hypothesis
If [change]
For [audience]
Then [metric] will [improve/decrease] by [expected %]
Because [evidence-based reasoning]

### Test Details
- **Page/Element**: [URL or element description]
- **Primary Metric**: [Single metric that matters]
- **Secondary Metrics**: [Other metrics to watch]
- **Audience**: [All users / segment]
- **Traffic Split**: [50/50 recommended]

### Variations
- **Control (A)**: [Description of current state]
- **Variant (B)**: [Description of change]

### Technical Requirements
- **Implementation Effort**: [Low/Medium/High]
- **Dev Resources Needed**: [None/Frontend/Backend]
- **Tracking Required**: [Events to set up]

### Calculations
- **Baseline Conversion Rate**: [X%]
- **Minimum Detectable Effect**: [X%]
- **Required Sample Size**: [X per variation]
- **Estimated Duration**: [X weeks]
- **Start Date**: [Date]
- **Planned End Date**: [Date]

### Prioritization Score
- **Framework Used**: [PIE/ICE/PXL]
- **Score**: [X]
```

### Post-Test

```markdown
## Results

### Summary
- **Winner**: [Control/Variant/Inconclusive]
- **Confidence Level**: [X%]
- **Observed Lift**: [X%]
- **Sample Size Achieved**: [X]

### Primary Metric
| Variation | Visitors | Conversions | Rate |
|-----------|----------|-------------|------|
| Control | X | X | X% |
| Variant | X | X | X% |

### Secondary Metrics
[Table of other metrics]

### Segment Analysis
[Notable segment differences]

### Learnings
1. [Key insight 1]
2. [Key insight 2]
3. [Key insight 3]

### Next Steps
- [ ] Implement winner (if applicable)
- [ ] Follow-up test ideas
- [ ] Document in knowledge base

### Screenshots
[Before/after screenshots]
```

---

## Common Mistakes

### 1. Insufficient Sample Size

> "Running underpowered tests is common due to insufficient sample sizes. Plan tests meticulously using power analysis calculators."
>
> *Source: [Statsig](https://www.statsig.com/blog/top-8-common-experimentation-mistakes-how-to-fix)*

**Solution**: Calculate sample size BEFORE starting. If you can't reach it, test bigger changes.

### 2. Testing Too Many Variations

More variations = more sample needed = longer test = higher error risk.

| Variations | Sample Multiplier |
|------------|-------------------|
| 2 (A/B) | 1x |
| 3 (A/B/C) | 1.5x |
| 4 (A/B/C/D) | 2x |

**Solution**: Stick to A/B unless you have massive traffic.

### 3. Stopping Early (Winner Declared)

> "Most experiments have a 70% chance of looking 'significant' before they are truly done collecting sufficient data."
>
> *Source: [Mida](https://www.mida.so/blog/what-is-peeking-ab-testing)*

**Solution**: Commit to the full duration. Period.

### 4. Testing Trivial Changes

Button color (blue vs. green) rarely matters. Test things that actually change user behavior.

**Solution**: Test hypothesis-driven changes based on real user problems.

### 5. Ignoring Segment Differences

Overall results may hide important segment-level insights.

**Solution**: Pre-define segments to analyze (mobile/desktop, new/returning, etc.)

### 6. Not Documenting Tests

90% of learning value comes from documentation and pattern recognition across tests.

**Solution**: Document every test, including losers and inconclusive results.

### 7. Sample Ratio Mismatch (SRM)

When traffic split doesn't match intended (e.g., 55/45 instead of 50/50).

> "Neglecting bots which make up a huge amount of traffic can impact SRM and skew results."
>
> *Source: [Kameleoon](https://www.kameleoon.com/blog/data-accuracy-pitfalls-ab-testing)*

**Solution**: Always check actual traffic distribution before analyzing results.

---

## Advanced Methods

### Sequential Testing

> "Sequential testing allows for continuous monitoring of test results without the statistical penalties associated with peeking."
>
> *Source: [Statsig](https://www.statsig.com/perspectives/false-positive-rate-ab-testing)*

Adjusts significance thresholds dynamically—useful when you need to monitor results.

### Bayesian Testing

Instead of p-values, uses probability distributions to estimate:
- Probability variant B beats A
- Expected lift range
- Risk of implementing B

More intuitive interpretation but requires different mental model.

### CUPED (Controlled-experiment Using Pre-Experiment Data)

> "In a 2025 survey, experimentation leaders using CUPED or Bayesian methods were 270% more likely to grow significantly than teams relying only on basic A/B testing."
>
> *Source: [Statsig](https://www.statsig.com/perspectives/ab-testing-methodology)*

Uses pre-experiment data to reduce variance and reach significance faster.

---

## A/B Testing Tools

### Enterprise

| Tool | Strength | Pricing |
|------|----------|---------|
| Optimizely | Full platform, statistics | $$$$ |
| VWO | User-friendly, visual editor | $$$ |
| AB Tasty | AI-powered, personalization | $$$ |

### Mid-Market

| Tool | Strength | Pricing |
|------|----------|---------|
| Convert | Privacy-focused, accurate | $$ |
| Kameleoon | Bayesian stats, AI | $$ |
| Omniconvert | E-commerce focus | $$ |

### Self-Hosted / Free

| Tool | Strength | Pricing |
|------|----------|---------|
| GrowthBook | Open source, full-featured | Free |
| Statsig | Generous free tier | Free-$$ |
| Google Optimize | Deprecated 2023 | N/A |

---

## A/B Testing Checklist

### Before Test

- [ ] Hypothesis documented with evidence
- [ ] Primary metric defined
- [ ] Sample size calculated
- [ ] Duration determined (min 2 weeks)
- [ ] Technical QA completed
- [ ] Tracking verified
- [ ] Stakeholders aligned

### During Test

- [ ] **Don't peek** (or use sequential testing)
- [ ] Monitor for technical issues only
- [ ] Check for SRM
- [ ] Document any external factors

### After Test

- [ ] Reached sample size
- [ ] Ran for full duration
- [ ] Analyzed primary metric first
- [ ] Checked segment breakdowns
- [ ] Documented results
- [ ] Shared learnings
- [ ] Planned next steps

---

## Sources

- [VWO - A/B Testing Statistics](https://vwo.com/blog/ab-testing-statistics/)
- [NN/g - A/B Testing 101](https://www.nngroup.com/articles/ab-testing/)
- [Evan Miller - How Not to Run an A/B Test](https://www.evanmiller.org/how-not-to-run-an-ab-test.html)
- [CXL - PXL Prioritization Framework](https://cxl.com/blog/better-way-prioritize-ab-tests/)
- [Speero - How to Prioritize A/B Tests](https://speero.com/post/how-to-prioritize-your-a-b-tests-ideas)
- [Statsig - A/B Testing Methodology](https://www.statsig.com/perspectives/ab-testing-methodology)
- [GrowthBook - Experimentation Problems](https://docs.growthbook.io/using/experimentation-problems)
- [Lucidchart - The Fatal Flaw of Peeking](https://www.lucidchart.com/blog/the-fatal-flaw-of-ab-tests-peeking)
- [Analytics-Toolkit - Statistical Significance Guide](https://blog.analytics-toolkit.com/2017/statistical-significance-ab-testing-complete-guide/)
- [Optimizely - Sample Size Calculator](https://www.optimizely.com/sample-size-calculator/)
- [Convert - A/B Testing Stats](https://www.convert.com/blog/a-b-testing/ab-testing-stats/)
- [Cro Metrics - Sample Size Guide](https://crometrics.com/blog/ab-testing-sample-size/)
- [Kameleoon - Data Accuracy Pitfalls](https://www.kameleoon.com/blog/data-accuracy-pitfalls-ab-testing)
