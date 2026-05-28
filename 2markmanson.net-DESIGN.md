# Design System Inspired by Mark Manson

## 1. Visual Theme & Atmosphere

Mark Manson's design system embodies a pragmatic, no-nonsense aesthetic that mirrors his philosophy of straightforward life advice. The visual language combines refined typography with bold, minimal interactions to create an authoritative yet approachable digital presence. The palette balances deep, confident neutrals with strategic pops of warmth (burnt orange) that signal authenticity and energy. Clean whitespace, generous padding, and deliberate use of serif and sans-serif typefaces create a sophisticated, readable experience that prioritizes clarity over decoration. The overall feeling is one of trustworthy expertise—modern without being trendy, bold without being loud.

**Key Characteristics**

- Deep neutral foundation (`#252121`, `#111111`) establishes authority and readability
- Strategic accent color (`#F26822`) adds warmth and draws attention to key actions
- Generous whitespace and breathing room conveys confidence
- Mixed serif (Source Serif Pro) and sans-serif (Montserrat) creates hierarchy and visual interest
- Pill-shaped buttons (`25px` radius) suggest friendly, approachable interaction
- High contrast between text and background ensures accessibility
- Minimal use of shadows—relies on color and typography instead

## 2. Color Palette & Roles

### Primary

- **Deep Charcoal** (`#252121`): Primary text, headings, dominant UI element color—conveys authority and forms the backbone of the interface
- **Off-Black** (`#111111`): Secondary dark text, subtle borders, support text in high-contrast scenarios
- **True Black** (`#000000`): Maximum contrast elements, critical emphasis

### Accent Colors

- **Burnt Orange** (`#F26822`): Call-to-action accents, highlights, social proof badges—energizes the interface with warmth
- **Warm Peach** (`#FCE1D3`): Soft background tint for highlighted sections, gentle visual differentiation
- **Dark Rust** (`#A74414`): Secondary accent for hover states or deeper prominence

### Interactive

- **Primary Action** (`#252121`): Filled button backgrounds, primary form submissions
- **Secondary Action** (`#495A5F`): Muted interactive states, alternative actions
- **Accent Link** (`#21759B`): Hyperlinks and interactive text elements that need distinction

### Neutral Scale

- **White** (`#FFFFFF`): Primary background, card surfaces, text on dark backgrounds
- **Light Gray** (`#F5F5F5`): Secondary background, subtle section separation
- **Pale Blue-Gray** (`#DAE5E6`): Form field backgrounds, subtle dividers
- **Medium Gray** (`#BBBBBB`): Disabled text, placeholder text, secondary content
- **Dim Gray** (`#AAAAAA`): Tertiary text, reduced emphasis information

### Surface & Borders

- **Pale Blue-Gray** (`#DAE5E6`): Subtle border color, section dividers
- **Off-White** (`#F5F5F5`): Soft container backgrounds
- **White** (`#FFFFFF`): Primary container and card surfaces

### Semantic / Status

- **Error Red** (`#EA1414`, `#BD2525`, `#D1193E`): Form validation errors, destructive warnings—use `#EA1414` as primary error state
- **Warning Yellow** (`#E3B200`): Caution alerts, warning messages, non-critical notifications

## 3. Typography Rules

### Font Family

**Primary Font:** Montserrat (sans-serif)
Fallback stack: `Montserrat, -apple-system, BlinkMacSystemFont, 'Segoe UI', Arial, sans-serif`
Usage: Headings, buttons, labels, body text (primary interface text)

**Secondary Font:** Source Serif Pro (serif)
Fallback stack: `'Source Serif Pro', Georgia, 'Times New Roman', serif`
Usage: Navigation links, supporting text, editorial content, emphasis spans

### Hierarchy

| Role | Font | Size | Weight | Line Height | Letter Spacing | Notes |
|------|------|------|--------|-------------|-----------------|-------|
| Display / H1 | Montserrat | 80px | 700 | 96px | 0px | Hero headlines, page titles |
| Heading 2 | Montserrat | 56px | 700 | 72.8px | 0px | Major section headings |
| Heading 4 | Montserrat | 24px | 800 | 36px | 0px | Subsection headings |
| Heading 5 | Montserrat | 14px | 500 | 16px | 0px | Small headings, labels |
| Heading 6 | Montserrat | 18px | 700 | 27px | 0px | Card titles, emphasis |
| Body | Montserrat | 14px | 400 | 16px | 0px | Primary body copy, paragraphs |
| Button | Montserrat | 13px | 600 | 14px | 0px | Interactive button text |
| Input | Montserrat | 13px | 400 | 19.5px | 0px | Form field text, placeholder |
| Small / Caption | Montserrat | 10.4px | 600 | 14px | 0px | Metadata, captions, helper text |
| Serif Emphasis | Source Serif Pro | 18px | 600 | 29.7px | 0px | Highlighted quotes, emphasis text |
| Link / Navigation | Source Serif Pro | 16px | 400 | 26.4px | 0px | Navigation items, editorial links |

### Principles

- **Clear Hierarchy**: Size and weight differentiation guide visual scanning; larger sizes for critical information
- **Generous Leading**: Line heights exceed font size (1.2–1.5x multiplier) for readability and breathing room
- **Serif for Emphasis**: Source Serif Pro creates editorial distinction and signals secondary navigation or quotes
- **Bold Action Text**: Buttons use `600–800` weight to signal interactivity
- **Consistent Tracking**: Maintain `0px` letter spacing for natural readability unless emphasis is required

## 4. Component Stylings

### Buttons

#### Primary Button (Filled Dark)
- **Background**: `#252121`
- **Text Color**: `#FFFFFF`
- **Font**: Montserrat, `13px`, weight `600`, line-height `14px`
- **Padding**: `12px 30px`
- **Border Radius**: `25px`
- **Border**: `1px solid transparent`
- **Box Shadow**: `none`
- **Height**: `40px`
- **Hover State**: Background `#111111`, text `#FFFFFF`
- **Active State**: Background `#000000`, text `#FFFFFF`
- **Disabled State**: Background `#BBBBBB`, text `#FFFFFF`, cursor `not-allowed`

#### Secondary Button (Outlined/Ghost)
- **Background**: `transparent`
- **Text Color**: `#252121`
- **Font**: Montserrat, `13px`, weight `600`, line-height `14px`
- **Padding**: `12px 30px`
- **Border Radius**: `25px`
- **Border**: `1px solid #252121`
- **Box Shadow**: `none`
- **Height**: `40px`
- **Hover State**: Background `#F5F5F5`, text `#252121`, border `1px solid #252121`
- **Active State**: Background `#DAE5E6`, text `#111111`, border `1px solid #111111`

#### Tertiary Button (Minimal/Navigation)
- **Background**: `transparent`
- **Text Color**: `#252121`
- **Font**: Montserrat, `13px`, weight `500`, line-height `14px`
- **Padding**: `5px 0px 5px 26px`
- **Border Radius**: `25px`
- **Border**: `none`
- **Box Shadow**: `none`
- **Height**: `40px`
- **Hover State**: Text `#F26822`
- **Active State**: Text `#A74414`

#### Icon Button
- **Background**: `transparent`
- **Text Color**: `#252121`
- **Font**: Montserrat, `13px`, weight `600`, line-height `14px`
- **Padding**: `0px`
- **Border Radius**: `25px`
- **Border**: `none`
- **Box Shadow**: `none`
- **Height**: `24px`
- **Width**: `24px`
- **Hover State**: Background `#F5F5F5`, text `#F26822`

### Cards & Containers

#### Standard Card
- **Background**: `#FFFFFF`
- **Border**: `1px solid #DAE5E6`
- **Border Radius**: `6px`
- **Padding**: `24px` (or `32px` for larger cards)
- **Box Shadow**: `0px 1px 3px rgba(0, 0, 0, 0.08)`
- **Text Color**: `#252121`
- **Hover State**: Border `1px solid #BBBBBB`, box-shadow `0px 2px 8px rgba(0, 0, 0, 0.12)`

#### Featured/Highlighted Card
- **Background**: `#FCE1D3`
- **Border**: `1px solid #F26822`
- **Border Radius**: `6px`
- **Padding**: `24px`
- **Box Shadow**: `0px 2px 8px rgba(242, 104, 34, 0.15)`
- **Text Color**: `#252121`

#### Hero Section Container
- **Background**: `#DAE5E6`
- **Padding**: `72px 56px`
- **Border Radius**: `0px`
- **Text Color**: `#252121`

### Inputs & Forms

#### Text Input
- **Background**: `#FFFFFF`
- **Text Color**: `#252121`
- **Font**: Montserrat, `13px`, weight `400`, line-height `19.5px`
- **Padding**: `12px 20px`
- **Border Radius**: `25px`
- **Border**: `1px solid #DAE5E6`
- **Height**: `48px`
- **Placeholder Color**: `#AAAAAA`
- **Focus State**: Border `1px solid #F26822`, outline `none`, box-shadow `0px 0px 0px 3px rgba(242, 104, 34, 0.1)`
- **Error State**: Border `1px solid #EA1414`, background `#FFFFFF`
- **Disabled State**: Background `#F5F5F5`, border `1px solid #BBBBBB`, color `#BBBBBB`

#### Email Input (Newsletter)
- **Background**: `#FFFFFF`
- **Text Color**: `#252121`
- **Font**: Montserrat, `13px`, weight `400`, line-height `19.5px`
- **Padding**: `12px 20px`
- **Border Radius**: `25px`
- **Border**: `1px solid #DAE5E6`
- **Height**: `48px`
- **Width**: `100%` (responsive, max `480px`)
- **Focus State**: Border `1px solid #F26822`, box-shadow `0px 0px 0px 3px rgba(242, 104, 34, 0.1)`

#### Form Label
- **Font**: Montserrat, `14px`, weight `600`, line-height `16px`
- **Text Color**: `#252121`
- **Margin Bottom**: `8px`

#### Helper Text / Caption
- **Font**: Montserrat, `10.4px`, weight `600`, line-height `14px`
- **Text Color**: `#AAAAAA`
- **Margin Top**: `4px`

### Navigation

#### Primary Navigation Bar
- **Background**: `#FFFFFF` (or `#DAE5E6` on hero sections)
- **Height**: `64px`
- **Padding**: `16px 40px`
- **Border Bottom**: `1px solid #DAE5E6`
- **Display**: Flex, align-items center, justify-content space-between

#### Navigation Link
- **Font**: Source Serif Pro, `16px`, weight `400`, line-height `26.4px`
- **Text Color**: `#252121`
- **Padding**: `8px 12px`
- **Text Decoration**: `none`
- **Hover State**: Text `#F26822`, text-decoration `underline`
- **Active State**: Text `#F26822`, font-weight `600`

#### Navigation Logo/Brand
- **Font**: Montserrat, `18px`, weight `700`, line-height `27px`
- **Text Color**: `#252121`
- **Letter Spacing**: `1px`

### Links

#### Inline Link
- **Font**: Source Serif Pro, `16px`, weight `400`, line-height `26.4px`
- **Text Color**: `#21759B`
- **Text Decoration**: `underline`
- **Cursor**: `pointer`
- **Hover State**: Text `#252121`, text-decoration `underline`
- **Visited State**: Text `#495A5F`

#### White Link (on dark background)
- **Font**: Source Serif Pro, `18px`, weight `600`, line-height `29.7px`
- **Text Color**: `#FFFFFF`
- **Text Decoration**: `underline`
- **Hover State**: Text `#DAE5E6`, text-decoration `underline`

### Badges & Labels

#### Accent Badge (Orange)
- **Background**: `#F26822`
- **Text Color**: `#FFFFFF`
- **Font**: Montserrat, `13px`, weight `600`, line-height `14px`
- **Padding**: `6px 12px`
- **Border Radius**: `16px`
- **Display**: Inline-block

#### Neutral Badge
- **Background**: `#F5F5F5`
- **Text Color**: `#252121`
- **Font**: Montserrat, `13px`, weight `600`, line-height `14px`
- **Padding**: `6px 12px`
- **Border Radius**: `16px`
- **Border**: `1px solid #DAE5E6`

## 5. Layout Principles

### Spacing System

**Base Unit**: `4px`

**Scale**: `4px`, `8px`, `12px`, `16px`, `20px`, `24px`, `32px`, `36px`, `40px`, `48px`, `56px`, `72px`, `84px`

**Usage Context**:
- `4px`: Micro gaps between tightly grouped elements
- `8px – 12px`: Spacing between form fields, buttons
- `16px`: Padding inside buttons, gap between inline elements
- `20px – 24px`: Padding inside cards, margin between list items
- `32px – 40px`: Vertical spacing between sections
- `48px – 56px`: Margin between major content sections
- `72px – 84px`: Vertical gap between hero and main content, footer spacing

### Grid & Container

- **Max Width**: `1200px` (full bleed for hero sections, contained for body content)
- **Container Padding**: `40px` (desktop), `24px` (tablet), `16px` (mobile)
- **Column Strategy**: 12-column fluid grid; cards/content use `1/2`, `1/3`, or full width depending on breakpoint
- **Section Pattern**: Full-width hero sections (`#DAE5E6` or `#FFFFFF`) with centered content container; alternating light/white backgrounds for visual rhythm

### Whitespace Philosophy

Whitespace is treated as a primary design element that conveys confidence and clarity. Generous padding (`32px – 72px`) surrounds major sections; content is never cramped. Breathing room around text and interactive elements reduces cognitive load and creates visual hierarchy. Vertical rhythm is maintained through consistent spacing multipliers—content feels intentional rather than arbitrary.

### Border Radius Scale

- `0px`: Sections, full-width containers, hero backgrounds
- `6px`: Cards, form containers, image frames
- `16px`: Badges, labels, small UI elements
- `25px`: Buttons (primary call-to-action), form inputs, pill-shaped interactive elements

## 6. Depth & Elevation

| Level | Treatment | Use |
|-------|-----------|-----|
| Base (0) | No shadow, flat color | Primary surfaces, page backgrounds |
| Level 1 | `0px 1px 3px rgba(0, 0, 0, 0.08)` | Cards at rest, subtle hover states |
| Level 2 | `0px 2px 8px rgba(0, 0, 0, 0.12)` | Hovered cards, input focus, dropdown menus |
| Level 3 | `0px 4px 16px rgba(0, 0, 0, 0.15)` | Modals, elevated panels, primary focus states |
| Accent Glow | `0px 0px 0px 3px rgba(242, 104, 34, 0.1)` | Input focus ring (branded), accent emphasis |

**Shadow Philosophy**

This design system favors restraint with shadows. Rather than heavy drop shadows, subtle elevation is communicated through border color shifts and focus states. Accent shadows (orange glow on inputs) reinforce the brand while maintaining readability. Shadows are soft and diffused to avoid harsh, plasticky effects; they exist to clarify hierarchy without distraction.

## 7. Do's and Don'ts

### Do

- **Use clear visual hierarchy** through size, weight, and color—headings should immediately stand out from body text
- **Maintain high contrast** between text and background (`#252121` on `#FFFFFF` is ideal)
- **Employ generous whitespace** around interactive elements to reduce accidental clicks and improve scannability
- **Apply the burnt orange (`#F26822`)** sparingly for critical actions, social proof badges, and hover states
- **Use Source Serif Pro for navigation and links** to differentiate them from body copy and create editorial elegance
- **Default buttons to filled dark (`#252121`)** for primary actions; use ghost/outline variants for secondary choices
- **Ensure all text meets WCAG AA contrast standards** (4.5:1 for body, 3:1 for large text)
- **Test form inputs across browsers**—maintain `25px` border radius and `48px` minimum height for touch accessibility
- **Stack sections vertically** with full-width alternating backgrounds (`#FFFFFF` / `#DAE5E6`) for rhythm
- **Use consistent `4px` base unit** for spacing; multiples of `4px` maintain alignment grid

### Don't

- **Mix serif and sans-serif within the same line of text**—use clearly separated layers (e.g., heading in Montserrat, body in Montserrat, link in Serif)
- **Reduce button padding below `12px 30px`**—maintains touch target size and visual affordance
- **Stack more than 2–3 levels of headings on one page**—risks visual chaos
- **Use orange (`#F26822`) as a background color** for extended text areas—reserve it for accents, badges, and hover states
- **Apply multiple shadow levels to the same element**—choose one elevation level and commit
- **Deviate from the `25px` button border radius**—it's a key brand signature; use `6px` only for cards/containers
- **Ignore placeholder text contrast**—`#AAAAAA` is the minimum acceptable; test with real users if lower contrast is considered
- **Nest form inputs deeper than one level** without clear visual grouping—maintain flat structure for clarity
- **Use more than 2 accent colors on a single page**—orange is primary; blues/teals are secondary; avoid simultaneous emphasis
- **Forget to test responsive behavior**—ensure button height/width, input width, and spacing reflow gracefully on mobile

## 8. Responsive Behavior

### Breakpoints

| Name | Width | Key Changes |
|------|-------|-------------|
| Mobile | `< 640px` | Single-column layout, `16px` padding, `56px` heading, `14px` body, full-width inputs, stacked buttons |
| Tablet | `640px – 1024px` | 2-column grid where appropriate, `24px` padding, `48px` heading, `14px` body, `50%` input width, side-by-side buttons |
| Desktop | `≥ 1024px` | Multi-column layouts, `40px` padding, full typography scale, max-width containers (`1200px`), inline form controls |

### Touch Targets

- **Minimum Touch Target**: `48px × 48px` (button height `40px` + `4px` padding)
- **Comfortable Target**: `56px × 56px` (form inputs at `48px` height, buttons at `40px` with surrounding whitespace)
- **Spacing Between Targets**: Minimum `8px` gap to prevent accidental activation
- **Icon Button Exception**: `24px × 24px` minimum (typically placed in less dense areas like headers)

### Collapsing Strategy

- **Hero Sections**: Reduce padding from `72px 56px` (desktop) → `48px 24px` (tablet) → `32px 16px` (mobile); h1 scales from `80px` → `56px` → `40px`
- **Navigation**: Collapse primary nav into hamburger menu at `< 768px`; logo remains visible at all breakpoints
- **Multi-Column Grids**: Shift from 3 columns (desktop) → 2 columns (tablet) → 1 column (mobile); maintain `16px` gap between columns
- **Form Inputs**: Full width on mobile (`width: 100%`, max-width `480px` on tablet, fixed `480px` on desktop)
- **Buttons**: Stack vertically on mobile (full-width), side-by-side on tablet/desktop
- **Card Grid**: 3 cards per row (desktop) → 2 per row (tablet) → 1 per row (mobile), maintain `24px` gap
- **Footer**: Single column on mobile, multi-column on tablet/desktop

## 9. Agent Prompt Guide

### Quick Color Reference

- **Primary CTA**: Deep Charcoal (`#252121`)
- **Accent Highlight**: Burnt Orange (`#F26822`)
- **Background**: White (`#FFFFFF`) and Pale Blue-Gray (`#DAE5E6`)
- **Primary Text**: Deep Charcoal (`#252121`)
- **Secondary Text**: Medium Gray (`#BBBBBB`)
- **Disabled State**: Dim Gray (`#AAAAAA`)
- **Error State**: Error Red (`#EA1414`)
- **Link**: Teal Blue (`#21759B`)
- **Card Surface**: White (`#FFFFFF`) with `1px solid #DAE5E6` border
- **Form Input**: White (`#FFFFFF`) with `1px solid #DAE5E6` border, `25px` radius

### Iteration Guide

1. **Typography First**: All text must use Montserrat (sans-serif) or Source Serif Pro (serif); respect the hierarchy table exactly—no deviations from specified px/weight/line-height
2. **Button Defaults**: All buttons start as `25px` border-radius pill shapes, `40px` height, `12px 30px` padding; filled buttons use `#252121` background with `#FFFFFF` text; ghost buttons use transparent background with `#252121` text and `1px solid #252121` border
3. **Color Discipline**: `#252121` is the dominant color (473 uses); `#F26822` is reserved for accents/actions (15 uses); use `#FFFFFF` (`#FFFFFF`, 149 uses) as primary surface
4. **Spacing Grid**: All spacing uses `4px` base unit; use `16px`, `24px`, `40px`, `56px`, `72px` for consistent rhythm; never use arbitrary values
5. **Input Styling**: All form inputs are `48px` height, `25px` border radius, `12px 20px` padding, `#FFFFFF` background, `1px solid #DAE5E6` border; focus state adds orange glow `0px 0px 0px 3px rgba(242, 104, 34, 0.1)`
6. **Cards & Containers**: Use `6px` border radius (not `25px`), `1px solid #DAE5E6` border, `24px` padding (or `32px` for larger); hover state shifts border to `#BBBBBB` and adds Level 2 shadow
7. **Navigation**: Navigation links use Source Serif Pro `16px` weight `400`; hover state is `#F26822` with underline; logo is Montserrat `18px` weight `700`
8. **Responsive Priority**: Mobile first—start at `< 640px`, progressively enhance; ensure all text scales (h1: `40px` mobile → `80px` desktop); buttons and inputs remain full-width until tablet breakpoint
9. **Contrast & Accessibility**: All text must meet WCAG AA (4.5:1 minimum); verify `#252121` on `#FFFFFF` (18:1 ratio—excellent); orange accents on white are acceptable; placeholder text `#AAAAAA` on `#FFFFFF` is 7.5:1 (sufficient)
10. **Shadows Minimalism**: Use only Level 1 (`0px 1px 3px rgba(0, 0, 0, 0.08)`) or Level 2 (`0px 2px 8px rgba(0, 0, 0, 0.12)`) shadows; never stack shadows; reserve Level 3 for rare modals; prefer border color and typography for hierarchy