# Benchmark

Get conversion benchmarks for a specific metric or industry.

## Usage
```
/benchmark [metric-or-industry]
```

## Examples
```
/benchmark landing-page-cvr
/benchmark saas
/benchmark form-completion
/benchmark ecommerce
/benchmark trial-to-paid
```

## Instructions

When this command is invoked:

1. **Search the knowledge base** for relevant benchmarks:
   - `library/_index.md` for general benchmarks
   - `library/industry/[industry].md` for industry-specific
   - `library/analytics/kpis-by-business.md` for KPIs by business type
   - `library/analytics/advanced-analytics.md` for attribution, retention, CLV
   - `library/analytics/technical-performance.md` for Core Web Vitals
   - `library/pages/*/` for page-type benchmarks
   - `library/conversion/benchmarks.md` for conversion metrics
   - `library/conversion/micro-conversions.md` for funnel metrics

2. **Return a structured response** with:
   - Metric name and definition
   - Average / Good / Excellent ranges
   - Source with link
   - Context (what affects this metric)
   - Related metrics to track

3. **Always include the source** - this repo prioritizes sourced data

## Common Metrics
- `landing-page-cvr` - Landing page conversion rate
- `form-completion` - Form completion rate
- `trial-to-paid` - Free trial to paid conversion
- `add-to-cart` - E-commerce add to cart rate
- `bounce-rate` - Page bounce rate
- `time-on-page` - Average time on page

## Industries
- `saas`, `ecommerce`, `healthcare`, `finance`, `real-estate`, `restaurants`, `media`, `professional-services`, `b2b-enterprise`, `nonprofit`, `education`, `creator-economy`, `local-business`, `crypto-web3`

## Analytics Metrics
- `core-web-vitals` - LCP, CLS, INP benchmarks
- `retention` - Industry retention rates
- `clv-cac` - Customer lifetime value to CAC ratio
- `attribution` - Multi-touch attribution stats
