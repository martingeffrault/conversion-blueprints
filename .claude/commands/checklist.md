# Checklist

Generate a conversion-optimized checklist for building or reviewing a page.

## Usage
```
/checklist [page-type] [industry?]
```

## Examples
```
/checklist landing-page
/checklist homepage saas
/checklist pricing ecommerce
/checklist product-page healthcare
```

## Instructions

When this command is invoked:

1. **Load the relevant blueprint** from:
   - `library/pages/[page-type]/` - primary patterns
   - `library/industry/[industry].md` - industry-specific requirements
   - `library/sections/` - section-level details

2. **Generate a practical checklist** organized by:

   ### Structure
   - [ ] Page sections in recommended order
   - [ ] Above-fold essentials present
   - [ ] Clear information hierarchy

   ### Hero Section
   - [ ] Clear value proposition (5-7 words)
   - [ ] Benefit-focused headline
   - [ ] Primary CTA visible
   - [ ] Trust signals present

   ### Content
   - [ ] Benefits before features
   - [ ] Social proof included
   - [ ] Objection handling
   - [ ] Scannable formatting

   ### Conversion Elements
   - [ ] Single primary CTA per section
   - [ ] Form optimized (if applicable)
   - [ ] Urgency/scarcity (if appropriate)
   - [ ] Exit intent strategy

   ### Technical
   - [ ] Mobile-responsive
   - [ ] Fast loading (<3s)
   - [ ] Accessible (WCAG basics)
   - [ ] Analytics tracking

3. **Include relevant benchmarks** for success metrics

4. **Reference specific library documents** for deeper guidance

## Output Format
Return as a copyable markdown checklist that can be added to project docs or task management.
