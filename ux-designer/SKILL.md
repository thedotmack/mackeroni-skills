---
name: ux-designer
description: @thedotmack's personal landing page design system. Use this skill whenever building landing pages, marketing sites, product pages, or conversion-focused web experiences. Covers visual hierarchy, UX patterns, marketing copy, messaging strategy, and conversion optimization based on proven preferences and successful projects.
---

# @thedotmack's Landing Page & Marketing Design System

This skill encodes the design philosophy, UX patterns, copywriting voice, and conversion strategies @thedotmack has developed across dozens of successful landing pages. These aren't theoretical principles; they're patterns extracted from what actually shipped and worked.

---

## Core Design Philosophy

### Simplicity Is The Strategy

Every design decision runs through KISS, DRY, and YAGNI. If a section doesn't earn its place on the page, it gets cut. If an animation doesn't serve comprehension or conversion, it goes. The goal is clarity, not decoration.

- Simple solutions first, always
- If you're reaching for complexity, stop and ask: "Could this be simpler?"
- Delete before you add. The best fix for a cluttered page is removing things.
- Build working prototypes, not theoretical wireframes

### Foundational References

This design system is built on two key texts that should be internalized, not just referenced:

**Steve Krug's "Don't Make Me Think":**
- Every page should be self-evident. If a user has to think about how to navigate, you've failed.
- Reduce noise and visual clutter ruthlessly
- Conventions are your friend — don't reinvent navigation, form patterns, or CTAs
- Test with real people, observe where they struggle, fix those things

**Adam Wathan & Steve Schoger's "Refactoring UI":**
- Hierarchy through weight AND color, not just size
- Labels as a last resort — if the content is clear, the label is noise
- Systematic spacing on an 8px grid, not arbitrary values
- Typography creates hierarchy — use weight, size, color, and opacity together
- Start with too much white space, then selectively reduce
- Don't force elements to fill available space unless they need to

---

## Page Architecture

### The Scroll Narrative

Landing pages tell stories. They don't dump features — they take the visitor on a journey from problem awareness to purchase decision. The structure follows a consistent emotional arc:

```
1. Hero → Grab attention, state the core promise
2. Problem → Name the pain the visitor already feels
3. Solution → Show how you solve it (not features—transformation)
4. Proof → Social proof, numbers, case studies
5. How It Works → Simple 3-step process
6. Pricing/CTA → Clear options, risk reversal
7. FAQ → Handle objections
8. Final CTA → One last push
```

This isn't rigid — some pages compress or expand sections. But the emotional arc remains consistent.

### Section-Level Patterns

**Hero Section:**
- One clear value proposition, not three competing messages
- Use "your" not "a" — "Build **your** ___" not "Build a ___"
- Benefits-oriented subhead (what changes for them), not feature-oriented
- Primary CTA + secondary CTA (never more than two)
- Social proof badges or stats strip below the fold line
- Generous spacing — let the message breathe

**Problem Section:**
- Name the specific pain point the audience already knows
- Use their language, not marketing speak
- Short, punchy sentences that build tension
- "Here's the trap:" or "But here's the problem:" as a pivot
- The visitor should be nodding before you present the solution

**Solution Section:**
- Lead with transformation, not mechanism
- Before/After framing works extremely well
- "What people actually want: [simple truth]"
- Show the contrast between old way and new way
- Keep it visceral and relatable

**Social Proof Section:**
- Quantified results over generic testimonials ("840% lead increase" not "great service")
- Specific numbers: dollar amounts, percentages, timeframes
- Real names, real photos, real titles
- Multiple testimonials addressing different concerns
- Case study cards with before/after metrics

**Process Section:**
- Maximum 3 steps
- Each step gets a clear label, brief description, and visual icon
- Numbered with large, visible step indicators
- This section exists to make the complex feel simple

**Pricing Section:**
- 2-3 tiers maximum, one marked as "Popular" or "Recommended"
- Show the value clearly — what's included at each level
- Risk reversal (money-back guarantee, satisfaction promise)
- "Starting at $X" is better than hiding price entirely
- Subscription framing reduces perceived cost vs. one-time

**FAQ Section:**
- Address real objections, not softballs
- Expandable accordion format
- 6-8 questions maximum
- Write answers that sell, not just inform

**Footer CTA:**
- Restate the core promise in different words
- "Not sure if [Product] is right for you? Let's chat."
- One final clear action button

---

## Visual Hierarchy Rules

### Typography System

Use distinct display/body font pairings. Typography does heavy lifting for hierarchy:

- **Headlines**: Large, distinctive display font. Serif italic for editorial feel, bold geometric sans for tech products.
- **Body**: Clean, readable sans-serif or monospace depending on context.
- **UI/Labels**: Monospace, small, uppercase with wide letter-spacing, low opacity.
- **Stats/Numbers**: Extra large, bold, high contrast. Numbers should punch.

**Hierarchy through layered opacity (especially on dark backgrounds):**
```
Primary text:    white/90 or text-white
Secondary text:  white/60 or text-gray-300
Tertiary text:   white/40 or text-gray-500
Labels/meta:     white/30 with tracking-[0.2em] uppercase
```

### Spacing & Layout

- 8px grid system, always
- Generous padding inside sections (py-20 to py-32)
- Max content width of 4xl to 6xl for readability
- Text line length: 45-75 characters (max-w-xl to max-w-2xl for paragraphs)
- Section separators: subtle borders (border-white/[0.05]) or spacing, not heavy dividers
- Mobile-first: everything must work on phones before desktop polish

### Color Approach

- **Dark base**: Near-black tones (#0a0a0c, slate-900, gray-950), not pure black
- **Text on dark**: White with varying opacity levels (see hierarchy above)
- **Accent colors**: One strong accent per project, used sparingly. Never more than 2-3 total.
- **Semantic color usage:**
  - Red = critical/error/danger
  - Yellow = warning/caution
  - Blue = information
  - Green = success/positive
  - Purple = discovery/insight
- **Gradients**: Subtle and purposeful. Gradient borders and accent glows work better than gradient backgrounds.
- **For light themes**: Natural palettes (beige, olive, earth tones) over sterile whites.

### Animation & Motion

- Purposeful, never decorative — if it distracts, remove it
- 150-300ms for micro-interactions
- Ease-out for entrances
- Scroll-driven reveals for hero sequences
- Subtle hover states: 5-10% darken or background shift, not dramatic transforms
- Loading skeletons over spinners
- One orchestrated page-load animation beats scattered micro-interactions
- If scroll transitions break the page, remove them — function over flair

---

## Marketing Copy & Messaging

### Voice Principles

Copy should be direct, personal, and conversational.

**Do:**
- Second person ("your", "you") — always address the reader directly
- Short sentences for impact. Longer ones for explanation.
- Confident without being arrogant
- Specific over vague ("840% lead increase" not "dramatically more leads")
- Honest about limitations

**Don't:**
- Generic language ("We leverage cutting-edge solutions")
- Passive voice ("Websites are built by our team")
- Buzzwords ("Synergize your digital transformation")
- Overpolished corporate tone — some roughness is authentic

### Copy Patterns

**Hero Headlines:**
- "[Verb] your [thing] [benefit clause]"
- Examples: "Build your fitness empire without the complexity or compromise", "Never miss another token launch", "Imagine what's possible when AI remembers everything"

**Subheads:**
- State the specific benefit or transformation
- Address one key anxiety: "No contracts, no BS, just results."

**Problem Statements:**
- Use "Here's the trap:" or "But here's the problem:" as pivots
- Name the pain directly in the audience's own language

**CTAs:**
- Primary: Action-oriented verb + clear outcome ("Book a Free Strategy Call", "View on GitHub", "Get Started")
- Secondary: Lower commitment ("See Client Results", "Learn More")
- Never more than 2 CTAs visible at once
- Repeat the primary CTA at multiple scroll points (minimum: hero, mid-page, footer)

### Benefits Over Features

Every section should answer "so what?" from the visitor's perspective.

| Feature (Don't Lead With) | Benefit (Lead With) |
|---|---|
| Three-layer architecture | Your AI remembers everything about you |
| Responsive development | Your website looks perfect on every device |
| 2.9% fee structure | Keep more of what you earn |
| Observer/note-taker pattern | One agent watches, learns, and remembers |

### Social Proof Copy

- Specific numbers always: "$45k MRR", "840% increase", "20x ROI in year 1"
- Attribution: Real name, role, company. With photo when possible.
- Pull quotes that mention specific outcomes, not generic praise
- Case study cards: business type badge, headline result, specific metrics, brief quote

---

## Conversion Optimization

### CTA Strategy

- Sticky nav with persistent CTA button on long pages
- Multiple CTA placements: hero, after social proof, after pricing, footer
- Single primary action per page — don't split attention
- Risk reversal near pricing: "30-day money-back guarantee", "If you're not stoked, request a refund"
- Scheduling integration (Calendly, SavvyCal) for "Book a call" CTAs — reduce friction

### Information Architecture for Conversion

```
Awareness  → Hero + Problem (they realize they have the pain)
Interest   → Solution + Social Proof (they see you can solve it)
Desire     → Process + Pricing (they understand the path and cost)
Action     → CTA + FAQ + Risk Reversal (they have no reason not to)
```

### Objection Handling

The FAQ section is a conversion tool, not an afterthought:

- "Is this right for me?" → Qualify the audience clearly
- "How long does it take?" → Set clear timelines
- "What if it doesn't work?" → Guarantee or risk reversal
- "How is this different from [competitor/DIY]?" → Specific differentiators
- "Can I talk to someone first?" → Low-friction contact option

---

## Responsive Design

### Breakpoint Rules

- Mobile-first, always. Design for phones, then expand.
- Tailwind breakpoints: Use `sm:`, `md:`, `lg:` systematically
- Touch targets: Minimum 44px × 44px, preferably 48px
- Mobile text: 16px minimum body text (prevents iOS zoom)
- Stack vertically on mobile: Horizontal layouts become vertical
- Hide non-essential elements on mobile rather than cramming
- Test at real device widths, not just "make the browser narrow"

### Common Responsive Patterns

```
Hero:         Full-width, reduced padding on mobile, stacked CTAs
Nav:          Hamburger on mobile with full-screen overlay
Grid cards:   3-col desktop → 2-col tablet → 1-col mobile
Stats strip:  Horizontal row → stacked or 2×2 grid
Pricing:      Side-by-side → stacked with swipe
Testimonials: Carousel on mobile, grid on desktop
```

---

## Project-Type Reference

Aesthetic direction varies by product category:

### Developer/Technical Products
- Dark theme
- Monospace for UI elements
- Serif italic for editorial headlines
- Subtle noise texture and scanlines
- Numbered, uppercase, wide-tracked section labels
- Stats displayed prominently with large bold numbers

### Consumer/Lifestyle Products
- Light or dark depending on brand
- Warmer palettes: beige, olive, earth tones, soft blues
- Elegant serif headlines, clean sans body text
- More photography, less illustration
- Approachable, warm copy tone

### DeFi/Trading Products
- Dark theme
- Animated elements: live data, notification banners, real-time updates
- Neon accents (green for gains, red for losses)
- Glassmorphism cards with backdrop blur
- Wallet connection as first-class UI element
- "How it works" must be dead simple — 3 steps max
- Trust signals: audit badges, lock icons, transparency

### Agency/Services
- Professional but not boring
- Split hero: copy left, social proof/image right
- Methodology section with numbered phases
- Real client testimonials with photos and metrics
- Tiered pricing with "Popular" indicator
- "Book a call" as primary CTA throughout

---

## Implementation Checklist

Before shipping any landing page:

### Visual
- [ ] Fonts loaded and rendering correctly
- [ ] Color palette is cohesive (2-3 colors max plus semantic colors)
- [ ] Visual hierarchy is clear at a glance
- [ ] Spacing follows 8px grid
- [ ] No orphaned headings or widowed lines
- [ ] Images optimized and properly sized

### Copy
- [ ] Hero headline passes the "so what?" test
- [ ] Benefits lead, features support
- [ ] All copy uses second person ("your", "you")
- [ ] Numbers are specific, not vague
- [ ] No buzzwords or corporate speak
- [ ] CTA copy is action-oriented

### UX
- [ ] Primary CTA visible without scrolling
- [ ] Page loads fast (no heavy animations on initial load)
- [ ] Smooth scroll between sections
- [ ] All interactive elements have hover/focus/active states
- [ ] Mobile experience tested at 375px width
- [ ] Touch targets are minimum 44px
- [ ] No horizontal scroll on any breakpoint
- [ ] Keyboard navigation works

### Conversion
- [ ] Single clear primary action per page
- [ ] CTA repeated at minimum 3 scroll points
- [ ] Social proof appears before pricing
- [ ] Risk reversal present near the ask
- [ ] FAQ addresses top 3 objections
- [ ] Contact/booking friction is minimal
