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
   - `library/pages/*/` for page-type benchmarks
   - `library/conversion/` for conversion metrics

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
- `saas`, `ecommerce`, `healthcare`, `finance`, `real-estate`, `restaurants`, `media`, `professional-services`, `b2b-enterprise`
