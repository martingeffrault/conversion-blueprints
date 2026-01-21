# Accessibility Testing Guide

> **Purpose**: Test websites for accessibility compliance systematically
> **Approach**: Combine automated, manual, and assistive technology testing
> **Principle**: Automated testing catches ~30% of issues — manual testing is essential

---

## Testing Approach

### The Three-Layer Testing Strategy

```
┌─────────────────────────────────────────────────────────────────┐
│  Layer 1: Automated Testing                                      │
│  Tools scan for common issues                                   │
│  Catches: ~30% of issues                                        │
└─────────────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────────────┐
│  Layer 2: Manual Testing                                         │
│  Human review of keyboard, visual, content                       │
│  Catches: ~50% of remaining issues                              │
└─────────────────────────────────────────────────────────────────┘
                              ↓
┌─────────────────────────────────────────────────────────────────┐
│  Layer 3: Assistive Technology Testing                          │
│  Real screen readers, voice control                             │
│  Catches: Context, flow, usability issues                       │
└─────────────────────────────────────────────────────────────────┘
```

### What Automated Testing Can Find

| Can Find | Cannot Find |
|----------|-------------|
| Missing alt text | Quality of alt text |
| Color contrast ratios | Color meaning context |
| Missing form labels | Label clarity |
| Invalid HTML | Logical reading order |
| Missing ARIA attributes | Correct ARIA usage |
| Focus order issues | Focus visibility quality |

---

## Layer 1: Automated Testing

### Browser Extensions

| Tool | Platform | Best For |
|------|----------|----------|
| **axe DevTools** | Chrome, Firefox, Edge | Comprehensive testing |
| **WAVE** | Chrome, Firefox | Visual feedback |
| **Lighthouse** | Chrome | Performance + accessibility |
| **ARC Toolkit** | Chrome | WCAG compliance |
| **Accessibility Insights** | Chrome, Edge | Step-by-step testing |

### CI/CD Integration Tools

| Tool | Integration | Features |
|------|-------------|----------|
| **axe-core** | npm, CI/CD | Automated testing in builds |
| **Pa11y** | CLI, npm | CI/CD integration |
| **Lighthouse CI** | GitHub Actions | Automated audits |
| **Deque axe** | API | Enterprise testing |

### Online Testing Tools

| Tool | URL | Best For |
|------|-----|----------|
| **WAVE** | wave.webaim.org | Quick checks |
| **axe** | deque.com/axe | Comprehensive |
| **Lighthouse** | PageSpeed Insights | Performance + a11y |
| **Tenon** | tenon.io | API-based testing |
| **SortSite** | powermapper.com | Full site scans |

### Running Automated Tests

**axe DevTools**:
1. Install browser extension
2. Open DevTools → axe tab
3. Click "Scan ALL of my page"
4. Review issues by impact (Critical, Serious, Moderate, Minor)

**Lighthouse**:
1. Open DevTools → Lighthouse tab
2. Check "Accessibility" category
3. Generate report
4. Review failing audits

**Pa11y (CLI)**:
```bash
# Single page
pa11y https://example.com

# With reporter
pa11y https://example.com --reporter cli

# Standard
pa11y https://example.com --standard WCAG2AA

# Multiple pages
pa11y-ci --config .pa11yci.json
```

---

## Layer 2: Manual Testing

### Keyboard Testing

**Test All Interactive Elements**:

| Element | Test | Expected |
|---------|------|----------|
| Links | Tab to, Enter to activate | Navigates |
| Buttons | Tab to, Enter/Space | Activates |
| Forms | Tab through, submit | Works |
| Menus | Tab, arrow keys | Opens, navigates |
| Modals | Tab, Escape | Focus trapped, closes |
| Carousels | Arrow keys | Navigates slides |

**Keyboard Testing Checklist**:
- [ ] Can reach all interactive elements with Tab
- [ ] Tab order is logical (follows visual layout)
- [ ] Focus indicator always visible
- [ ] No keyboard traps (can Tab out of everything)
- [ ] Skip link works
- [ ] Modals trap focus correctly
- [ ] Can close modals with Escape
- [ ] Dropdowns work with arrow keys

**How to Test**:
1. Put mouse aside
2. Use Tab to navigate through page
3. Verify every interactive element is reachable
4. Verify focus is always visible
5. Use Enter/Space to activate elements
6. Verify modals and menus work

### Visual Testing

**Color Contrast**:
1. Use WAVE or axe to flag issues
2. Manually verify flagged elements
3. Check text over images (often missed)
4. Check focus indicators
5. Check error states

**Tools**:
- **WebAIM Contrast Checker**: webaim.org/resources/contrastchecker
- **Colour Contrast Analyser**: tpgi.com/color-contrast-checker
- **Stark** (Figma plugin): Check during design

**Text Resizing**:
1. Browser zoom to 200%
2. Verify no content cut off
3. Verify no horizontal scroll
4. Verify text remains readable

**Motion**:
1. Enable "Reduce Motion" in OS
2. Verify animations respect preference
3. Check for flashing content

### Content Testing

**Headings**:
1. Use WAVE or HeadingsMap extension
2. Verify single H1
3. Verify no skipped levels
4. Verify headings describe content

**Links**:
1. Review link text (no "click here")
2. Verify links make sense out of context
3. Check for duplicate link text with different destinations

**Images**:
1. Disable images (browser extension)
2. Read alt text — does it convey meaning?
3. Verify decorative images have empty alt

**Forms**:
1. Tab through form
2. Verify all fields have labels
3. Verify error messages are clear
4. Verify required fields indicated
5. Test error handling

---

## Layer 3: Assistive Technology Testing

### Screen Readers

| Screen Reader | Platform | Browser |
|---------------|----------|---------|
| **VoiceOver** | macOS, iOS | Safari |
| **NVDA** | Windows | Firefox, Chrome |
| **JAWS** | Windows | Chrome, Firefox, Edge |
| **TalkBack** | Android | Chrome |
| **Narrator** | Windows | Edge |

### VoiceOver Basics (macOS)

**Enable**: Command + F5 or System Preferences → Accessibility → VoiceOver

| Command | Action |
|---------|--------|
| VO + Right Arrow | Next item |
| VO + Left Arrow | Previous item |
| VO + Space | Activate |
| VO + Shift + Down | Enter element |
| VO + Shift + Up | Exit element |
| VO + U | Rotor (lists, headings, links) |
| Control | Stop speaking |

**VO key**: Control + Option

**Testing with VoiceOver**:
1. Enable VoiceOver
2. Navigate page with VO + arrow keys
3. Verify content read in logical order
4. Verify images described appropriately
5. Verify form labels read correctly
6. Verify buttons/links have clear names
7. Test with Rotor (headings, links, landmarks)

### NVDA Basics (Windows)

**Download**: nvaccess.org (free)

| Command | Action |
|---------|--------|
| Insert + Down Arrow | Read from current position |
| Insert + Up Arrow | Current line |
| Tab | Next focusable |
| H | Next heading |
| D | Next landmark |
| Insert + F7 | Elements list |
| Escape | Stop |

**Testing with NVDA**:
1. Launch NVDA
2. Navigate with Tab and arrow keys
3. Use H for headings, D for landmarks
4. Verify logical reading order
5. Verify forms work
6. Test interactive components

### Screen Reader Testing Checklist

- [ ] Page title announced
- [ ] Headings navigate correctly
- [ ] Landmarks present and correct
- [ ] Images described appropriately
- [ ] Links have clear purpose
- [ ] Buttons clearly labeled
- [ ] Forms can be completed
- [ ] Tables read correctly
- [ ] Dynamic content announced
- [ ] Error messages announced

---

## Testing Different Disabilities

### Visual Impairments

**Low Vision**:
- Zoom to 200% — is content usable?
- Is contrast sufficient?
- Can text be resized without breaking layout?

**Color Blindness**:
- Use Color Oracle or Sim Daltonism
- Is information conveyed without color alone?

**Blindness**:
- Screen reader testing (above)

### Motor Impairments

**Keyboard Only**:
- Can all functionality be accessed?
- Are touch targets large enough (44x44px)?
- Is there enough time for interactions?

**Voice Control**:
- Are all links/buttons visually labeled?
- Can Dragon NaturallySpeaking navigate?

### Cognitive Impairments

**Readability**:
- Is content clear and concise?
- Are instructions easy to follow?
- Are errors explained with solutions?

**Focus**:
- Is design clean without distractions?
- Can animations be paused?
- Is navigation consistent?

### Hearing Impairments

**Video Content**:
- Are captions accurate?
- Are captions synchronized?
- Is there a transcript?

**Audio Cues**:
- Are there visual alternatives to audio alerts?

---

## Reporting Issues

### Issue Documentation Template

```markdown
## Accessibility Issue

**Page**: [URL]
**Element**: [Description/selector]
**WCAG Criterion**: [e.g., 1.1.1 Non-text Content]
**Level**: [A, AA, AAA]
**Impact**: [Critical, Serious, Moderate, Minor]

### Description
[What is the issue?]

### Steps to Reproduce
1. [Step 1]
2. [Step 2]
3. [Step 3]

### Expected Behavior
[What should happen]

### Actual Behavior
[What actually happens]

### Recommended Fix
[How to fix the issue]

### Screenshot/Recording
[Attach if applicable]
```

### Issue Severity Levels

| Level | Impact | Example |
|-------|--------|---------|
| **Critical** | Blocks users | Cannot submit form, no keyboard access |
| **Serious** | Major barrier | Missing form labels, no skip link |
| **Moderate** | Significant barrier | Poor contrast, confusing navigation |
| **Minor** | Annoyance | Best practice violation |

---

## Testing Workflow

### Development Phase

1. **Component Level**: Test each component as built
2. **Integration**: Test components together
3. **Pre-merge**: Automated tests in CI

### QA Phase

1. **Automated Scan**: Run axe/WAVE on all pages
2. **Manual Audit**: Keyboard, visual, content
3. **Screen Reader**: NVDA or VoiceOver on key flows

### Pre-Launch

1. **Full Audit**: All pages, all criteria
2. **User Testing**: Disabled users (if possible)
3. **Documentation**: Accessibility statement

### Ongoing

- Automated monitoring (monthly)
- Manual review of new features
- User feedback loop
- Annual comprehensive audit

---

## Testing Tools Summary

### Free Tools

| Category | Tools |
|----------|-------|
| Browser Extensions | axe DevTools, WAVE, Lighthouse |
| Screen Readers | NVDA, VoiceOver (built-in) |
| Color Contrast | WebAIM Contrast Checker |
| Color Blindness | Color Oracle, Sim Daltonism |
| CI/CD | Pa11y, axe-core, Lighthouse CI |

### Paid Tools

| Tool | Best For |
|------|----------|
| Deque axe Pro | Enterprise testing |
| SortSite | Full site audits |
| Tenon | API-based testing |
| Level Access | Comprehensive audits |
| Siteimprove | Monitoring |

---

## Sources

- [WebAIM - Testing Techniques](https://webaim.org/articles/testing/)
- [Deque - Accessibility Testing](https://www.deque.com/web-accessibility-testing/)
- [W3C - Easy Checks](https://www.w3.org/WAI/test-evaluate/preliminary/)
- [A11y Project - How to Test](https://www.a11yproject.com/checklist/)
- [Apple VoiceOver Guide](https://www.apple.com/accessibility/vision/)
- [NV Access - NVDA](https://www.nvaccess.org/)
- [WebAIM Screen Reader Survey](https://webaim.org/projects/screenreadersurvey9/)
