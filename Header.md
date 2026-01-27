# Header UI – Designer Specification

Document version: 1.0  
Last updated: January 27, 2026  
Scope: Global site header (logo, primary nav, CTAs, mobile menu) for EduMeUp landing page.

---

## 1) Objectives (Brief)
- Instant brand recognition; keep logo left, CTA right.
- Fast navigation to key sections (Hero, Programs, Services, Comparison, Research, Pricing, FAQ).
- Mobile-first: uncluttered hamburger overlay, 44px+ touch targets.
- Keep vertical height tight (64-72px desktop) to maximize above-the-fold hero.
- Strong contrast and legibility against light backgrounds; sticky option allowed if performance OK.

---

## 2) Layout & Sizing
- Container: max-width 1200px (desktop), 24px side padding desktop, 20px tablet, 16px mobile.
- Height: 68px desktop, 64px tablet, 60px mobile.
- Grid: 3 zones (Logo | Nav links | CTA). CTA may collapse to icon on tablet; hidden on mobile overlay.
- Spacing: 16px gap between links desktop; 12px tablet; 10px mobile overlay vertical list.

ASCII layout (desktop):
```
[Logo 140w]   Home  Programs  Services  Comparison  Research  Pricing  FAQ      [Primary CTA]
```

Mobile overlay layout:
```
┌─────────────────────────┐
│ Logo               ✕    │
│                        │
│ > Home                 │
│ > Programs             │
│ > Services             │
│ > Comparison           │
│ > Research             │
│ > Pricing              │
│ > FAQ                  │
│                        │
│ [Start Free Diagnostic]│
└─────────────────────────┘
```

---

## 3) Color & Typography
- Background: white (#FFFFFF). Optional subtle shadow: 0 2px 12px rgba(0,0,0,0.06).
- Text: Dark Navy (#1A2B3C); Hover: Deep Blue (#1E40AF).
- CTA: Primary Vibrant Blue (#0066CC), hover #0052A3.
- Active link underline: 2px Deep Blue.
- Fonts: Headings/links Montserrat Semibold 15-16px; CTA Montserrat Bold 15-16px.

---

## 4) States & Interactions
- Hover: link underline; CTA lifts 2px + stronger shadow.
- Focus: 3px #60A5FA outline, offset 2px.
- Active (mouse-down): remove lift, darker bg.
- Current page/section: underline + color Deep Blue.
- Sticky option: add 1px bottom border #E5E7EB when stuck.

---

## 5) Mobile Menu (Hamburger)
- Icon size: 24px, hit area 44x44px, right-aligned.
- Overlay: white background, slide-in from right 300ms ease-out, z-index 2000.
- Close icon: 32px inside 44x44 hit area, 16px from edges.
- Link rows: 20px text, 20px vertical padding, divider 1px #E5E7EB.
- CTA inside overlay: full-width button, 52px height.

---

## 6) Responsive Rules
- xl (1200+): show full nav + CTA.
- lg (1024-1199): show full nav; shrink gaps; CTA medium width.
- md (768-1023): allow optional collapse of 1-2 low-priority links into "More" dropdown; CTA medium.
- sm/xs (<768): hide nav links; show hamburger + logo + optional small CTA icon; overlay handles navigation.
- Touch targets: 44px min; side padding 16px on mobile.

---

## 7) Content Slots (Header)
- Logo: SVG, 140px width desktop, 120px tablet, 110px mobile.
- Primary links (suggested): Home, Programs, Services, Comparison, Research, Pricing, FAQ.
- CTA text: "START FREE DIAGNOSTIC" (primary). Optional secondary text-only link: "View Features".

---

## 8) Accessibility
- Maintain 4.5:1 contrast for text; 3:1 for icons/lines.
- Focus visible on all interactive elements.
- ARIA: hamburger button `aria-expanded`, `aria-controls`; set `role="navigation"` on nav.
- Skip link recommended (positions above header).
- `prefers-reduced-motion`: disable slide animation; instant show/hide.

---

## 9) Assets
- Logo SVG (light and dark if needed).
- Hamburger/close icons as SVG (24px).
- No background images needed for header.

---

## 10) Checklist (Designer)
- Links readable at 100% zoom on 320px wide.
- Touch targets ≥44px.
- Active state visible for current section.
- CTA stands out vs links.
- Mobile overlay scrolls if content exceeds height.
- Shadow/border subtle; header not overpowering hero.
