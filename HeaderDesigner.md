# Header UI – Designer Specification

Document version: 1.1  
Last updated: January 27, 2026  
Scope: Full header + mega menus for EduMeUp landing page (desktop, tablet, mobile).

---

## 1) Objectives
- Sticky, low-profile bar that keeps primary paths visible (Start Study, Who We Serve, About, Resources, Pricing, My Account, Start Diagnostic).
- Mega menu for Start Study (grade/subject/featured) to surface deep IA quickly.
- Clear CTAs: secondary “My Account”, primary “Start Diagnostic →”.
- Mobile overlay with generous touch targets and same IA depth.

---

## 2) Layout & Sizing
- Height: 80px desktop, 70px tablet, 64px mobile.
- Padding: 24px desktop, 20px tablet, 16px mobile.
- Structure: Logo (200px area, logo 180px) | Nav (center, 32px link gap) | CTAs (right).
- Background: White #FFFFFF; Shadow: 0 2px 8px rgba(0,0,0,0.06); Sticky with z-index 1000.

ASCII (desktop):
```
[Logo 180w]   Start Study ▾  Who We Serve ▾  About ▾  Resources ▾  Pricing    [My Account] [Start Diagnostic →]
```

---

## 3) Navigation & Menus

### Start Study (Mega Menu, full-width up to 1200px)
- Padding 40px; three columns (40% / 30% / 30%).
- Column 1 (Grade Level): Starter Primary, Lower Primary, Upper Primary, Get Ready (⭐ UNIQUE badge, gold border), O-Level/IGCSE, FSc/Intermediate. Icons per item; description line 14px.
- Column 2 (Subject): Mathematics, English, Physics, Chemistry, Biology, “View All Subjects →”.
- Column 3 (Featured/Quick): Featured Get Ready card (light blue, 2px border #BFDBFE, gold badge, CTA), Quick links list (Diagnostic, All Courses, Sample Lessons, Pricing).

### Who We Serve (Dropdown 280px)
- Vertical list with icon + title + 13px description: Students, Parents, Homeschool Families, Teachers, Schools; divider; “Compare Solutions →”.

### About (Dropdown 300px)
- Our Story, How It Works, Research & Validation (UNIVERSITY-PROVEN badge), Our Team, Success Stories; divider; Why Choose EduMeUp? →

### Resources (Dropdown 320px)
- Section “Learning Resources”: Blog, Sample Lessons, Past Papers Library, Parent Guide. Divider. Section “Support”: Help Center, Contact Us, Schedule Demo.

### Pricing
- Single link, no dropdown.

### Right CTAs
- My Account: outline Deep Blue, 140×40px, radius 6px, hover light blue.
- Start Diagnostic: solid Deep Blue, 180×44px, radius 6px, shadow, hover darker + lift 2px.

---

## 4) Visual System
- Text color: Dark Navy #1A2B3C; Hover/active: Deep Blue #1E40AF; Body Gray #4A5568; Dividers #E5E7EB.
- Fonts: Montserrat Semibold 15-16px (links), Montserrat Bold 15-16px (CTA), Open Sans 14px for descriptions.
- Active state: underline 2px Deep Blue + color change.

---

## 5) States & Interactions
- Hover: underline links; CTAs lift 2px (primary) or fill light blue (secondary).
- Focus: 3px #60A5FA outline offset 2px on all interactive items.
- Dropdowns: appear on hover/focus desktop; close on mouseleave; shadow 0 4px 12px rgba(0,0,0,0.1); radius 8px.
- Mega menu: full-width panel below header; no layout shift.

---

## 6) Mobile / Tablet
- Header row: logo left (120px), hamburger right (24px icon, 44×44 hit); height 64px.
- Overlay menu: fixed full-screen white; slide-in 300ms ease-out; close “×” 32px in 44×44 hit.
- Menu list: 20px text, 20px vertical padding, dividers #E5E7EB; CTA full-width 52px.
- Retain IA: include Start Study sub-links, Who We Serve items, About, Resources, Pricing, My Account, Start Diagnostic.

---

## 7) Accessibility
- Contrast: text ≥4.5:1, icons/lines ≥3:1.
- Focus visible everywhere; skip link recommended above header.
- ARIA: nav has `role="navigation"`; hamburger `aria-expanded`/`aria-controls`; menus `role="menu"` with proper labelling.
- prefers-reduced-motion: disable slide/hover lifts (instant show/hide).

---

## 8) Assets
- Logo SVG (light on dark optional), hamburger/close SVG 24px, chevron 12px, badges (gold for UNIQUE/FEATURED).

---

## 9) Checklist (Designer)
- Heights respected (80/70/64); 32px desktop link gaps.
- Mega menu columns align; featured card distinct; Get Ready link has gold badge/border.
- Touch targets ≥44px; no horizontal scroll at 320px.
- CTA prominence: primary more visual weight than secondary.
- Mobile overlay scrollable if overflow; close affordance clear.
