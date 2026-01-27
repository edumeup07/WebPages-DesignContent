# 🎨 EDUMEUP LANDING PAGE - DESIGNER SPECIFICATIONS

**Document Version:** 1.0  
**Last Updated:** January 27, 2026  
**Purpose:** Complete visual design specifications for UI/UX designers

---

## 📋 TABLE OF CONTENTS

1. [Design System Overview](#design-system-overview)
2. [Typography System](#typography-system)
3. [Color Palette](#color-palette)
4. [Spacing & Layout System](#spacing--layout-system)
5. [Component Specifications](#component-specifications)
6. [Section-by-Section Design](#section-by-section-design)
7. [Image Requirements & Prompts](#image-requirements--prompts)
8. [Responsive Design Guidelines](#responsive-design-guidelines)
9. [Animation & Interaction States](#animation--interaction-states)
10. [Accessibility Requirements](#accessibility-requirements)

---

## 🎯 DESIGN SYSTEM OVERVIEW

### Brand Personality

| Attribute | Description |
|-----------|-------------|
| **Tone** | Professional, trustworthy, research-backed |
| **Mood** | Aspirational, optimistic, empowering |
| **Style** | Modern, clean, technology-forward but warm |
| **Aesthetic** | Netflix/Spotify-style UI with educational warmth |

### Design Principles

```
1. CLARITY FIRST
   - Clean, uncluttered layouts
   - Clear visual hierarchy
   - Generous white space
   
2. RESEARCH-BACKED CREDIBILITY
   - Statistics prominently displayed
   - Academic/professional feel
   - Trust indicators throughout
   
3. PROGRESSIVE DISCLOSURE
   - "Read More" expandable sections
   - Don't overwhelm with information
   - Let users choose depth
   
4. STAKEHOLDER-SPECIFIC PATHS
   - Clear audience segmentation
   - Tailored messaging per segment
   - Easy navigation to relevant sections
```

---

## 📝 TYPOGRAPHY SYSTEM

### Font Families

| Usage | Font Family | Fallback |
|-------|-------------|----------|
| **Headings** | Montserrat | Arial, sans-serif |
| **Body Text** | Open Sans | Helvetica, sans-serif |
| **Code/Data** | Roboto Mono | monospace |

### Heading Scale

```
HEADING HIERARCHY
═══════════════════════════════════════════════════════════════

H1 (Hero Headline)
├── Font: Montserrat ExtraBold (800)
├── Size: 56px
├── Line Height: 1.1
├── Letter Spacing: -0.02em
└── Color: Dark Navy (#1A2B3C)

H2 (Section Titles)
├── Font: Montserrat Bold (700)
├── Size: 42px
├── Line Height: 1.2
├── Letter Spacing: -0.01em
└── Color: Dark Navy (#1A2B3C)

H3 (Subsection Titles)
├── Font: Montserrat SemiBold (600)
├── Size: 28px
├── Line Height: 1.3
└── Color: Dark Navy (#1A2B3C)

H4 (Card Titles)
├── Font: Montserrat SemiBold (600)
├── Size: 20-24px
├── Line Height: 1.4
└── Color: Dark Navy (#1A2B3C)

H5 (Small Headings)
├── Font: Montserrat SemiBold (600)
├── Size: 16-18px
├── Line Height: 1.4
└── Color: Dark Navy (#1A2B3C)

H6 (Label Headings)
├── Font: Montserrat Medium (500)
├── Size: 14px
├── Line Height: 1.4
└── Color: Medium Gray (#718096)
```

### Body Text Scale

| Type | Size | Weight | Line Height | Usage |
|------|------|--------|-------------|-------|
| **Large Body** | 18-20px | Regular (400) | 1.7 | Hero supporting text, key paragraphs |
| **Regular Body** | 16-17px | Regular (400) | 1.6-1.7 | Main content, descriptions |
| **Small Body** | 14-15px | Regular (400) | 1.6 | Card descriptions, secondary text |
| **Caption** | 12-13px | Regular (400) | 1.5 | Fine print, disclaimers |
| **Micro** | 11px | Regular (400) | 1.4 | Legal text, footnotes |

### Special Text Styles

```
PRE-HEADLINE BADGE
├── Font: Montserrat SemiBold
├── Size: 14px
├── Color: Deep Blue (#1E40AF)
├── Background: Light Blue (#DBEAFE)
├── Padding: 8px 16px
├── Border Radius: 20px
└── Text Transform: None

STAT NUMBER (Large)
├── Font: Montserrat ExtraBold
├── Size: 48px
├── Color: Deep Blue (#1E40AF)
└── Line Height: 1.0

STAT LABEL
├── Font: Open Sans Regular
├── Size: 16px
├── Color: Medium Gray (#4A5568)
└── Line Height: 1.4

QUOTE TEXT
├── Font: Open Sans Italic
├── Size: 20px
├── Color: Dark Gray (#4A5568)
├── Line Height: 1.7
└── Border Left: 4px solid Deep Blue

LINK TEXT
├── Font: Open Sans SemiBold
├── Size: Inherit from parent
├── Color: Deep Blue (#1E40AF)
├── Hover: Underline
└── Cursor: Pointer
```

---

## 🎨 COLOR PALETTE

### Primary Colors

```
┌─────────────────────────────────────────────────────────────────┐
│  PRIMARY COLORS                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ████████  Deep Blue        #1E40AF                            │
│            RGB: 30, 64, 175                                     │
│            Usage: Primary CTAs, headers, key accents            │
│                                                                 │
│  ████████  Dark Navy        #1A2B3C                            │
│            RGB: 26, 43, 60                                      │
│            Usage: Headings, primary text, footer                │
│                                                                 │
│  ████████  Vibrant Blue     #0066CC                            │
│            RGB: 0, 102, 204                                     │
│            Usage: Alternate CTAs, links                         │
│            Hover: #0052A3                                       │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Secondary Colors

```
┌─────────────────────────────────────────────────────────────────┐
│  SECONDARY COLORS (Stakeholder/Feature Specific)               │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ████████  Success Green    #10B981                            │
│            RGB: 16, 185, 129                                    │
│            Usage: Success states, guarantees, improvements      │
│            Light: #ECFDF5                                       │
│                                                                 │
│  ████████  Premium Gold     #F59E0B                            │
│            RGB: 245, 158, 11                                    │
│            Usage: Get Ready, premium features, popular badge    │
│            Hover: #D97706                                       │
│            Light: #FEF3C7                                       │
│                                                                 │
│  ████████  Parent Orange    #EA580C                            │
│            RGB: 234, 88, 12                                     │
│            Usage: Parent-focused content, urgency               │
│            Light: #FFF7ED                                       │
│                                                                 │
│  ████████  Teacher Purple   #7C3AED                            │
│            RGB: 124, 58, 237                                    │
│            Usage: Teacher content, tutoring                     │
│            Light: #F3E8FF                                       │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Neutral Colors

```
┌─────────────────────────────────────────────────────────────────┐
│  NEUTRAL COLORS                                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ████████  Dark Gray        #4A5568                            │
│            Usage: Body text, descriptions                       │
│                                                                 │
│  ████████  Medium Gray      #718096                            │
│            Usage: Secondary text, placeholders                  │
│                                                                 │
│  ████████  Light Gray       #F3F4F6                            │
│            Usage: Card backgrounds, inactive tabs               │
│                                                                 │
│  ████████  Border Gray      #E5E7EB                            │
│            Usage: Borders, dividers                             │
│                                                                 │
│  ████████  White            #FFFFFF                            │
│            Usage: Backgrounds, text on dark                     │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

### Background Colors

| Background Type | Color | Hex Code | Usage |
|-----------------|-------|----------|-------|
| **Primary White** | White | #FFFFFF | Main sections |
| **Light Blue 1** | Very Light Blue | #F0F9FF | Hero gradient end |
| **Light Blue 2** | Light Blue | #EFF6FF | Alternate sections |
| **Light Blue 3** | Blue Tint | #DBEAFE | Stats bar, badges |
| **Light Green** | Success Background | #ECFDF5 | Savings, guarantees |
| **Light Orange** | Parent Background | #FFF7ED | Parent-focused |
| **Light Purple** | Teacher Background | #FAF5FF | Teacher-focused |
| **Deep Blue Gradient** | Blue to Darker | #1E40AF → #1E3A8A | Final CTA |
| **Dark Navy** | Footer | #1A2B3C | Footer background |
| **Darker Navy** | Footer Bottom | #0F172A | Copyright bar |

### Color Usage by Stakeholder

```
STAKEHOLDER COLOR MAPPING
═══════════════════════════════════════════════════════════════

Students     → Deep Blue (#1E40AF)
               Light: #DBEAFE, #EFF6FF
               
Parents      → Orange (#EA580C)
               Light: #FFF7ED
               
Homeschool   → Green (#10B981)
               Light: #ECFDF5
               
Schools      → Teal (#0891B2)
               Light: #ECFEFF
               
Teachers     → Purple (#7C3AED)
               Light: #F3E8FF
               
Get Ready    → Gold (#F59E0B)
               Light: #FEF3C7
```

---

## 📐 SPACING & LAYOUT SYSTEM

### Base Spacing Scale

```
SPACING TOKENS (Base: 4px)
═══════════════════════════════════════════════════════════════

--space-1:    4px     (0.25rem)   │ Tight gaps
--space-2:    8px     (0.5rem)    │ Small gaps
--space-3:    12px    (0.75rem)   │ Icon gaps
--space-4:    16px    (1rem)      │ Standard gap
--space-5:    20px    (1.25rem)   │ Medium gap
--space-6:    24px    (1.5rem)    │ Component gap
--space-8:    32px    (2rem)      │ Section element gap
--space-10:   40px    (2.5rem)    │ Large gap
--space-12:   48px    (3rem)      │ Section heading margin
--space-16:   64px    (4rem)      │ Section padding (mobile)
--space-20:   80px    (5rem)      │ Section padding (desktop)
--space-24:   96px    (6rem)      │ Large section padding
--space-25:   100px   (6.25rem)   │ Hero top padding
```

### Section Padding

| Section Type | Desktop | Tablet | Mobile |
|--------------|---------|--------|--------|
| **Hero** | 100px top, 80px bottom | 80px top, 60px bottom | 60px top, 40px bottom |
| **Standard Section** | 80px top/bottom | 60px top/bottom | 40px top/bottom |
| **Compact Section** | 60px top/bottom | 48px top/bottom | 32px top/bottom |
| **Footer** | 60px top, 40px bottom | 48px top, 32px bottom | 40px top, 24px bottom |

### Container Widths

```
CONTAINER SYSTEM
═══════════════════════════════════════════════════════════════

Max Width Containers:
├── Full Width:     1400px (Hero sections)
├── Standard:       1200px (Most sections)
├── Narrow:         1100px (Text-heavy sections)
├── Compact:        1000px (Focused content)
├── Text Column:    900px  (FAQ, text blocks)
└── Centered Text:  800-850px (Subheadings)

Side Padding (within containers):
├── Desktop:   24-32px
├── Tablet:    20-24px
└── Mobile:    16-20px
```

### Grid System

```
COLUMN GRID (12-Column Base)
═══════════════════════════════════════════════════════════════

Desktop (1200px+):
┌────┬────┬────┬────┬────┬────┬────┬────┬────┬────┬────┬────┐
│ 1  │ 2  │ 3  │ 4  │ 5  │ 6  │ 7  │ 8  │ 9  │ 10 │ 11 │ 12 │
└────┴────┴────┴────┴────┴────┴────┴────┴────┴────┴────┴────┘
Column: ~83px  |  Gutter: 24px  |  Total: 1200px

Common Layouts:
├── 2 columns:  6+6 (50% / 50%)
├── Hero:       7+5 (55% / 45%) or 6+6
├── 3 columns:  4+4+4 (33.3% each)
├── 4 columns:  3+3+3+3 (25% each)
├── 5 columns:  20% each (stakeholder cards)
└── 6 columns:  2+2+2+2+2+2 (program cards 3×2)

Tablet (768px - 1199px):
├── 2 columns → 2 columns (narrower)
├── 3 columns → 2 columns
├── 4+ columns → 2 columns
└── 5+ columns → 2-3 columns

Mobile (< 768px):
└── All layouts → Single column stack
```

---

## 🧩 COMPONENT SPECIFICATIONS

### Button Styles

```
PRIMARY CTA (Large)
═══════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────┐
│              START FREE DIAGNOSTIC TEST →                   │
└─────────────────────────────────────────────────────────────┘

Dimensions:     380-420px × 64-72px
Background:     #0066CC (Vibrant Blue)
Text:           White, 20-22px, Montserrat Bold
Border Radius:  8px
Box Shadow:     0px 4px 12px rgba(0,102,204,0.3)
Padding:        20px 40px

Hover State:
├── Background: #0052A3 (Darken 15%)
├── Transform: translateY(-2px)
└── Box Shadow: 0px 6px 16px rgba(0,102,204,0.4)

Active State:
├── Transform: translateY(0)
└── Box Shadow: 0px 2px 8px rgba(0,102,204,0.3)

Focus State:
├── Outline: 3px solid #60A5FA
└── Outline Offset: 2px


SECONDARY CTA (Medium)
═══════════════════════════════════════════════════════════════
Dimensions:     260-300px × 48-56px
Background:     #1E40AF (Deep Blue)
Text:           White, 16-18px, Montserrat SemiBold
Border Radius:  6-8px
Box Shadow:     0px 2px 8px rgba(30,64,175,0.25)


TERTIARY CTA (Small/Outline)
═══════════════════════════════════════════════════════════════
Dimensions:     180-220px × 40-44px
Background:     Transparent
Border:         2px solid #1E40AF
Text:           #1E40AF, 14-16px, Montserrat SemiBold
Border Radius:  6px

Hover:
├── Background: #1E40AF
└── Text: White


TEXT LINK BUTTON
═══════════════════════════════════════════════════════════════
Background:     None
Text:           #1E40AF, 16px, Open Sans SemiBold
Decoration:     None
Hover:          Underline
Icon:           → (arrow) if navigational
```

### Card Styles

```
STANDARD CARD
═══════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────┐
│  [Icon 64px]                                                │
│                                                             │
│  Card Title                                                 │
│  Subtitle / Age Range                                       │
│                                                             │
│  Description text goes here with 2-3 sentences             │
│  explaining the content of this card.                       │
│                                                             │
│  ✓ Feature one                                             │
│  ✓ Feature two                                             │
│  ✓ Feature three                                           │
│                                                             │
│  Learn More →                                               │
└─────────────────────────────────────────────────────────────┘

Properties:
├── Background:     White
├── Border:         2px solid #BFDBFE (Light Blue)
├── Border Radius:  12px
├── Padding:        32px
├── Min Height:     320px
└── Box Shadow:     0px 2px 8px rgba(0,0,0,0.08)

Hover State:
├── Transform:      translateY(-4px)
├── Box Shadow:     0px 8px 24px rgba(0,0,0,0.12)
└── Border Color:   #93C5FD (Slightly darker)


TESTIMONIAL CARD
═══════════════════════════════════════════════════════════════
┌─────────────────────────────────────────────────────────────┐
│       ┌──────────┐                                          │
│       │  Photo   │                                          │
│       │ (Circle) │                                          │
│       └──────────┘                                          │
│                                                             │
│  Name - Achievement Title                                   │
│  ┌──────────────────────────────────────────────────────┐  │
│  │ ⭐ Achievement Badge                                  │  │
│  └──────────────────────────────────────────────────────┘  │
│                                                             │
│  ┌────────────────────────────────────────────────────┐    │
│  │ BEFORE: 45%    │    AFTER: 91%                     │    │
│  │ Outcome: University Acceptance                      │    │
│  └────────────────────────────────────────────────────┘    │
│                                                             │
│  "Quote text with testimonial content that wraps to        │
│   multiple lines as needed..."                              │
│                                                             │
│  — Attribution, Location | Since Year                       │
└─────────────────────────────────────────────────────────────┘

Properties:
├── Background:     White
├── Border:         2px solid #BFDBFE
├── Border Radius:  12px
├── Padding:        32px
├── Min Height:     380px
├── Width:          32% desktop / 100% mobile
└── Box Shadow:     0px 4px 12px rgba(0,0,0,0.08)

Photo:
├── Size:           80-120px diameter
├── Shape:          Circle (border-radius: 50%)
├── Border:         3px solid White
└── Shadow:         0px 2px 8px rgba(0,0,0,0.15)

Stats Box:
├── Background:     #ECFDF5 (Light Green)
├── Border:         2px solid #10B981 (Green)
├── Padding:        16px
├── Border Radius:  8px
└── Numbers:        28px, Montserrat ExtraBold, #065F46


SERVICE CARD (Tabbed Interface)
═══════════════════════════════════════════════════════════════
Properties:
├── Background:     #F0F9FF (Light Blue)
├── Border:         1px solid #BFDBFE
├── Padding:        24px
├── Border Radius:  8px
├── Min Height:     200px
└── Icon:           48px
```

### Badge/Tag Styles

```
BADGE TYPES
═══════════════════════════════════════════════════════════════

PRE-HEADLINE BADGE
┌─────────────────────────────────────────────────────────────┐
│ 🏆 World's First Complete Educational Ecosystem             │
└─────────────────────────────────────────────────────────────┘
├── Background:     #DBEAFE
├── Border:         None
├── Text:           #1E40AF, 14px, Montserrat SemiBold
├── Padding:        8px 16px
├── Border Radius:  20px (pill shape)
└── Display:        Inline-block


FEATURE BADGE (Unique/Special)
┌───────────────────────────┐
│ ⭐ UNIQUE TO EDUMEUP      │
└───────────────────────────┘
├── Background:     #F59E0B (Gold)
├── Text:           White, 12px, Montserrat Bold
├── Padding:        6px 12px
├── Border Radius:  6px
├── Position:       Above card title
└── Text Transform: Uppercase


ACHIEVEMENT BADGE
┌───────────────────────────┐
│ ⭐ O-Level: 5 A* Grades   │
└───────────────────────────┘
├── Background:     #F59E0B (Gold)
├── Text:           White, 13px, Montserrat Bold
├── Padding:        6px 12px
└── Border Radius:  12px (pill)


STAKEHOLDER BADGE
┌────────────────────────────────────┐
│ 👨‍👩‍👧‍👦 Mother of Two O-Level Students │
└────────────────────────────────────┘
├── Background:     Varies by stakeholder
├── Text:           White, 13px, Montserrat Bold
├── Padding:        6px 12px
└── Border Radius:  12px


PROOF PILLS (Inline Trust Indicators)
┌─────────────────────────────────────┐
│ ✓ 2,000+ Students, 25+ Countries   │
└─────────────────────────────────────┘
├── Background:     #ECFDF5 (Light Green)
├── Border:         2px solid #10B981
├── Text:           #065F46, 14px, Open Sans SemiBold
├── Padding:        10px 20px
├── Border Radius:  24px (pill)
└── Display:        Inline-flex with gap
```

### Table Styles

```
COMPARISON TABLE
═══════════════════════════════════════════════════════════════

Container:
├── Background:     White
├── Border:         2px solid #1E40AF
├── Border Radius:  12px
├── Box Shadow:     0px 4px 16px rgba(30,64,175,0.15)
├── Overflow:       Hidden (for rounded corners)
└── Width:          100% (max 1100px)

Header Row:
├── Background:     #1E40AF (Deep Blue)
├── Text:           White, 16px, Montserrat Bold
├── Padding:        20px
├── Position:       Sticky on scroll
└── Border Bottom:  None

EduMeUp Column (Highlighted):
├── Background:     #ECFDF5 (Light Green)
├── Text:           #1A2B3C, 15px, Open Sans Regular
└── Border Right:   2px solid #10B981

Competitor Columns:
├── Background:     White
├── Text:           #4A5568, 15px, Open Sans Regular
└── Border Right:   1px solid #E5E7EB

Row Styling:
├── Padding:        16px 20px
├── Border Bottom:  1px solid #E5E7EB
├── Vertical Align: Top
└── Hover:          Background #F9FAFB

Feature Icons:
├── ✅ Comprehensive: Green (#10B981)
├── ⚠️ Partial:      Orange (#F59E0B)
└── ❌ Absent:       Red (#EF4444)

Footer Note:
├── Background:     #F9FAFB
├── Text:           #718096, 13px, Open Sans Italic
└── Padding:        20px
```

### Tab Interface

```
TABBED INTERFACE (Services Section)
═══════════════════════════════════════════════════════════════

Tab Bar:
├── Layout:         Horizontal, flex
├── Gap:            4px between tabs
├── Background:     None
└── Border Bottom:  2px solid #E5E7EB

Inactive Tab:
├── Background:     #F3F4F6 (Light Gray)
├── Text:           #4A5568, 16px, Montserrat SemiBold
├── Padding:        12px 24px
├── Border Radius:  8px 8px 0 0
├── Border:         None
└── Cursor:         Pointer

Active Tab:
├── Background:     #1E40AF (Deep Blue)
├── Text:           White
├── Border Bottom:  2px solid #1E40AF (covers container border)
└── Transform:      translateY(2px) to overlap border

Hover (Inactive):
├── Background:     #E5E7EB
└── Text:           #1A2B3C

Tab Content Area:
├── Background:     White
├── Border:         2px solid #E5E7EB (no top)
├── Border Radius:  0 0 12px 12px
├── Padding:        32px
└── Min Height:     400px
```

### Accordion (FAQ)

```
FAQ ACCORDION
═══════════════════════════════════════════════════════════════

Container:
└── Max Width: 900px centered

Accordion Item (Collapsed):
┌─────────────────────────────────────────────────────────────┐
│  Q: What makes EduMeUp different from Khan Academy?      ▼  │
└─────────────────────────────────────────────────────────────┘
├── Background:     #F9FAFB
├── Border:         1px solid #E5E7EB
├── Border Radius:  8px
├── Padding:        20px
├── Margin Bottom:  12px
├── Cursor:         Pointer
└── Transition:     All 0.3s ease

Question Text:
├── Font:           18px, Montserrat SemiBold
├── Color:          #1A2B3C
└── Padding Right:  40px (for icon)

Expand Icon:
├── Position:       Absolute, right 20px
├── Size:           24px
├── Color:          #4A5568
├── Rotation:       0° collapsed, 180° expanded
└── Transition:     Transform 0.3s ease

Accordion Item (Expanded):
┌─────────────────────────────────────────────────────────────┐
│  Q: What makes EduMeUp different from Khan Academy?      ▲  │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  A: Khan Academy offers free video lectures (passive,      │
│  5-10% retention). EduMeUp offers complete ecosystem...    │
│                                                             │
│  [Read detailed comparison →]                               │
│                                                             │
└─────────────────────────────────────────────────────────────┘
├── Border Color:   #1E40AF
├── Background:     White
└── Box Shadow:     0px 4px 12px rgba(0,0,0,0.08)

Answer Text:
├── Font:           16px, Open Sans Regular
├── Color:          #4A5568
├── Line Height:    1.7
├── Padding:        20px
├── Border Top:     1px solid #E5E7EB
└── Animation:      Slide down 0.3s
```

---

## 📄 SECTION-BY-SECTION DESIGN

### Section 1: Hero

```
HERO SECTION LAYOUT
═══════════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────────────────────────┐
│ [Padding: 100px top]                                                    │
│                                                                         │
│  ┌───────────────────────────────┐ ┌───────────────────────────────┐  │
│  │                               │ │                               │  │
│  │  🏆 Pre-headline Badge        │ │                               │  │
│  │                               │ │                               │  │
│  │  Transform 5% Learning        │ │     [HERO IMAGE]              │  │
│  │  Into 75%+ Mastery With       │ │                               │  │
│  │  Research-Backed Education    │ │     Student with tablet       │  │
│  │                               │ │     showing 45% → 91%         │  │
│  │  Supporting tagline text      │ │     improvement               │  │
│  │  with key statistics...       │ │                               │  │
│  │                               │ │     Neural network            │  │
│  │  [Pill] [Pill] [Pill]        │ │     background elements       │  │
│  │                               │ │                               │  │
│  │  ┌───────────────────────┐   │ │     700px × 600px             │  │
│  │  │ START FREE DIAGNOSTIC │   │ │                               │  │
│  │  └───────────────────────┘   │ │                               │  │
│  │                               │ │                               │  │
│  │  Or explore features →        │ │                               │  │
│  │                               │ │                               │  │
│  │  ✓ Trust  ✓ Trust  ✓ Trust   │ │                               │  │
│  │                               │ │                               │  │
│  │     55% Width                 │ │       45% Width               │  │
│  └───────────────────────────────┘ └───────────────────────────────┘  │
│                                                                         │
│ [Padding: 80px bottom]                                                  │
└─────────────────────────────────────────────────────────────────────────┘

Background: Clean white with subtle gradient to #F0F9FF (light blue)
Max Width: 1400px centered
```

### Section 2: Quick Stats Bar

```
STATS BAR LAYOUT
═══════════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────────────────────────┐
│  Background: #EFF6FF (Light Blue)                                       │
│                                                                         │
│  ┌──────────────┐ ┌──────────────┐ ┌──────────────┐ ┌──────────────┐  │
│  │     🎯       │ │     🧠       │ │     🎓       │ │     💰       │  │
│  │     91%      │ │     75%      │ │     84%      │ │  $7K-29K     │  │
│  │  Pass Rate   │ │  Retention   │ │  Uni Accept  │ │   Savings    │  │
│  │ (vs 65%)     │ │  (vs 5%)     │ │              │ │              │  │
│  └──────────────┘ └──────────────┘ └──────────────┘ └──────────────┘  │
│                         25%             25%             25%             │
│                                                                         │
│  [Disclaimer text - 12px italic centered]                               │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘

Padding: 60px top/bottom
Stat Icon: 32px emoji
Stat Number: 48px, Montserrat ExtraBold, Deep Blue
Stat Label: 16px, Open Sans Regular, Medium Gray
```

### Section 3: What Is EduMeUp

```
WHAT IS EDUMEUP LAYOUT
═══════════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────────────────────────┐
│  Background: White                                                      │
│  [Padding: 80px]                                                        │
│                                                                         │
│                    What Is EduMeUp?                                     │
│         (H2 - 42px, centered, max-width 800px subheading)              │
│                                                                         │
│  ┌─────────────────────────────────┐ ┌───────────────────────────┐     │
│  │                                 │ │                           │     │
│  │  Text content (18px body)       │ │   [Dashboard Mockup]      │     │
│  │                                 │ │                           │     │
│  │  Paragraph 1...                 │ │   500px × 400px           │     │
│  │                                 │ │                           │     │
│  │  Paragraph 2...                 │ │   Student interface       │     │
│  │                                 │ │   showing mastery %,      │     │
│  │  Paragraph 3...                 │ │   subjects, progress      │     │
│  │                                 │ │                           │     │
│  │  [Read More ▼]                  │ │   Border radius: 12px     │     │
│  │                                 │ │   Subtle shadow           │     │
│  │  --- EXPANDABLE CONTENT ---     │ │                           │     │
│  │                                 │ │                           │     │
│  │         55% Width               │ │       45% Width           │     │
│  └─────────────────────────────────┘ └───────────────────────────┘     │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

### Section 4: What We Offer (Programs)

```
PROGRAMS GRID LAYOUT
═══════════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────────────────────────┐
│  Background: Gradient White → #F0F9FF                                   │
│                                                                         │
│        What We Offer: Complete Pre-K to O-Level Curriculum              │
│                                                                         │
│  ┌──────────────────┐ ┌──────────────────┐ ┌──────────────────┐        │
│  │   🎨             │ │   📚             │ │   🔬             │        │
│  │  Starter Primary │ │  Lower Primary   │ │  Upper Primary   │        │
│  │  Ages 4-7        │ │  Ages 8-10       │ │  Age 11          │        │
│  │  Pre-K to Gr 2   │ │  Grades 3-5      │ │  Grade 6         │        │
│  │                  │ │                  │ │                  │        │
│  │  Description...  │ │  Description...  │ │  Description...  │        │
│  │                  │ │                  │ │                  │        │
│  │  ✓ Feature 1     │ │  ✓ Feature 1     │ │  ✓ Feature 1     │        │
│  │  ✓ Feature 2     │ │  ✓ Feature 2     │ │  ✓ Feature 2     │        │
│  │                  │ │                  │ │                  │        │
│  │  Explore →       │ │  Explore →       │ │  Explore →       │        │
│  └──────────────────┘ └──────────────────┘ └──────────────────┘        │
│                                                                         │
│  ┌──────────────────┐ ┌──────────────────┐ ┌──────────────────┐        │
│  │  ⭐ UNIQUE       │ │                  │ │                  │        │
│  │   🎯             │ │   🎓             │ │   🏛️             │        │
│  │  Get Ready       │ │  O-Level/IGCSE   │ │  FSc/Intermed.   │        │
│  │  Ages 12-14      │ │  Ages 14-16      │ │  Ages 17-18      │        │
│  │  Grades 7-8      │ │  Grades 9-10     │ │  Grades 11-12    │        │
│  │                  │ │                  │ │                  │        │
│  │  GOLD Border     │ │                  │ │                  │        │
│  └──────────────────┘ └──────────────────┘ └──────────────────┘        │
│                                                                         │
│                    [START FREE DIAGNOSTIC →]                            │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘

Grid: 3 columns × 2 rows
Gap: 24px
Card Min Height: 320px
Get Ready Card: Special gold (#F59E0B) border + badge
```

### Section 5: Services (Tabbed)

```
TABBED SERVICES LAYOUT
═══════════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────────────────────────┐
│  Background: White                                                      │
│                                                                         │
│           Services & Resources: Everything You Need                      │
│                                                                         │
│  ┌─────────┬─────────┬─────────┬─────────┬──────────────┐              │
│  │Students │ Parents │Teachers │ Schools │ Homeschool   │ ← Tab Bar    │
│  │ ACTIVE  │         │         │         │              │              │
│  └─────────┴─────────┴─────────┴─────────┴──────────────┘              │
│  ┌─────────────────────────────────────────────────────────────────┐   │
│  │                                                                 │   │
│  │  ┌─────────┐ ┌─────────┐ ┌─────────┐                           │   │
│  │  │  🔍     │ │  🛠️     │ │  🎬     │                           │   │
│  │  │ AI      │ │ Remedial│ │ Dual-   │                           │   │
│  │  │ Diagnos.│ │ Program │ │ Coding  │                           │   │
│  │  │         │ │         │ │         │                           │   │
│  │  │ [+More] │ │ [+More] │ │ [+More] │                           │   │
│  │  └─────────┘ └─────────┘ └─────────┘                           │   │
│  │                                                                 │   │
│  │  ┌─────────┐ ┌─────────┐ ┌─────────┐                           │   │
│  │  │  📝     │ │  📅     │ │  📊     │                           │   │
│  │  │ Past    │ │ Spaced  │ │ Progress│                           │   │
│  │  │ Papers  │ │ Review  │ │ Dashbrd │                           │   │
│  │  └─────────┘ └─────────┘ └─────────┘                           │   │
│  │                                                                 │   │
│  │  ┌─────────┐ ┌─────────┐ ┌─────────┐                           │   │
│  │  │  🤖     │ │  👨‍🏫     │ │  📱     │                           │   │
│  │  │ AI      │ │ Human   │ │ Mobile  │                           │   │
│  │  │ Chatbot │ │ Tutors  │ │ App     │                           │   │
│  │  └─────────┘ └─────────┘ └─────────┘                           │   │
│  │                                                                 │   │
│  │  Grid: 3 columns × 3 rows = 9 service cards per tab            │   │
│  │                                                                 │   │
│  └─────────────────────────────────────────────────────────────────┘   │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

### Section 6: Comparison Table

```
COMPARISON SECTION LAYOUT
═══════════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────────────────────────┐
│  Background: Gradient #EFF6FF → #DBEAFE                                 │
│                                                                         │
│            Why EduMeUp Succeeds Where Others Fail                       │
│                                                                         │
│  ┌─────────────────────────────────────────────────────────────────┐   │
│  │ Feature      │ EduMeUp  │ Khan     │ Kognity  │ ChatGPT│ Tutor  │   │
│  │              │ (GREEN)  │ Academy  │ GCSEPod  │        │        │   │
│  ├──────────────┼──────────┼──────────┼──────────┼────────┼────────┤   │
│  │ AI Diagnostic│ ✅ Sub-  │ ⚠️ Basic │ ❌ None  │ ❌     │ ⚠️     │   │
│  │              │ skill    │          │          │        │ Manual │   │
│  ├──────────────┼──────────┼──────────┼──────────┼────────┼────────┤   │
│  │ Personalized │ ✅ 80%   │ ⚠️ Self  │ ❌ Linear│ ❌     │ ⚠️     │   │
│  │ Paths        │ mastery  │ directed │          │        │        │   │
│  ├──────────────┼──────────┼──────────┼──────────┼────────┼────────┤   │
│  │ ... more rows spanning full comparison ...                      │   │
│  ├──────────────┼──────────┼──────────┼──────────┼────────┼────────┤   │
│  │ Pass Rate    │ 91%      │ ~70-75%  │ Unknown  │ N/A    │ ~65%   │   │
│  └──────────────┴──────────┴──────────┴──────────┴────────┴────────┘   │
│                                                                         │
│  ┌──────────────────┐ ┌──────────────────┐ ┌──────────────────┐        │
│  │ 💎 $3-5M Moat    │ │ 🎯 Get Ready     │ │ 🔬 Research      │        │
│  │ Multi-Purpose    │ │ World's Only     │ │ Independent      │        │
│  │ Content          │ │ O-Level Bridge   │ │ Proof            │        │
│  └──────────────────┘ └──────────────────┘ └──────────────────┘        │
│                                                                         │
│  Key Differentiator Boxes: Gold, Green, Deep Blue borders              │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

### Section 7: Research Validation

```
RESEARCH SECTION LAYOUT
═══════════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────────────────────────┐
│  Background: White                                                      │
│                                                                         │
│        Research Validation: Independent University Study                 │
│                                                                         │
│  ┌─────────────────────────────────────────────────────────────────┐   │
│  │ 🏆 INDEPENDENT UNIVERSITY STUDY | PEER-REVIEWED | 2024          │   │
│  │                                                                 │   │
│  │  University of Education Lahore Randomized Controlled Trial     │   │
│  │                                                                 │   │
│  │  ┌─────────────────────┐ ┌─────────────────────────────────┐   │   │
│  │  │ STUDY INFO          │ │ KEY RESULTS                     │   │   │
│  │  │                     │ │                                 │   │   │
│  │  │ Institution: UE     │ │ Pass Rate: 91% vs 65%          │   │   │
│  │  │ Sample: n=611       │ │ High Grades: 47% vs 18%        │   │   │
│  │  │ Duration: 18 months │ │ Retention: 94% vs 67%          │   │   │
│  │  │ Design: RCT         │ │ Effect Size: d=0.72 (LARGE)    │   │   │
│  │  │                     │ │                                 │   │   │
│  │  │ [+ Full Method]     │ │ p<0.001 (99.9% confidence)     │   │   │
│  │  └─────────────────────┘ └─────────────────────────────────┘   │   │
│  │                                                                 │   │
│  │  ┌─────────────────────────────────────────────────────────┐   │   │
│  │  │ ⚠️ What "p<0.001" Means: [Yellow explainer box]          │   │   │
│  │  └─────────────────────────────────────────────────────────┘   │   │
│  │                                                                 │   │
│  │  ┌─────────────────────────────────────────────────────────┐   │   │
│  │  │ "EduMeUp's systematic methodology produces outcomes..." │   │   │
│  │  │ — Dr. Faheem Ahmed, Lead Researcher                     │   │   │
│  │  └─────────────────────────────────────────────────────────┘   │   │
│  │                                                                 │   │
│  │              [📄 DOWNLOAD FULL STUDY (PDF) →]                   │   │
│  │                                                                 │   │
│  └─────────────────────────────────────────────────────────────────┘   │
│                                                                         │
│        Our Methods Validated by 15+ Peer-Reviewed Studies               │
│                                                                         │
│  ┌──────────┐ ┌──────────┐ ┌──────────┐                                │
│  │ Spaced   │ │ Dual-    │ │ Active   │                                │
│  │ Repetit. │ │ Coding   │ │ Learning │                                │
│  └──────────┘ └──────────┘ └──────────┘                                │
│  ┌──────────┐ ┌──────────┐ ┌──────────┐                                │
│  │ Mastery  │ │ Retrieval│ │Formative │                                │
│  │ Learning │ │ Practice │ │ Assess.  │                                │
│  └──────────┘ └──────────┘ └──────────┘                                │
│                                                                         │
│  Research Citations Grid: 3 columns × 2 rows                            │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘

Main Study Box:
├── Background: #EFF6FF
├── Border: 3px solid #1E40AF
├── Border Radius: 12px
├── Padding: 40px
└── Box Shadow: 0px 6px 20px rgba(30,64,175,0.2)
```

### Section 8: Testimonials

```
TESTIMONIALS LAYOUT
═══════════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────────────────────────┐
│  Background: Gradient White → #F0F9FF                                   │
│                                                                         │
│            Real Students, Real Results: Success Stories                  │
│                                                                         │
│  ┌──────────────────┐ ┌──────────────────┐ ┌──────────────────┐        │
│  │                  │ │                  │ │                  │        │
│  │     [Photo]      │ │     [Photo]      │ │     [Photo]      │        │
│  │     (Circle)     │ │     (Circle)     │ │     (Circle)     │        │
│  │                  │ │                  │ │                  │        │
│  │  Ahmed Hassan    │ │  Mrs. Nadia      │ │  Hassan Family   │        │
│  │  Student         │ │  Parent          │ │  Homeschool      │        │
│  │                  │ │                  │ │                  │        │
│  │  ⭐ 5 A* Grades  │ │  👨‍👩‍👧‍👦 2 Students │ │  🏡 Success      │        │
│  │                  │ │                  │ │                  │        │
│  │  ┌────────────┐  │ │  ┌────────────┐  │ │  ┌────────────┐  │        │
│  │  │ 45% → 82%  │  │ │  │ Visibility │  │ │  │ 5 A*, LUMS │  │        │
│  │  │ LUMS Schol.│  │ │  │ Peace Mind │  │ │  │ $140K Saved│  │        │
│  │  └────────────┘  │ │  └────────────┘  │ │  └────────────┘  │        │
│  │                  │ │                  │ │                  │        │
│  │  "Quote..."      │ │  "Quote..."      │ │  "Quote..."      │        │
│  │                  │ │                  │ │                  │        │
│  │  — Attribution   │ │  — Attribution   │ │  — Attribution   │        │
│  │                  │ │                  │ │                  │        │
│  └──────────────────┘ └──────────────────┘ └──────────────────┘        │
│                                                                         │
│                     [Read 50+ More Success Stories →]                   │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘

Carousel: Horizontal scroll on mobile
Cards: 32% width each on desktop
```

### Section 9: Stakeholder Quick Access

```
STAKEHOLDER CARDS LAYOUT
═══════════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────────────────────────┐
│  Background: Deep Blue (#1E40AF)                                        │
│                                                                         │
│               Who Are You? Find Your Perfect Path                        │
│               (White text on dark)                                       │
│                                                                         │
│  ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐ ┌──────────┐      │
│  │   🎓     │ │   👨‍👩‍👧    │ │   🏡     │ │   🏫     │ │   👨‍🏫    │      │
│  │          │ │          │ │          │ │          │ │          │      │
│  │ Students │ │ Parents  │ │ Homeschl │ │ Schools  │ │ Teachers │      │
│  │          │ │          │ │          │ │          │ │          │      │
│  │ Master.. │ │ Stop...  │ │ 92%...   │ │ Boost... │ │ Ready... │      │
│  │          │ │          │ │          │ │          │ │          │      │
│  │ [Start→] │ │ [Get →]  │ │ [Explr→] │ │ [Demo→]  │ │ [Explr→] │      │
│  │          │ │          │ │          │ │          │ │          │      │
│  │   20%    │ │   20%    │ │   20%    │ │   20%    │ │   20%    │      │
│  └──────────┘ └──────────┘ └──────────┘ └──────────┘ └──────────┘      │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘

Card Styling:
├── Background: rgba(255,255,255,0.1)
├── Border: 2px solid rgba(255,255,255,0.3)
├── Border Radius: 12px
├── Padding: 24px
├── Text: White
└── Hover: Background brighter, lift effect

Button:
├── Background: White
├── Text: Deep Blue (#1E40AF)
├── Full width within card
└── Border Radius: 6px
```

### Section 10: Pricing

```
PRICING SECTION LAYOUT
═══════════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────────────────────────┐
│  Background: White                                                      │
│                                                                         │
│              Transparent Pricing: Exceptional Value                      │
│                                                                         │
│  ┌──────────────────┐ ┌──────────────────┐ ┌──────────────────┐        │
│  │ 🎯 MOST AFFORD.  │ │ ⭐ MOST POPULAR  │ │ 🎯 AS-NEEDED     │        │
│  │                  │ │                  │ │                  │        │
│  │   Self-Learning  │ │  Teacher-Guided  │ │  Add-On Tutoring │        │
│  │                  │ │ ┌──────────────┐ │ │                  │        │
│  │    $150-1,500    │ │ │  $400-4,000  │ │ │    $15-35/hr     │        │
│  │                  │ │ │   (GOLD)     │ │ │                  │        │
│  │   per student/yr │ │ └──────────────┘ │ │   per session    │        │
│  │                  │ │  ELEVATED CARD   │ │                  │        │
│  │  ✓ Feature 1     │ │  Gold border 3px │ │  ✓ Feature 1     │        │
│  │  ✓ Feature 2     │ │  translateY(-8px)│ │  ✓ Feature 2     │        │
│  │  ✓ Feature 3     │ │                  │ │  ✓ Feature 3     │        │
│  │  ...             │ │  ✓ Everything +  │ │  ...             │        │
│  │                  │ │  ✓ Teacher       │ │                  │        │
│  │  Best For:       │ │  ✓ Weekly Live   │ │  Best For:       │        │
│  │  Independent     │ │                  │ │  Occasional      │        │
│  │                  │ │  Best For:       │ │  support         │        │
│  │ [START FREE →]   │ │  Structured      │ │                  │        │
│  │     BLUE         │ │                  │ │ [BROWSE TUTORS]  │        │
│  │                  │ │ [CONSULTATION →] │ │    PURPLE        │        │
│  │                  │ │     GOLD         │ │                  │        │
│  └──────────────────┘ └──────────────────┘ └──────────────────┘        │
│                                                                         │
│  ┌─────────────────────────────────────────────────────────────────┐   │
│  │  SAVINGS COMPARISON BOX                                         │   │
│  │  Background: #ECFDF5  |  Border: 2px solid #10B981              │   │
│  │                                                                 │   │
│  │  Traditional: $345K-1.017M  |  EduMeUp: $7.5K-135K              │   │
│  │                                                                 │   │
│  │         💰 SAVE $210,000-882,000 (85-95% Reduction)             │   │
│  │         (36px, ExtraBold, Dark Green)                           │   │
│  │                                                                 │   │
│  └─────────────────────────────────────────────────────────────────┘   │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘

Middle Card (Most Popular):
├── Border: 3px solid Gold (#F59E0B)
├── Transform: translateY(-8px)
├── Box Shadow: Stronger
└── Badge: Gold background, white text
```

### Section 11: Guarantees

```
GUARANTEES SECTION LAYOUT
═══════════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────────────────────────┐
│  Background: Dark Navy (#1A2B3C)                                        │
│  Text: White                                                            │
│                                                                         │
│              Risk-Free: Our Unprecedented Guarantees                     │
│                                                                         │
│  ┌───────────────────────────┐   ┌───────────────────────────┐         │
│  │                           │   │                           │         │
│  │  ✅ (48px Green)          │   │  🎯 (48px Gold)           │         │
│  │                           │   │                           │         │
│  │  30-Day Money-Back        │   │  Get Ready Success        │         │
│  │  Guarantee                │   │  Guarantee                │         │
│  │                           │   │                           │         │
│  │  Try risk-free...         │   │  Complete courses...      │         │
│  │                           │   │                           │         │
│  │  Refund rate: <3%         │   │  89% score 80%+           │         │
│  │                           │   │                           │         │
│  │  Border: 3px Green        │   │  Border: 3px Gold         │         │
│  │  Background: White        │   │  Background: White        │         │
│  │  48% width each           │   │  48% width each           │         │
│  │                           │   │                           │         │
│  └───────────────────────────┘   └───────────────────────────┘         │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

### Section 12: FAQ

```
FAQ SECTION LAYOUT
═══════════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────────────────────────┐
│  Background: White                                                      │
│  Max Width: 900px centered                                              │
│                                                                         │
│                    Frequently Asked Questions                            │
│                                                                         │
│  ┌─────────────────────────────────────────────────────────────────┐   │
│  │  Q: What makes EduMeUp different from Khan Academy?          ▼  │   │
│  └─────────────────────────────────────────────────────────────────┘   │
│                                                                         │
│  ┌─────────────────────────────────────────────────────────────────┐   │
│  │  Q: How much does EduMeUp cost? Is it worth it?              ▲  │   │
│  ├─────────────────────────────────────────────────────────────────┤   │
│  │                                                                 │   │
│  │  A: Self-Learning: $150-1,500 annually per student...          │   │
│  │  [Read detailed pricing →]                                      │   │
│  │                                                                 │   │
│  └─────────────────────────────────────────────────────────────────┘   │
│                                                                         │
│  ┌─────────────────────────────────────────────────────────────────┐   │
│  │  Q: Will universities accept homeschoolers using EduMeUp?    ▼  │   │
│  └─────────────────────────────────────────────────────────────────┘   │
│                                                                         │
│  ... 10 total FAQ items ...                                             │
│                                                                         │
│               Still have questions? We're here to help.                 │
│                   [SCHEDULE FREE CONSULTATION →]                        │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

### Section 13: Final CTA

```
FINAL CTA SECTION LAYOUT
═══════════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────────────────────────┐
│  Background: Gradient Deep Blue (#1E40AF → #1E3A8A)                     │
│  Text: White                                                            │
│                                                                         │
│          Ready to Transform Your Learning Journey?                       │
│          (48px, ExtraBold, White, centered)                             │
│                                                                         │
│          Join 2,000+ students across 25+ countries...                   │
│          (22px, Regular, White 95%, max-width 800px)                    │
│                                                                         │
│                ┌───────────────────────────────────┐                    │
│                │                                   │                    │
│                │   START FREE DIAGNOSTIC NOW →     │                    │
│                │                                   │                    │
│                │   420px × 72px                    │                    │
│                │   Background: White               │                    │
│                │   Text: Deep Blue, 22px Bold      │                    │
│                │   Strong shadow                   │                    │
│                │                                   │                    │
│                └───────────────────────────────────┘                    │
│                                                                         │
│             No credit card required | 2-3 hours | Instant roadmap       │
│                                                                         │
│  ┌──────────────────┐ ┌──────────────────┐ ┌──────────────────┐        │
│  │ 📅 Schedule      │ │ 📊 Download      │ │ 💬 Contact       │        │
│  │ Consultation     │ │ Research Study   │ │ Our Team         │        │
│  │                  │ │                  │ │                  │        │
│  │ Semi-transparent │ │ Semi-transparent │ │ Semi-transparent │        │
│  │ white cards      │ │ white cards      │ │ white cards      │        │
│  └──────────────────┘ └──────────────────┘ └──────────────────┘        │
│                                                                         │
│  ┌─────────────────────────────────────────────────────────────────┐   │
│  │  Trust indicators bar (semi-transparent)                        │   │
│  │  ✓ 2,000+ Students  ✓ 91% Pass Rate  ✓ 15+ Studies  ✓ 24/7     │   │
│  └─────────────────────────────────────────────────────────────────┘   │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘
```

### Section 14: Footer

```
FOOTER LAYOUT
═══════════════════════════════════════════════════════════════

┌─────────────────────────────────────────────────────────────────────────┐
│  Background: Dark Navy (#1A2B3C)                                        │
│  Text: White with varying opacity                                       │
│                                                                         │
│  ┌──────────────┐ ┌──────────────┐ ┌──────────────┐ ┌──────────────┐  │
│  │              │ │              │ │              │ │              │  │
│  │  EDUMEUP     │ │ FOR LEARNERS │ │  RESOURCES   │ │ LEGAL/CONTACT│  │
│  │              │ │              │ │              │ │              │  │
│  │  Logo        │ │ • Students   │ │ • Features   │ │ • Privacy    │  │
│  │              │ │ • Parents    │ │ • Get Ready  │ │ • Terms      │  │
│  │  Description │ │ • Homeschool │ │ • Tutoring   │ │ • Refund     │  │
│  │  text about  │ │ • Teachers   │ │ • Research   │ │ • Guarantee  │  │
│  │  EduMeUp     │ │ • Schools    │ │ • Stories    │ │              │  │
│  │              │ │              │ │ • Blog       │ │ Email:       │  │
│  │  [Social     │ │ • Diagnostic │ │ • FAQ        │ │ admin@...    │  │
│  │   Icons]     │ │ • Courses    │ │ • Support    │ │              │  │
│  │              │ │ • Pricing    │ │ • Contact    │ │ Hours:       │  │
│  │              │ │              │ │              │ │ 24/7 AI      │  │
│  │    25%       │ │    25%       │ │    25%       │ │    25%       │  │
│  └──────────────┘ └──────────────┘ └──────────────┘ └──────────────┘  │
│                                                                         │
│  ┌─────────────────────────────────────────────────────────────────┐   │
│  │  Background: Darker Navy (#0F172A)                              │   │
│  │                                                                 │   │
│  │  © 2026 EduMeUp by Softsincs     Powered by Moodle | Edwiser   │   │
│  │                                                                 │   │
│  └─────────────────────────────────────────────────────────────────┘   │
│                                                                         │
└─────────────────────────────────────────────────────────────────────────┘

Footer Links:
├── Font: 15px, Open Sans Regular
├── Color: White (opacity 0.75)
├── Line Height: 2.2
├── Hover: Opacity 1.0, underline
└── Social Icons: 32px, opacity 0.7, hover 1.0
```

---

## 🖼️ IMAGE REQUIREMENTS & PROMPTS

### Hero Image

```
NOOBANANA PROMPT: HERO IMAGE
═══════════════════════════════════════════════════════════════

Create a modern, professional educational illustration showing diverse 
students achieving success through technology-enhanced learning:

MAIN ELEMENTS:
─────────────────────────────────────────────────────────────
• Central figure: Confident teenage student (age 14-16, South Asian, 
  wearing modern casual clothing) holding tablet displaying upward-
  trending graph showing "45% → 91%" improvement
• Background: Abstract neural network pattern (light blue/teal lines 
  connecting nodes) representing AI-powered learning
• Floating elements around student:
  - Interactive H5P quiz bubble (colorful, engaging)
  - Diagnostic report icon showing "Mastery: 85%"
  - Past paper document with checkmarks
  - Video lesson play button
  - Brain icon with lightbulb (representing conceptual understanding)

COLOR PALETTE:
─────────────────────────────────────────────────────────────
• Primary: Deep Blue (#1E40AF), Teal (#0891B2)
• Accents: Green (#10B981) for success, Orange (#F97316) for highlights
• Background: Clean white with subtle gradient to light blue

STYLE:
─────────────────────────────────────────────────────────────
• Modern, professional illustration (not cartoon, not photo-realistic)
• Aspirational and optimistic mood
• Clean lines, organized composition
• Technology-forward but warm and approachable
• International/global aesthetic (diverse, culturally neutral)

COMPOSITION:
─────────────────────────────────────────────────────────────
• Student positioned slightly left of center
• Tablet/device prominent and clearly visible
• Floating elements balanced around student
• Sense of upward movement and progress

SPECIFICATIONS:
─────────────────────────────────────────────────────────────
• Dimensions: 1200 × 1000px (export at 700 × 600px for web)
• Format: PNG or WebP
• File Size: Under 300KB
• Alt Text: "Student achieving 91% pass rate through EduMeUp 
  research-backed learning system"
```

### Dashboard Mockup

```
NOOBANANA PROMPT: DASHBOARD MOCKUP
═══════════════════════════════════════════════════════════════

Create a clean, modern dashboard interface mockup showing the EduMeUp 
student learning platform:

MAIN SCREEN ELEMENTS:
─────────────────────────────────────────────────────────────
• Header: EduMeUp logo, student name "Ahmed K.", notification bell
• Left Sidebar: Subject icons (Math, Physics, Chemistry, Biology, 
  English) with progress bars showing percentage completion
• Center Panel: Current lesson "Quadratic Equations"
  - Video player showing teacher explanation (paused frame)
  - Interactive H5P drag-and-drop activity visible below video
  - Progress indicator: "Step 3 of 8: Practice Problems"
• Right Sidebar:
  - "Your Mastery: 78%" circular progress indicator (green/orange)
  - "Next Review: 2 days" with calendar icon
  - "Need Help?" AI chatbot button

VISUAL STYLE:
─────────────────────────────────────────────────────────────
• Clean, modern interface design (Netflix/Spotify aesthetic)
• Color scheme: Deep Blue (#1E40AF) primary, Green (#10B981) for 
  progress, White background
• Professional UI/UX quality
• Clearly readable text and labels
• Organized, uncluttered layout

SPECIFICATIONS:
─────────────────────────────────────────────────────────────
• Dimensions: 900 × 700px (display at 500 × 400px)
• Perspective: Slight 3D perspective view showing depth
• Format: PNG
• Border: 1px solid light gray (#E5E7EB)
• Border Radius: 12px
• Box Shadow: 0px 4px 20px rgba(0,0,0,0.1)
• Alt Text: "EduMeUp student dashboard showing personalized 
  learning interface"
```

### Testimonial Photos

```
NOOBANANA PROMPTS: TESTIMONIAL PHOTOS
═══════════════════════════════════════════════════════════════

STUDENT PHOTO (Ahmed Hassan):
─────────────────────────────────────────────────────────────
Create professional student portrait: South Asian male teenager 
(age 17-18), confident smile, wearing formal attire (dress shirt), 
holding university acceptance letter visible with "LUMS" logo, 
modern school/office background with bookshelves, warm natural 
lighting, aspirational mood. 
Style: Professional portrait photography, realistic. 
Format: 400×400px, circular crop.


PARENT PHOTO (Mrs. Nadia Ahmed):
─────────────────────────────────────────────────────────────
Professional portrait: South Asian mother (age 38-45), warm 
confident smile, wearing business casual / traditional attire, 
modern home office setting, relieved and proud expression, 
books and educational materials visible background. 
Style: Professional portrait, realistic, warm lighting. 
Format: 400×400px, circular crop.


HOMESCHOOL FAMILY PHOTO (Hassan Family):
─────────────────────────────────────────────────────────────
Professional family portrait: South Asian homeschool family 
(mother, father, two children ages 14-17), grouped naturally 
around table with laptop showing educational dashboard, bright 
modern home setting, pride and achievement mood, natural lighting. 
Style: Professional family photography, realistic, warm.
Format: 600×400px, landscape (crop to featured section).
```

### Icon System

```
ICON SPECIFICATIONS
═══════════════════════════════════════════════════════════════

For initial implementation, use emoji icons:
├── 🎓 Students/Graduation
├── 👨‍👩‍👧 Parents/Family
├── 🏡 Homeschool
├── 🏫 Schools
├── 👨‍🏫 Teachers
├── 🎯 Target/Goals/Get Ready
├── 🧠 Brain/Learning
├── 📚 Books/Courses
├── 🔬 Research/Science
├── 📊 Dashboard/Analytics
├── 💰 Money/Savings
├── ✅ Success/Check
├── ⭐ Premium/Featured
├── 🏆 Achievement
├── 🔍 Search/Diagnostic
├── 🛠️ Tools/Remediation
├── 🎬 Video/Media
├── 📝 Papers/Documents
├── 📅 Calendar/Schedule
├── 🤖 AI/Chatbot
├── 📱 Mobile

For production, create custom SVG icon set:
├── Size: 24px, 32px, 48px, 64px variants
├── Style: Outline style, 2px stroke
├── Colors: Inherit from parent (currentColor)
└── Format: SVG sprite or individual files
```

---

## 📱 RESPONSIVE DESIGN GUIDELINES

### Breakpoints

```
BREAKPOINT SYSTEM
═══════════════════════════════════════════════════════════════

$breakpoint-xs:    320px   // Small phones
$breakpoint-sm:    480px   // Large phones
$breakpoint-md:    768px   // Tablets
$breakpoint-lg:    1024px  // Small laptops
$breakpoint-xl:    1200px  // Desktop
$breakpoint-xxl:   1400px  // Large desktop

MEDIA QUERIES:
─────────────────────────────────────────────────────────────
Mobile First Approach:

/* Base styles (mobile) */
.element { ... }

/* Tablet and up */
@media (min-width: 768px) { ... }

/* Desktop and up */
@media (min-width: 1024px) { ... }

/* Large desktop */
@media (min-width: 1200px) { ... }
```

### Layout Changes by Breakpoint

| Element | Mobile (<768px) | Tablet (768-1023px) | Desktop (1024px+) |
|---------|-----------------|---------------------|-------------------|
| **Hero** | Stack vertical (100%) | 50/50 columns | 55/45 columns |
| **Stats Bar** | 2×2 grid | 4 columns | 4 columns |
| **Program Cards** | 1 column | 2 columns | 3 columns |
| **Service Grid** | 1 column | 2 columns | 3 columns |
| **Testimonials** | Carousel | 2 visible | 3 visible |
| **Stakeholder Cards** | 2×3 grid | 3+2 layout | 5 columns |
| **Pricing Cards** | Stack | Stack (center elevated) | 3 columns |
| **Guarantee Boxes** | Stack | 2 columns | 2 columns |
| **Footer** | Stack | 2×2 grid | 4 columns |

### Typography Scale by Breakpoint

| Element | Mobile | Tablet | Desktop |
|---------|--------|--------|---------|
| **H1 (Hero)** | 36px | 44px | 56px |
| **H2 (Section)** | 28px | 34px | 42px |
| **H3 (Subsection)** | 22px | 24px | 28px |
| **Large Body** | 16px | 17px | 18-20px |
| **Regular Body** | 15px | 16px | 16-17px |
| **Stat Number** | 36px | 42px | 48px |

### Touch Targets

```
MOBILE TOUCH SPECIFICATIONS
═══════════════════════════════════════════════════════════════

Minimum Touch Target: 44px × 44px (Apple HIG / WCAG 2.1)

Buttons (Mobile):
├── Height: Minimum 48px
├── Padding: 16px horizontal minimum
└── Full-width preferred for primary CTAs

Links (Mobile):
├── Line Height: 2.0+ for tap targets
├── Padding: 8px vertical
└── Underline for clarity

Cards (Mobile):
├── Full tap area clickable
├── Visual feedback on press (opacity 0.9)
└── Clear active states
```

---

## ✨ ANIMATION & INTERACTION STATES

### Hover Effects

```
HOVER SPECIFICATIONS
═══════════════════════════════════════════════════════════════

BUTTONS:
─────────────────────────────────────────────────────────────
Primary CTA:
├── Background: Darken 15%
├── Transform: translateY(-2px)
├── Box Shadow: Increase blur and spread
└── Transition: all 0.2s ease-out

Text Link:
├── Text Decoration: underline
├── Color: Unchanged or slightly darker
└── Transition: all 0.15s ease


CARDS:
─────────────────────────────────────────────────────────────
Standard Card:
├── Transform: translateY(-4px)
├── Box Shadow: 0px 8px 24px rgba(0,0,0,0.12)
├── Border Color: Slightly darker
└── Transition: all 0.25s ease-out

Testimonial Card:
├── Same as standard
└── Photo: Slight scale (1.02)


TABLE ROWS:
─────────────────────────────────────────────────────────────
├── Background: #F9FAFB (subtle highlight)
└── Transition: background 0.15s ease


TAB BUTTONS:
─────────────────────────────────────────────────────────────
Inactive Tab:
├── Background: Darken slightly (#E5E7EB)
├── Text: Darken (#1A2B3C)
└── Transition: all 0.15s ease
```

### Transitions

```
TRANSITION TOKENS
═══════════════════════════════════════════════════════════════

--transition-fast:      0.15s ease
--transition-normal:    0.2s ease-out
--transition-slow:      0.3s ease-out
--transition-expand:    0.35s cubic-bezier(0.4, 0, 0.2, 1)

USAGE:
─────────────────────────────────────────────────────────────
Fast (0.15s):     Text color, opacity, background (subtle)
Normal (0.2s):    Buttons, links, form elements
Slow (0.3s):      Cards, panels, complex elements
Expand (0.35s):   Accordion expand/collapse, modal open
```

### Focus States

```
FOCUS SPECIFICATIONS (Accessibility)
═══════════════════════════════════════════════════════════════

Standard Focus Ring:
├── Outline: 3px solid #60A5FA (Light Blue)
├── Outline Offset: 2px
└── Border Radius: Match element border-radius

For dark backgrounds:
├── Outline: 3px solid #FCD34D (Yellow)
└── High contrast visibility

Focus-Visible (Keyboard Only):
.element:focus-visible {
  outline: 3px solid #60A5FA;
  outline-offset: 2px;
}

.element:focus:not(:focus-visible) {
  outline: none;
}
```

### Loading States

```
LOADING INDICATORS
═══════════════════════════════════════════════════════════════

Button Loading:
├── Text: Replace with "Loading..."
├── Icon: Spinning loader (16px)
├── Pointer Events: None
└── Opacity: 0.7

Content Loading:
├── Skeleton screens preferred
├── Pulse animation: opacity 0.5 → 1 → 0.5
├── Background: #E5E7EB (gray)
└── Animation: 1.5s infinite
```

---

## ♿ ACCESSIBILITY REQUIREMENTS

### Color Contrast

```
WCAG 2.1 AA COMPLIANCE
═══════════════════════════════════════════════════════════════

MINIMUM CONTRAST RATIOS:
─────────────────────────────────────────────────────────────
Normal Text (< 24px):     4.5:1 minimum
Large Text (≥ 24px):      3:1 minimum
UI Components:            3:1 minimum

VERIFIED COMBINATIONS:
─────────────────────────────────────────────────────────────
✅ Dark Navy (#1A2B3C) on White (#FFFFFF)     — 14.5:1
✅ Deep Blue (#1E40AF) on White               — 7.8:1
✅ Dark Gray (#4A5568) on White               — 7.5:1
✅ Medium Gray (#718096) on White             — 4.6:1
✅ White on Deep Blue (#1E40AF)               — 7.8:1
✅ White on Dark Navy (#1A2B3C)               — 14.5:1

⚠️ CHECK BEFORE USE:
─────────────────────────────────────────────────────────────
• Gold (#F59E0B) on White                     — Test with tool
• Light text on colored backgrounds           — Verify each
```

### Screen Reader Support

```
ARIA REQUIREMENTS
═══════════════════════════════════════════════════════════════

LANDMARKS:
─────────────────────────────────────────────────────────────
<header role="banner">
<nav role="navigation" aria-label="Main">
<main role="main">
<section aria-labelledby="section-heading-id">
<footer role="contentinfo">

INTERACTIVE ELEMENTS:
─────────────────────────────────────────────────────────────
Buttons:
└── <button type="button">Text</button> (not <div onclick>)

Links:
└── <a href="..." aria-label="Descriptive text">

Tabs:
├── role="tablist" on container
├── role="tab" on each tab button
├── aria-selected="true/false"
├── role="tabpanel" on content
└── aria-labelledby linking tab to panel

Accordions:
├── <button aria-expanded="true/false">
├── aria-controls="content-id"
└── Hidden content: aria-hidden="true" when collapsed

Images:
├── Meaningful: alt="Descriptive text"
├── Decorative: alt="" (empty)
└── Complex: aria-describedby="longer-description-id"
```

### Keyboard Navigation

```
KEYBOARD SUPPORT
═══════════════════════════════════════════════════════════════

Tab Order:
├── Logical top-to-bottom, left-to-right flow
├── Skip links at top: "Skip to main content"
├── Focus trapped in modals when open
└── tabindex="0" only when semantically necessary

Interactive Elements:
├── Enter/Space: Activate buttons, links
├── Arrow Keys: Navigate tabs, dropdowns
├── Escape: Close modals, dropdowns
└── Tab/Shift+Tab: Move between focusable elements
```

---

## 📋 DESIGN CHECKLIST

### Pre-Launch Review

```
DESIGN QA CHECKLIST
═══════════════════════════════════════════════════════════════

TYPOGRAPHY
□ All fonts loading correctly (Montserrat, Open Sans)
□ Font sizes match specifications
□ Line heights consistent
□ No orphan words in headlines
□ Text readable at all breakpoints

COLORS
□ Brand colors accurate (hex values verified)
□ Contrast ratios meet WCAG AA
□ Consistent color usage across sections
□ Hover states visible
□ Focus states visible

SPACING
□ Consistent section padding
□ Consistent component margins
□ Grid alignment verified
□ No overlapping elements
□ Proper breathing room

RESPONSIVE
□ Mobile layout tested (320px - 767px)
□ Tablet layout tested (768px - 1023px)
□ Desktop layout tested (1024px+)
□ Touch targets 44px minimum
□ No horizontal scroll

IMAGES
□ All images optimized (< 300KB each)
□ Alt text provided
□ Images loading correctly
□ Proper aspect ratios maintained
□ Fallbacks for broken images

INTERACTIONS
□ Hover states working
□ Focus states visible
□ Transitions smooth
□ Loading states implemented
□ Error states designed

ACCESSIBILITY
□ Screen reader tested
□ Keyboard navigation working
□ Skip links present
□ ARIA attributes correct
□ Color not only indicator
```

---

**End of Designer Specifications Document**

---

*Document prepared for EduMeUp design team. For questions or clarifications, contact the project lead.*
