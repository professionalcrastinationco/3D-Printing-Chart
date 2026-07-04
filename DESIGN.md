---
name: Precision Core
colors:
  surface: '#f8f9ff'
  surface-dim: '#d0dbed'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e6eeff'
  surface-container-high: '#dee9fc'
  surface-container-highest: '#d9e3f6'
  on-surface: '#121c2a'
  on-surface-variant: '#414755'
  inverse-surface: '#27313f'
  inverse-on-surface: '#eaf1ff'
  outline: '#717786'
  outline-variant: '#c1c6d7'
  surface-tint: '#005bc1'
  primary: '#0058bc'
  on-primary: '#ffffff'
  primary-container: '#0070eb'
  on-primary-container: '#fefcff'
  inverse-primary: '#adc6ff'
  secondary: '#006c49'
  on-secondary: '#ffffff'
  secondary-container: '#6cf8bb'
  on-secondary-container: '#00714d'
  tertiary: '#825100'
  on-tertiary: '#ffffff'
  tertiary-container: '#a36700'
  on-tertiary-container: '#fffbff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d8e2ff'
  primary-fixed-dim: '#adc6ff'
  on-primary-fixed: '#001a41'
  on-primary-fixed-variant: '#004493'
  secondary-fixed: '#6ffbbe'
  secondary-fixed-dim: '#4edea3'
  on-secondary-fixed: '#002113'
  on-secondary-fixed-variant: '#005236'
  tertiary-fixed: '#ffddb8'
  tertiary-fixed-dim: '#ffb95f'
  on-tertiary-fixed: '#2a1700'
  on-tertiary-fixed-variant: '#653e00'
  background: '#f8f9ff'
  on-background: '#121c2a'
  surface-variant: '#d9e3f6'
typography:
  display-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
    letterSpacing: -0.01em
  title-sm:
    fontFamily: Hanken Grotesk
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-md:
    fontFamily: Hanken Grotesk
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Hanken Grotesk
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
  code-label:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
    letterSpacing: 0.02em
  table-header:
    fontFamily: Hanken Grotesk
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 48px
  container-max: 1440px
  gutter: 16px
---

## Brand & Style

The design system is engineered for technical clarity and comparative analysis. It targets a sophisticated audience of engineers, hobbyists, and industrial designers who require high-density data visualization without cognitive fatigue.

The brand personality is **Technical, Authoritative, and Precise.** It utilizes a **Modern Corporate** style infused with **Low-Contrast Outlines** to maintain a clean, organized structure. The aesthetic prioritizes function, using whitespace not just for breathing room, but as a deliberate separator for complex data sets. The interface should feel like a high-end laboratory instrument: reliable, neutral, and exceptionally sharp.

## Colors

The palette is anchored by a sophisticated range of deep grays and crisp whites to ensure a professional foundation. 

- **Primary (Electric Blue):** Reserved for primary actions, active states, and critical data points.
- **Secondary (Emerald Green):** Used for "Success" indicators, optimal filament properties, and positive comparisons.
- **Tertiary (Amber):** Used for warnings, transitional states, or moderate property ratings.
- **Neutrals:** A multi-layered gray scale facilitates the "Tonal Layering" strategy, differentiating headers from cell data.

For data visualization, use a high-contrast logic where the background remains neutral to allow the accent colors to signify performance metrics (e.g., strength bars or temperature ranges).

## Typography

This design system utilizes **Hanken Grotesk** for its exceptional legibility and modern, geometric structure. It provides a clean, professional "SaaS" feel that scales perfectly from large displays to dense data rows.

For technical specifications, units of measurement (e.g., MPa, °C, g/cm³), and status badges, **JetBrains Mono** is employed. This monospaced addition reinforces the technical nature of the tool and ensures that numerical values align vertically in comparison tables, aiding rapid scanning.

**Hierarchy Rules:**
- Use `table-header` for all column and row labels in the comparison matrix.
- `code-label` is the default for all technical units and badges.
- Maintain a strict high-contrast ratio for all body text to ensure WCAG AA compliance.

## Layout & Spacing

The layout follows a **Fixed Grid** philosophy for the main comparison engine to ensure the matrix remains readable on large screens, while transitioning to a **Fluid Grid** for mobile views.

- **Desktop:** 12-column grid, 24px margins, 16px gutters. Comparison columns should have a fixed minimum width of 120px to prevent data cramping.
- **Table Density:** A "Compact" vertical rhythm is used within the data grid (8px cell padding) to maximize the amount of information visible without scrolling.
- **Sticky Headers:** Both the top row (Filament Names) and the first column (Properties) must remain sticky during scroll to maintain context in large data sets.

## Elevation & Depth

To maintain a "technical" feel, the system avoids heavy shadows. Instead, it uses **Tonal Layering** and **Low-Contrast Outlines**.

- **Level 0 (Base):** The main background (`#FFFFFF`).
- **Level 1 (Surface):** Subtle gray fills (`#F9FAFB`) for alternating table rows (zebra striping) and sidebar navigation.
- **Level 2 (Floating):** Used for tooltips and dropdown menus. These utilize a very soft, highly diffused shadow (0px 4px 20px rgba(0,0,0,0.05)) and a 1px solid border (`#E5E7EB`).
- **Dividers:** Use 1px borders to define the grid of the comparison tool rather than depth effects. This keeps the focus on the data.

## Shapes

The shape language is **Soft (0.25rem)**. This provides a modern, approachable feel while maintaining the structural integrity of a grid-based tool. 

- **Buttons & Inputs:** Use the standard `rounded` (4px).
- **Badges/Chips:** Use `rounded-xl` (12px) to create a "pill" contrast against the rectangular grid cells.
- **Data Bars:** Comparison bars (e.g., strength or durability) should have 2px rounded corners on the fill indicators to feel integrated but distinct.

## Components

### Comparison Table
The core component. Features a "Sticky" header row with filament thumbnails. Cells use alternating zebra-striping. Hover states on cells should trigger a subtle highlight of the entire row and column to assist in cross-referencing.

### Data Visualization Bars
Used for 1-10 ratings. A background track of light gray with a foreground fill of Primary Blue or Secondary Green. Use a "segmented" bar style (10 distinct blocks) for easier value estimation.

### Status Badges
Used for "Required", "Optional", or "Recommended" hardware. 
- **Style:** Small text, uppercase, monospaced font. 
- **Colors:** Neutral background with dark text for "Optional"; Primary background for "Required".

### Input Fields & Selectors
Strictly rectangular with 4px corners. Use a 1px border that darkens on focus. Selection checkboxes for "Compare" should be high-contrast with a Primary Blue fill when active.

### Cards (Filament Preview)
Used in search results or "top-rated" sections. Minimalist design with a small image, title, and 2-3 key metrics (Price, Strength, Printability) displayed as compact labels.