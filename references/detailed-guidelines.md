# Detailed Web Design & Brand Architecture Guidelines

Reference material for deep audits, multi-section page builds, and comprehensive reviews. The SKILL.md covers the strategic essentials — this file provides the full checklist and expanded rationale.

## Table of Contents

1. [Stage-Appropriate Design Deep Dive](#1-stage-appropriate-design-deep-dive)
2. [Messaging and Copy Standards](#2-messaging-and-copy-standards)
3. [Visual Execution Audit Checklist](#3-visual-execution-audit-checklist)
4. [Interaction Design Detailed Rules](#4-interaction-design-detailed-rules)
5. [Conversion and Social Proof Standards](#5-conversion-and-social-proof-standards)
6. [Comprehensive QA Checklist](#6-comprehensive-qa-checklist)

---

## 1. Stage-Appropriate Design Deep Dive

### Mystery vs. Transparency Tactics

Choose based on your conversion goal:

**Mystery (early-stage, waitlist capture):**
- Use faded, stylized, or partially obscured product screenshots
- Builds curiosity and manages expectations for an incomplete product
- Example: Linear in 2019 — moody, minimal, suggestive of capability without proving it
- Single-page is fine. Buildable in a day. The message matters, not the page count.

**Transparency (growth-stage, direct conversion):**
- Use high-fidelity, literal, full-resolution screenshots
- Proves product depth and maturity to users ready to commit
- Example: Linear in 2024 — every feature documented, real UI everywhere
- Multi-page with dedicated sections for features, pricing, security, docs

### Simplicity as Strategic Signal

Simple design is not a budget compromise. It's a strategic filter. The goal is to attract users who need the core solution, not visitors impressed by visual effects. A clean, focused page signals that the team is focused on the product, not on marketing theater.

---

## 2. Messaging and Copy Standards

### Value Proposition Formula

Structure: [Specific action verb] + [for whom] + [concrete outcome]

**Good examples:**
- "Issue tracking for engineering teams. Ship 2x faster."
- "Automated bookkeeping for freelancers. Save 10 hours/month."

**Bad examples:**
- "The platform for modern work" (vague, no audience, no outcome)
- "Empowering teams to achieve more" (corporate filler, says nothing)

### Jargon as a Filter

Specific terminology self-selects the right audience:
- "Issue Tracking" → attracts engineers, filters out non-technical users
- "Revenue Operations" → attracts ops leaders, filters out casual browsers
- "HIPAA-Compliant Messaging" → attracts healthcare, signals compliance focus

Only large, established platforms earn the right to use broad language. If you're not Slack, don't say "Where work happens."

### Defining Unfamiliar Terms

Never assume users know your internal terminology. If your product references concepts like "MCP," "Deep Eval," or any non-obvious term, define it in a sub-headline immediately. Ground the user before expecting them to care.

---

## 3. Visual Execution Audit Checklist

### Brand Identity Checks

- [ ] **Logo integrity**: Professionally sized and placed. Not a tiny emoji or awkwardly scaled.
- [ ] **Contrast and legibility**: No light-on-light text. No yellow backgrounds with white text.
- [ ] **Color intentionality**: No clashing palettes (red logo on purple background). Colors should reinforce, not fight.
- [ ] **Asset fidelity**: All screenshots high-resolution and high-contrast. No blurry, cropped, or placeholder images.

### "AI Slop" Detection Checklist

Flag any of the following on sight:

- [ ] Purple-to-blue gradients as primary background treatment
- [ ] Default CSS box-shadows with no intentional design system
- [ ] 3×2 bento-box grid with generic icons (no product context)
- [ ] Dashboard mockups using Google's primary color palette (red/yellow/green/blue)
- [ ] Floating 3D shapes, abstract cubes, or generic geometric hero graphics
- [ ] Five or more different font treatments on one page ("style soup")
- [ ] Background images or videos with no contrast overlay (unreadable nav)
- [ ] Hard-coded timestamps, placeholder names, or fake data in screenshots

### Typography Rules

- If not a typographer, use clean system fonts. One display font + one body font maximum.
- Heading hierarchy must be visually distinct and consistent.
- Never mix more than two font families on a page (three in exceptional cases with clear roles).

---

## 4. Interaction Design Detailed Rules

### Animation Principles

**Rule of Purpose**: Every animation must serve one of these goals:
1. Draw attention to the primary CTA
2. Provide feedback on user action (hover, click, transition)
3. Create a sense of spatial relationship (scroll reveals, section transitions)

If an animation doesn't serve one of these, remove it.

**Forbidden patterns:**
- **Scroll jacking**: Hijacking native scroll behavior to force timed animations. Users should always control their scroll speed.
- **Looping chaos**: Shooting meteors, perpetually flickering cards, pulsing backgrounds. Constant motion creates cognitive noise.
- **The molasses effect**: Timed fade-ins that make users wait before they can read. Content should be available immediately on scroll.

### Hover State Rules

Hover should make elements feel inviting and responsive:
- Subtle color shifts, scale changes, or glow effects to indicate interactivity
- Cursor changes to signal clickability

**Forbidden**: Hover-to-disclose. Never hide critical information or navigation behind hover. It fails on mobile and creates frustrating "treasure hunts" on desktop.

### Navigation Standards

- Navigation must remain readable over any background (video, images, dynamic content). Use contrast overlays.
- Menus must not disappear, jump, or behave non-standardly.
- Mobile navigation deserves equal attention to desktop — it's not an afterthought.

---

## 5. Conversion and Social Proof Standards

### Reducing Friction

**The demo paradox**: "Book a Demo" requires a 20-minute commitment. Before asking for time, offer:
- In-browser interactive prompts or sandboxes
- Short product videos (under 2 minutes)
- Feature screenshots with annotated callouts
- Free tier or trial with no credit card required

**CTA discipline**: One goal per scroll segment. Eliminate competing calls to action. The hero section especially should not be "link salad" with simultaneous links to Discord, GitHub, Twitter, Docs, Blog, and Careers.

### Social Proof Standards

**Human output signals** — testimonials must feel written by humans:
- [ ] No Every Word Capitalized patterns
- [ ] Specific outcomes ("Saved 500 hours on manual QA") not vague praise ("Great tool!")
- [ ] Real names and real job titles attached
- [ ] Company logos standardized in B&W for visual cleanliness
- [ ] Ideally, real photos or linked profiles

**Anti-patterns to flag:**
- Anonymous testimonials with no attribution
- Testimonials that read like marketing copy
- Logos of companies who aren't actually customers
- Star ratings with no context or review text

---

## 6. Comprehensive QA Checklist

Run this checklist as the final audit before shipping any page:

### Content & Messaging
- [ ] Hero passes the Five-Second Filter (What / Who / Why / So what?)
- [ ] No vague slogans where specific language would serve better
- [ ] All internal jargon defined on first use
- [ ] Claims backed by visual evidence (screenshots, demos, metrics)
- [ ] No "Everything-on-One-Page" trap — pricing, about, and security get their own pages for mature products

### Visual Quality
- [ ] No AI slop patterns (purple gradients, bento boxes, fake dashboards)
- [ ] Consistent spacing throughout — no double spaces, stray periods, or alignment drift
- [ ] Logo properly sized and placed
- [ ] All text meets contrast accessibility standards
- [ ] Screenshots are high-res, current, and show real product UI
- [ ] No hard-coded timestamps or placeholder data visible

### Interaction & UX
- [ ] No scroll jacking or timed animations blocking content
- [ ] No critical info hidden behind hover states
- [ ] Navigation readable over all background types
- [ ] Single clear CTA per scroll segment
- [ ] Mobile experience tested and functional

### Conversion Flow
- [ ] Path from landing to action is frictionless
- [ ] Low-commitment option available before "Book a Demo"
- [ ] Social proof is specific, attributed, and human-sounding
- [ ] No link salad in hero section

### Technical Polish
- [ ] No broken links or 404s
- [ ] Page loads fast (no massive unoptimized hero videos)
- [ ] Responsive across breakpoints
- [ ] Favicon and meta tags set
- [ ] OG/social preview image configured
