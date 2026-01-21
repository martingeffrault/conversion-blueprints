# Audit Page

Audit a page or component against conversion best practices from this knowledge base.

## Usage
```
/audit-page [page-type] [url-or-description]
```

## Examples
```
/audit-page landing-page https://example.com/signup
/audit-page homepage "SaaS product homepage with hero, features, pricing"
/audit-page pricing "3-tier pricing table for B2B software"
```

## Instructions

When this command is invoked:

1. **Identify the page type** from the argument or infer from context
2. **Load relevant blueprints** from this repo:
   - `library/pages/[page-type]/` for page-specific patterns
   - `library/sections/` for section patterns
   - `library/conversion/` for conversion patterns
   - `library/industry/` if industry is specified

3. **Analyze against checklist** covering:
   - Above-fold elements (hero, value prop, CTA)
   - Trust signals and social proof
   - Form optimization (if applicable)
   - Mobile considerations
   - Page speed factors

4. **Output a structured audit** with:
   - Score or grade (optional)
   - What's working well
   - Critical issues to fix
   - Quick wins
   - Recommended A/B tests
   - Relevant benchmarks with sources

5. **Reference specific documents** from the library for each recommendation

## Page Types Supported
- `landing-page` → library/pages/landing-page/
- `homepage` → library/pages/homepage/
- `pricing` → library/pages/pricing/
- `product` → library/pages/product/
- `case-study` → library/pages/case-study/
- `demo-trial` → library/pages/demo-trial/
- `contact` → library/pages/contact/
