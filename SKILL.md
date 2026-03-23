---
name: yc-web-design-strategy
description: >
  Strategic web design consultant for building, reviewing, or auditing websites and landing pages. Trigger when the user asks to build a landing page, review a site's messaging, write hero copy or CTAs, audit for "AI slop," or plan page information architecture. Also trigger on keywords: "landing page," "above the fold," "hero section," "conversion funnel," "social proof," "product page design."
---

# Web Design Strategy

A strategic design consultant skill that ensures websites communicate the right message, to the right audience, in the right order — before worrying about how pretty they look.

This skill applies to building new sites, reviewing existing ones, writing landing page copy, and auditing pages for common failures. Read `references/detailed-guidelines.md` for the full checklist when performing deep audits or multi-section page builds.

## Core Principle

Design strategy comes before visual execution. A beautiful site that says the wrong thing, to the wrong audience, in the wrong order, will always lose to a plain site with clear messaging. Lead with strategy, then layer on aesthetics (using the `frontend-design` skill for visual execution when building).

---

## 1. Stage-Aware Design

Before writing a single line of copy or code, identify where the company sits in its lifecycle. This determines everything — layout complexity, screenshot fidelity, CTA strategy, and page depth.

| Stage | Design Approach | Key Signals |
|-------|----------------|-------------|
| **Pre-launch / Early** | Build mystery. Faded or stylized screenshots. Waitlist/email capture. Single-page, buildable in a day. Simple, focused message. | No public product, small team, pre-revenue |
| **Growth** | Brand recognition. Signature accent colors, detailed feature breakdowns, high-res product screenshots, multiple CTAs. | Live product, active users, iterating on PMF |
| **Mature** | Information depth. Product sub-sections, roadmaps, security/compliance pages, enterprise tiers. Restrained, authoritative palette. | Established market presence, enterprise deals |

Mimicking a mature company's polish when you're pre-launch creates a trust deficit — it promises completeness you can't deliver. Conversely, a mature product with a single-page waitlist site signals neglect.

---

## 2. The Five-Second Filter

Every landing page must answer these four questions within five seconds of arrival:

1. **What is it?** — Use plain, specific language. "A chat app" not "A synergy platform."
2. **Who is it for?** — Name the audience. "For technical project managers" beats "For teams."
3. **To what end?** — State the immediate benefit or outcome.
4. **Why should they care?** — What makes this better than the status quo?

Startups cannot afford vague slogans. Use specific jargon as a high-value filter — "Issue Tracking" attracts engineers while filtering out non-fits. Only massive established platforms earn the right to say things like "Where work happens."

### The Pyramid of Clarity

Structure homepage content in order of decreasing urgency:

1. **Apex** — Sharp, jargon-aligned value proposition (hero section)
2. **Expanding context** — Feature narratives with visual proof as user scrolls
3. **Functional depth** — Technical docs, secondary use cases, pricing, security (separate pages for mature products)

---

## 3. Avoiding "AI Slop" Patterns

Originality is a proxy for product quality. If the site looks like generic LLM output, users assume the product is too. Flag and eliminate these patterns:

**Visual slop signals:**
- Purple gradients and default drop shadows (the #1 "AI made this" signal)
- Generic bento-box grids (3×2 with simple icons, no product context)
- Google-style fake dashboards with primary-color callouts (red/yellow/green/blue)
- Floating cubes, abstract 3D shapes, or generic hero graphics with no product evidence

**Micro-detail failures (the "fit and finish" layer):**
- Inconsistent spacing, double spaces in headlines, stray periods
- Hard-coded timestamps or placeholder data visible in screenshots
- "Style soup" — mixing 5+ font treatments, destroying visual hierarchy
- Low-contrast text (light-on-light, yellow on white)
- Tiny or awkwardly sized logos

**Copy slop signals:**
- Every Word Capitalized In Testimonials (screams "AI-generated")
- Vague social proof like "Great tool!" instead of "Saved 500 hours on manual QA"
- Undefined internal jargon (don't assume users know what "Deep Eval" or "MCP" means)

---

## 4. Interaction Design Rules

Animation and interaction should enhance navigation, never distract from the value proposition.

**Do:**
- Use motion to draw attention to the primary CTA
- Subtle hover color shifts or glows to indicate clickability
- Scroll-triggered reveals that feel natural

**Don't:**
- Scroll-jack (hijack native scrolling with timed animations)
- Loop background animations (meteors, flickering cards, constant motion)
- Hide information behind hover states (breaks on mobile, forces "hunting" on desktop)
- Create "link salad" in the hero — simultaneous links to Discord, GitHub, Twitter, and Docs

---

## 5. Conversion Optimization

Every hurdle is an abandonment point. Minimize friction between arrival and the "aha moment."

- **Demo paradox**: A "Book a Demo" button asks for a 20-minute commitment. Offer a taste first — in-browser prompts, interactive sandboxes, short product videos.
- **CTA discipline**: One clear goal per scroll segment. Don't stack competing CTAs.
- **Social proof standards**: Real names, real titles, real company logos (B&W for cleanliness). Specific outcomes over generic praise.

---

## 6. Applying This Skill

**When building a new page:**
1. Ask (or determine) the company's lifecycle stage
2. Draft copy that passes the Five-Second Filter
3. Plan the information architecture using the Pyramid of Clarity
4. Build the page (use `frontend-design` for visual execution)
5. Audit the result against the slop checklist and fit-and-finish items in `references/detailed-guidelines.md`

**When reviewing/critiquing an existing page:**
1. Read `references/detailed-guidelines.md` for the full audit checklist
2. Evaluate stage-appropriateness first
3. Run the Five-Second Filter
4. Check for AI slop patterns
5. Audit interaction design and conversion flow
6. Provide specific, actionable feedback organized by severity

**When writing hero copy or CTAs:**
1. Identify the target audience and their language
2. Use the Five-Second Filter as a writing constraint
3. Prefer specific jargon over broad slogans
4. Back every claim with visual proof (screenshots, demos, metrics)
