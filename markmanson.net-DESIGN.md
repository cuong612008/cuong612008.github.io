# Design System Inspired by Mark Manson

## 1. Visual Theme & Atmosphere

The Mark Manson design system embodies a modern, pragmatic aesthetic rooted in editorial sophistication and direct communication. The visual language prioritizes clarity over ornamentation, combining warm accent tones with a controlled neutral palette to create an approachable yet authoritative presence. The design reflects the brand's core philosophy: straightforward, no-nonsense life advice delivered with intelligence and candor. Typography-driven layouts, generous whitespace, and high-contrast interactive elements ensure every element serves a functional purpose while maintaining visual warmth through strategic use of terracotta orange and soft cream tones.

**Key Characteristics**
- Editorial-forward with strong typographic hierarchy
- Warm, human-centric color palette with purposeful accent usage
- High contrast for accessibility and emphasis
- Minimalist approach with deliberate ornamentation
- Mobile-responsive with touch-friendly interactions
- Serif and sans-serif pairing for personality and readability
- Generous whitespace creating breathing room for content
- Strong emphasis on direct calls-to-action

## 2. Color Palette & Roles

### Primary
- **Charcoal Black** (`#252121`): Dominant text color, button backgrounds, primary UI elements. Used for headlines, body text, and structural components. Conveys authority and directness.
- **Pure White** (`#FFFFFF`): Primary background for content areas, form inputs, card surfaces. Creates clean contrast and legibility.

### Accent Colors
- **Terracotta Orange** (`#F26822`): Primary accent for highlights, testimonial markers, and emphasis. Draws attention to key messages and emotional moments. Warm and inviting.
- **Cream** (`#FCE1D3`): Soft background tint for featured content areas and subtle visual separation. Creates warmth without harshness.

### Interactive
- **Dark Charcoal** (`#252121`): Primary CTA background; creates strong visual hierarchy for action buttons.
- **White Text on Dark** (`#FFFFFF`): High-contrast text for primary buttons ensuring readability.
- **Charcoal Text on Light** (`#252121`): Navigation and secondary interactive elements on light backgrounds.

### Neutral Scale
- **Light Gray** (`#DAE5E6`): Subtle borders, dividers, and background tints for secondary content.
- **Medium Gray** (`#BBBBBB`): Placeholder text, disabled states, secondary labels.
- **Warm Gray** (`#AAAAAA`): Icon fills and muted interactive elements.
- **Almost Black** (`#111111`): Text alternatives for extra emphasis.
- **True Black** (`#000000`): Rare use; maximum contrast scenarios only.
- **Dark Gray-Blue** (`#212223`): Alternative text color for specific component contexts.
- **Off-White** (`#F5F5F5`): Minimal-contrast background for subtle visual distinction.

### Surface & Borders
- **Soft Blue-Gray** (`#DAE5E6`): Primary border and divider color. Creates gentle visual separation without harshness.
- **Light Gray Variant** (`#BBBBBB`): Secondary borders for less prominent dividers.

### Semantic / Status
- **Error Red** (`#EA1414`): Primary error indicator for form validation and alerts.
- **Error Secondary** (`#BD2525`): Error state backgrounds and supporting elements.
- **Error Dark** (`#D1193E`): High-priority error messaging.
- **Warning Gold** (`#E3B200`): Warning states and cautionary messages.

### Supporting Brand Colors
- **Teal** (`#01AFB5`): Optional accent for diversity in large content systems.
- **Deep Navy** (`#21759B`): Archive/legacy content indicator.
- **Rust Brown** (`#A74414`): Warm alternative accent for specific contexts.
- **Burgundy** (`#AF3B43`): Error alternative or premium content marker.
- **Slate** (`#495A5F`): Neutral alternative for structured data.

## 3. Typography Rules

### Font Family
**Primary Font (Headings & UI):** Montserrat
- Fallback stack: `Montserrat, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif`
- Usage: All headings, buttons, navigation, UI labels. Modern, geometric sans-serif with clarity and personality.

**Secondary Font (Body & Editorial):** Source Serif Pro
- Fallback stack: `'Source Serif Pro', Georgia, 'Times New Roman', serif`
- Usage: Body text, links, long-form content, testimonials, editorial voice. Traditional serif provides trustworthiness and editorial credibility.

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing | Notes |
|------|------|------|--------|-------------|----------------|-------|
| Display (H1) | Montserrat | 80px | 700 | 96px | -0.02em | Maximum impact; hero headlines and major page titles. |
| Large Heading (H2) | Montserrat | 56px | 700 | 72.8px | -0.01em | Section headlines and major content breaks. |
| Section Heading (H4) | Montserrat | 24px | 800 | 36px | 0em | Component titles and subsection headers. |
| Heading Secondary (H5) | Montserrat | 14px | 500 | 16px | 0em | Small labels and supplementary headings. |
| Heading Tertiary (H6) | Montserrat | 18px | 700 | 27px | 0em | Card titles and content section headers. |
| Body Text | Source Serif Pro | 18px | 400 | 29.7px | 0em | Primary long-form reading content. |
| Body Secondary | Montserrat | 14px | 400 | 16px | 0em | Supporting text, descriptions, and secondary content. |
| Button Text | Montserrat | 13px | 600 | 14px | 0.02em | Action-oriented text with emphasis. |
| Input Text | Montserrat | 13px | 400 | 19.5px | 0em | Form fields and user-entered content. |
| Caption | Montserrat | 10.4px | 600 | 14px | 0.01em | Small labels, metadata, and annotations. |
| Link Text | Source Serif Pro | 16px | 400 | 26.4px | 0em | Inline links and navigation in editorial context. |

### Principles
- **Contrast Over Decoration:** Typography creates hierarchy through weight and size rather than ornament. Clean, readable structures.
- **Serif for Authority:** Body copy uses serif font to convey editorial credibility and thoughtful messaging.
- **Sans for Action:** UI elements, buttons, and navigation use geometric sans-serif for modern clarity and scannability.
- **Generous Line Heights:** Line heights exceed 1.4× font size for comfortable reading, especially in long-form content.
- **Weight Matters:** Extreme weights (600–800) reserved for headings and CTAs to maintain visual impact without increasing size.
- **Consistent Baselines:** All type aligns to 4px baseline grid for precision and rhythm.

## 4. Component Stylings

### Buttons

#### Primary Button (Filled Dark)
```
Background: #252121
Text Color: #FFFFFF
Font: Montserrat, 13px, 600
Padding: 12px 30px
Height: 40px
Border Radius: 25px
Border: None
Box Shadow: None
Line Height: 14px
Hover State: Background #111111 (darker charcoal)
Active State: Background #000000 (true black)
Disabled State: Background #AAAAAA, Text #FFFFFF, Opacity 0.6
```

#### Secondary Button (Light Text)
```
Background: Transparent
Text Color: #252121
Font: Montserrat, 13px, 600
Padding: 12px 30px
Height: 40px
Border Radius: 25px
Border: None
Box Shadow: None
Line Height: 14px
Hover State: Background #F5F5F5
Active State: Background #DAE5E6
Disabled State: Text #BBBBBB
```

#### Navigation Button (Minimal)
```
Background: Transparent
Text Color: #252121
Font: Montserrat, 13px, 500
Padding: 5px 26px
Height: 40px
Border Radius: 25px
Border: None
Box Shadow: None
Line Height: 14px
Hover State: Text #F26822 (terracotta accent)
Active State: Text #252121, Weight 600
```

#### Accent Button (Future Use)
```
Background: #F26822
Text Color: #FFFFFF
Font: Montserrat, 13px, 600
Padding: 12px 30px
Height: 40px
Border Radius: 25px
Border: None
Box Shadow: None
Line Height: 14px
Hover State: Background #A74414 (darker rust)
Active State: Background #8B3410
Disabled State: Background #BBBBBB, Opacity 0.6
```

### Inputs & Forms

#### Text Input
```
Background: #FFFFFF
Text Color: #252121
Font: Montserrat, 13px, 400
Padding: 1px 2px 1px 20px (left padding for icon/focus)
Height: 48px
Border Radius: 25px
Border: 1px solid #DAE5E6
Box Shadow: None
Line Height: 19.5px
Placeholder Text: #AAAAAA
Focus State: Border #252121 (2px), Box Shadow 0 0 0 3px rgba(242, 104, 34, 0.1)
Error State: Border #EA1414, Background #FFF5F5
Disabled State: Background #F5F5F5, Text #AAAAAA, Border #BBBBBB
```

#### Email Input (Newsletter Signup)
```
Background: #FFFFFF
Text Color: #252121
Font: Montserrat, 13px, 400
Padding: 1px 2px 1px 20px
Height: 48px
Border Radius: 25px
Border: None
Box Shadow: None
Line Height: 19.5px
Placeholder Text: "Your Email Address", #AAAAAA
Focus State: Border 2px solid #252121
Error State: Border 2px solid #EA1414, Background #FFF5F5
Autofill State: Background #FFFBF0
```

### Cards & Containers

#### Content Card
```
Background: #FFFFFF
Border: 1px solid #DAE5E6
Border Radius: 6px
Padding: 32px
Box Shadow: None
Hover State: Border #252121 (2px)
```

#### Mobile App Card (Featured)
```
Background: #FFFFFF
Border: 3px solid #252121
Border Radius: 6px
Padding: 20px
Box Shadow: None
Typography Override: Montserrat, 14px, 600
```

#### Testimonial / Quote Card
```
Background: #FCE1D3
Border: None
Border Radius: 0px
Padding: 24px 32px
Left Border: 4px solid #F26822
Quote Mark Color: #F26822
Text Color: #252121
Font: Source Serif Pro, 18px, 600
Line Height: 29.7px
```

### Navigation

#### Main Navigation
```
Background: #DAE5E6 (light header background, inferred from screenshot)
Text Color: #252121
Font: Source Serif Pro, 16px, 400
Height: 40px
Line Height: 26.4px
Horizontal Spacing: 24px between items
Active Link: Font Weight 600, Color #252121
Hover State: Text #F26822
```

#### Mobile Navigation (Inferred)
```
Background: #FFFFFF
Border Top: 1px solid #DAE5E6
Text Color: #252121
Font: Source Serif Pro, 16px, 400
Padding: 16px 20px
Active Item: Background #F5F5F5, Left Border 4px #F26822
```

### Badges & Labels

#### Status Badge
```
Background: #FCE1D3
Text Color: #252121
Font: Montserrat, 10.4px, 600
Padding: 4px 12px
Border Radius: 12px
Line Height: 14px
```

#### Featured Number Badge (Testimonial Count)
```
Background: Transparent
Text Color: #F26822
Font: Montserrat, 24px, 800
Padding: 0px
Border: 2px solid #F26822
Border Radius: 50%
Width: 80px
Height: 80px
Display: Flex, Center
Line Height: 36px
```

### Links

#### Inline Link (Editorial)
```
Text Color: #252121
Font: Source Serif Pro, 16px, 400
Text Decoration: Underline
Underline Color: #F26822
Line Height: 26.4px
Hover State: Text Color #F26822
Active State: Text Color #A74414
```

#### White Link (On Dark Background)
```
Text Color: #FFFFFF
Font: Source Serif Pro, 18px, 600
Text Decoration: None
Line Height: 29.7px
Hover State: Text Color #FCE1D3
Active State: Text Color #F26822
```

## 5. Layout Principles

### Spacing System

**Base Unit:** 4px

**Spacing Scale:**
- **4px:** Fine-grained gaps between inline elements, icon-to-text spacing
- **8px:** Inferred; minimal spacing between related items
- **16px:** Gap between sibling content elements
- **20px:** Padding within contained sections
- **24px:** Margin between major content blocks
- **32px:** Padding within cards and containers
- **36px:** Large padding for container interiors
- **40px:** Margin between major sections
- **48px:** Section margin on desktop
- **52px:** Large section separation
- **56px:** Padding for premium content areas
- **72px:** Padding for hero sections and maximum spacing
- **84px:** Gap between independent major sections

**Usage Context:**
- **4px – 16px:** Internal component spacing (padding, gaps)
- **20px – 40px:** Local content grouping
- **48px – 84px:** Page-level section separation

### Grid & Container

**Maximum Width:** 1200px (inferred from desktop layout)

**Container Strategy:**
- Full-width hero sections with centered content max-width
- Multi-column layouts on desktop using 12-column grid
- Gutters: 24px (between columns)

**Section Patterns:**
- Header: Full width, background `#DAE5E6`
- Hero: Full width, centered content, background `#FFFFFF`
- Content Areas: Centered max-width with side padding
- Footer: Full width, structured grid

### Whitespace Philosophy

Whitespace is treated as a primary design element, not a byproduct. Generous margins and padding create visual rhythm and hierarchy. Key principles:

- **Breathing Room:** Minimum 24px padding around major content blocks
- **Section Separation:** Minimum 48px vertical space between distinct sections
- **Content Emphasis:** More whitespace around high-priority CTAs and messaging
- **Readability:** Line-height exceeds 1.4× font size for comfortable reading
- **Visual Hierarchy:** Strategic whitespace isolates and emphasizes important elements

### Border Radius Scale

- **0px:** Blocks, hard-edge containers (legacy cards, certain borders)
- **6px:** Card and container corners for slight softness
- **12px:** Badge and small component corners
- **25px:** Buttons and input fields; fully rounded for pill-shaped appearance
- **50%:** Circular elements (avatar containers, percentage-based badges)

## 6. Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| 0 (Flat) | No shadow, solid borders only | Buttons, navigation, standard cards |
| 1 (Subtle) | `0 1px 2px rgba(0, 0, 0, 0.05)` | Input focus states, hovered cards |
| 2 (Soft) | `0 2px 4px rgba(0, 0, 0, 0.08)` | Card hover states, dropdown indicators |
| 3 (Pronounced) | `0 4px 12px rgba(0, 0, 0, 0.12)` | Modals, overlays, premium content cards |

**Shadow Philosophy:** The Mark Manson design system employs minimal shadows, preferring borders and color contrast for visual hierarchy. Shadows are reserved for transient states (hover, focus) and overlaying content (modals, dropdowns). This keeps the design clean and editorial-focused while maintaining modern depth perception. All shadows use neutral black with low opacity to avoid color cast.

**Inferred Elevation Rules:**
- Primary UI components (buttons, navigation): No shadow
- Secondary interactions (card hover): Subtle shadow with border enhancement
- Modal overlays: Level 3 shadow with overlay backdrop
- Form inputs on focus: Level 1 shadow with colored border

## 7. Do's and Don'ts

### Do

- **Use Montserrat for all UI, navigation, and buttons** to maintain consistent modernity and clarity
- **Use Source Serif Pro for body text and editorial content** to establish credibility and brand voice
- **Apply terracotta orange (`#F26822`) sparingly** for highlights, testimonials, and primary accents—it should never be a background color for text
- **Maintain minimum touch target of 40px height** for buttons and interactive elements on all devices
- **Include generous whitespace (minimum 24px padding)** around major content blocks to improve readability
- **Use high-contrast text on colored backgrounds** to ensure WCAG AA compliance (minimum 4.5:1 ratio)
- **Stack vertical spacing in multiples of 4px** to maintain rhythm and alignment to baseline grid
- **Employ rounded pill-shaped buttons (25px radius)** as the standard for primary interactions
- **Reserve weight 800 for headings only** to prevent visual noise and maintain hierarchy
- **Leverage the neutral palette (`#DAE5E6`, `#AAAAAA`)** for secondary information and disabled states

### Don't

- **Never use orange as a text color on light backgrounds**—contrast becomes illegible; use it only for icons, borders, and accents
- **Don't mix serif and sans-serif in the same text block** without intentional hierarchy (one must be clearly secondary)
- **Avoid shadows on primary buttons and static components**—shadow should signal interactivity or depth only
- **Never reduce line height below 1.4× font size** in body text; readability will suffer on screens
- **Don't use true black (`#000000`) for body text**; use dark charcoal (`#252121`) for reduced eye strain
- **Avoid full-width layouts on desktop without max-width constraint** (1200px recommended); line length becomes unreadable
- **Never apply color to multiple buttons in the same group**—one primary, others secondary or ghost
- **Don't use gray text smaller than 14px**; small type in neutral colors becomes invisible
- **Avoid border radius greater than 25px** on non-circular elements; looks unfinished
- **Never stack more than 3 different font weights** on one page; contrast is diluted and hierarchy becomes unclear

## 8. Responsive Behavior

### Breakpoints

| Breakpoint | Width | Key Changes | Grid Cols |
|------------|-------|-------------|-----------|
| Mobile | 320px – 599px | Single column, full-width padding 16px, headline sizes reduced to 48px (H1), button full width, input full width | 1 |
| Tablet | 600px – 1023px | Two-column layout, padding 24px, H1 reduced to 64px, inputs max-width 480px, partial gutters | 2 |
| Desktop | 1024px+ | Multi-column, max-width container 1200px, full typography scale, button groups horizontal, inputs max-width 480px | 12 (inferred) |

### Touch Targets

- **Minimum touch target:** 40px × 40px (enforced on all buttons and interactive elements)
- **Buttons:** 40px height minimum, padding 12px 30px for adequate tap area
- **Input fields:** 48px height minimum for comfortable text entry
- **Navigation links:** 40px line height, 16px padding horizontal for easy selection on mobile
- **Icons:** Minimum 24px × 24px, with 8px surrounding whitespace for accidental tap tolerance

### Collapsing Strategy

**Mobile (320px – 599px):**
- H1 reduces from 80px → 48px
- H2 reduces from 56px → 36px
- Padding collapses to 16px (sides), 24px (vertical)
- Navigation becomes single-column menu with hamburger toggle
- Buttons and inputs span full width
- Two-column cards stack to single column
- Hero section maintains full width; internal padding increases

**Tablet (600px – 1023px):**
- H1: 64px (from 80px)
- H2: 44px (from 56px)
- Navigation becomes horizontal scrollable on small tablet, fixed row on larger tablet
- Two-column content grid introduced for content areas
- Buttons remain full width on card forms; sidebar buttons group horizontally
- Input width max 480px as specified

**Desktop (1024px+):**
- Full typography scale
- Max-width container at 1200px with centered alignment
- Multi-column layouts fully available
- Navigation fixed or sticky
- Sidebar patterns available for secondary content

## 9. Agent Prompt Guide

### Quick Color Reference

When implementing Mark Manson components, use these semantic color mappings:

- **Primary CTA Background:** Charcoal Black (`#252121`)
- **Primary CTA Text:** Pure White (`#FFFFFF`)
- **Secondary CTA Background:** Transparent
- **Secondary CTA Text:** Charcoal Black (`#252121`)
- **Accent Highlight:** Terracotta Orange (`#F26822`)
- **Heading Text:** Charcoal Black (`#252121`)
- **Body Text:** Charcoal Black (`#252121`) for sans-serif UI, Source Serif Pro for editorial
- **Placeholder / Disabled:** Medium Gray (`#AAAAAA`)
- **Borders / Dividers:** Light Gray (`#DAE5E6`)
- **Error State:** Error Red (`#EA1414`)
- **Warning State:** Warning Gold (`#E3B200`)
- **Background (Primary):** Pure White (`#FFFFFF`)
- **Background (Secondary):** Off-White (`#F5F5F5`)
- **Background (Featured):** Cream (`#FCE1D3`)
- **Background (Navigation):** Light Gray (`#DAE5E6`)
- **Overlay / Focus Tint:** Terracotta with 10% opacity `rgba(242, 104, 34, 0.1)`

### Iteration Guide

1. **Foundation First:** All text defaults to Charcoal Black (`#252121`); all backgrounds default to Pure White (`#FFFFFF`). Deviation requires intentional design purpose.

2. **Typography Precedence:** Use Montserrat for UI, buttons, labels, and navigation. Use Source Serif Pro only for body paragraphs, long-form editorial, and testimonials. Never mix fonts in a single component without clear hierarchy.

3. **Button Grammar:** Primary buttons are filled dark (`#252121` background, `#FFFFFF` text); secondary buttons are transparent with dark text; accent use is rare and reserved for special CTAs. All buttons must reach minimum 40px height and use 25px border radius.

4. **Spacing Discipline:** Base all spacing on 4px units. Apply whitespace in multiples: 4px, 16px, 24px, 32px, 48px, 72px. Padding within components ≥20px; margin between sections ≥24px on mobile, ≥48px on desktop.

5. **Accent Restraint:** Terracotta Orange (`#F26822`) is for accents, icons, testimonial highlights, and error alternatives only. Never use as body text background or input fill.

6. **Border Radius Standard:** Buttons and inputs use 25px (pill shape); cards use 6px; most UI defaults to 0px (sharp edges). Only deviate if component requires distinction.

7. **Interactive Feedback:** Hover states change color or add subtle shadow (Level 1). Focus states add a 2px border. Disabled states reduce opacity to 0.6 and shift text to medium gray.

8. **Responsive Scaling:** H1 starts 80px desktop, 64px tablet, 48px mobile. All other sizes scale proportionally. Container max-width never exceeds 1200px. Gutters: 24px desktop, 16px mobile.

9. **Semantic Color Accuracy:** Use the exact hex values provided—never approximate shades. Error states always use the error red family (`#EA1414` primary). Warnings use gold (`#E3B200`). Status indicators use cream background with terracotta border.

10. **Accessibility Compliance:** All text on colored backgrounds must achieve minimum 4.5:1 contrast ratio. Line height must be ≥1.4× font size. Touch targets: 40px minimum. Button text: always 600+ weight for legibility.