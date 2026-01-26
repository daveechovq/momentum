# Momentum Website - Project Context

## What This Is
Marketing website for **Momentum** - a team development business offering transformational experiences through voice, movement, and music.

**The Team:**
- **Darren Percival** - Voice & Expression (Outward) - The Voice Australia, Gold Record artist
- **Linda Lou Küster** - Movement & Bodywork (Inward) - Psychology Masters, ZenThai Shiatsu
- **Dave Spicer** - Music & Harmony (Connecting) - Jazz pianist, Griffith Conservatorium lecturer

## Core Concept: Three Forces
The offering is built around three complementary energies:
- **Outward** (Darren/Voice) - Expression, confidence, communication - Color: Terracotta
- **Inward** (Linda/Movement) - Grounding, awareness, presence - Color: Forest Green
- **Connecting** (Dave/Music) - The thread that weaves them together - Color: Gold

## File Structure
```
momentum-website/
├── index.html          # Main single-page site
├── css/
│   └── styles.css      # All styles (CSS variables at top)
├── js/
│   └── main.js         # Scroll animations, navigation
├── assets/
│   └── images/         # Photos (placeholders currently)
├── docs/               # Business documents
│   ├── BUSINESS-PLAN.md
│   ├── MARKETING-PLAN.md
│   ├── PRICING-GUIDE.md
│   ├── PARTNERSHIP-AGREEMENT-OUTLINE.md
│   └── FINANCIAL-PROJECTIONS.md
├── LAUNCH-CHECKLIST.md
├── README.md
└── CLAUDE.md           # This file
```

## Design System

### Colors (CSS Variables in styles.css)
```css
--color-cream: #F7F4EF;           /* Background */
--color-warm-white: #FDFCFA;      /* Cards, sections */
--color-sand: #E8E2D9;            /* Borders, subtle backgrounds */
--color-terracotta: #C4785A;      /* Darren / Outward / Primary accent */
--color-forest: #2D4A3E;          /* Linda / Inward / Programs section */
--color-gold: #B8956E;            /* Dave / Connecting */
--color-charcoal: #2C2C2C;        /* Text */
```

### Typography
- **Display:** Cormorant Garamond (Google Fonts)
- **Body:** DM Sans (Google Fonts)

### Tone of Voice
- Warm but confident
- Authentic, not salesy
- Direct, not corporate
- Conversational ("Here's what we've noticed...")

## Page Sections (in order)
1. **Hero** - Main headline, CTA
2. **Truth** - "The honest truth" - why this matters
3. **Forces** - Three Forces visual + cards
4. **How** - Voice, Movement, Music explanation
5. **Who** - Target audiences (Workplaces, Schools, Sports, Events)
6. **Team** - Three facilitators with Outward/Inward/Connecting labels
7. **Programs** - Half-Day ($4,500) and Full-Day ($6,500)
8. **Science** - Research backing
9. **Testimonial** - Placeholder for now
10. **CTA/Contact** - Form (Netlify Forms)
11. **Footer**

## Making Changes

### To edit content:
- Edit `index.html` directly
- Sections are clearly commented

### To edit styles:
- Edit `css/styles.css`
- Colors/fonts are CSS variables at the top
- Sections are labelled with comments

### To edit animations:
- Edit `js/main.js`
- Currently: scroll reveal, smooth scroll, nav scroll state

### Adding photos:
1. Add images to `assets/images/`
2. Update `.team__photo` classes in CSS, or add `<img>` tags in HTML
3. Recommended: WebP format, ~100-200KB each

## Deployment
- Hosted on Netlify
- Deploy via: `git push` (if connected to GitHub)
- Contact form submissions go to Netlify dashboard

## Key Business Info
- **Target:** 2 sessions/week @ $6,000 average = $576K/year
- **Location:** Brisbane, Australia (will travel)
- **Programs:** Half-Day (4hrs, $4,500) / Full-Day (7hrs, $6,500)

## Common Tasks

### Update pricing:
1. Edit `index.html` - Programs section
2. Edit `docs/PRICING-GUIDE.md`

### Add a testimonial:
1. Find `.testimonial` section in `index.html`
2. Update quote text, name, role
3. Add photo to `assets/images/` and update `.testimonial__avatar`

### Change colors:
1. Edit CSS variables in `:root` at top of `css/styles.css`
2. Colors cascade through the whole site

### Add a new section:
1. Follow existing section patterns in `index.html`
2. Add corresponding styles in `css/styles.css`
3. Add `.reveal` class for scroll animation
