---
name: Cybernetic Precision
colors:
  surface: '#0e1417'
  surface-dim: '#0e1417'
  surface-bright: '#333a3d'
  surface-container-lowest: '#080f11'
  surface-container-low: '#161d1f'
  surface-container: '#1a2123'
  surface-container-high: '#242b2d'
  surface-container-highest: '#2f3638'
  on-surface: '#dde4e6'
  on-surface-variant: '#bbc9ce'
  inverse-surface: '#dde4e6'
  inverse-on-surface: '#2a3234'
  outline: '#859398'
  outline-variant: '#3c494d'
  surface-tint: '#00d9ff'
  primary: '#afecff'
  on-primary: '#003641'
  primary-container: '#00d9ff'
  on-primary-container: '#005b6c'
  inverse-primary: '#00687b'
  secondary: '#cdbdff'
  on-secondary: '#370096'
  secondary-container: '#5203d5'
  on-secondary-container: '#c0acff'
  tertiary: '#58ffad'
  on-tertiary: '#003920'
  tertiary-container: '#00e391'
  on-tertiary-container: '#005f3a'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#aeecff'
  primary-fixed-dim: '#00d9ff'
  on-primary-fixed: '#001f26'
  on-primary-fixed-variant: '#004e5d'
  secondary-fixed: '#e8deff'
  secondary-fixed-dim: '#cdbdff'
  on-secondary-fixed: '#20005f'
  on-secondary-fixed-variant: '#4f00d0'
  tertiary-fixed: '#52ffac'
  tertiary-fixed-dim: '#00e290'
  on-tertiary-fixed: '#002111'
  on-tertiary-fixed-variant: '#005231'
  background: '#0e1417'
  on-background: '#dde4e6'
  surface-variant: '#2f3638'
typography:
  display-lg:
    fontFamily: Space Grotesk
    fontSize: 72px
    fontWeight: '700'
    lineHeight: 80px
    letterSpacing: -0.02em
  display-lg-mobile:
    fontFamily: Space Grotesk
    fontSize: 40px
    fontWeight: '700'
    lineHeight: 48px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Space Grotesk
    fontSize: 48px
    fontWeight: '600'
    lineHeight: 56px
  headline-md:
    fontFamily: Space Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
  body-lg:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-md:
    fontFamily: JetBrains Mono
    fontSize: 14px
    fontWeight: '500'
    lineHeight: 20px
    letterSpacing: 0.05em
  label-sm:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 16px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  grid-unit: 8px
  container-max: 1280px
  gutter: 24px
  margin-mobile: 20px
  section-padding: 120px
---

## Brand & Style

This design system is engineered for a high-end personal portfolio that bridges the gap between hardware engineering and software development. The brand personality is technical, avant-garde, and meticulously crafted, evoking the feeling of a sophisticated terminal or a high-performance electronic interface.

The design style is **Futuristic Glassmorphism** blended with **Cybernetic Brutalism**. It utilizes deep obsidian backgrounds, vibrant neon accents, and semi-transparent frosted surfaces to create a sense of depth and luminosity. The interface should feel like a premium piece of proprietary hardware: precise, illuminated, and high-energy. Key visual motifs include digital grid overlays, 1px "glowing" strokes, and subtle circuit-inspired patterns.

## Colors

The palette is anchored in a deep space-black core, designed exclusively for dark mode to maximize the impact of "light-emitting" accents.

- **Primary Blue (#00D9FF):** The main functional color, used for primary actions, active states, and glowing borders. It represents the "energy source" of the UI.
- **Accent Purple (#7C4DFF):** Used for secondary highlights, gradients, and to distinguish software-centric elements.
- **Accent Green (#00FFA3):** Reserved for "Success" states, system status indicators, and hardware-readout metaphors.
- **Highlight Orange (#FF8A00):** A high-contrast warning or "attention" color, used sparingly for critical call-to-outs or specific engineering milestones.
- **Glass Surfaces:** Semi-transparent layers use `#0C1F2D` at 60% opacity with a heavy backdrop blur (20px+) to maintain legibility against complex backgrounds.

## Typography

The typographic hierarchy balances futuristic geometry with technical readability.

- **Space Grotesk** is used for headlines to provide a cutting-edge, geometric feel that mimics high-tech branding.
- **Inter** provides a highly legible, neutral foundation for long-form content, project descriptions, and technical documentation.
- **JetBrains Mono** is utilized for labels, technical specs, and metadata to reinforce the "Full Stack Developer" and "Electronics Engineer" identity. It should be used whenever data or "readouts" are presented.

## Layout & Spacing

The layout follows a **Rigid Technical Grid**. All spacing is derived from an 8px base unit to ensure mathematical precision.

- **Desktop:** A 12-column fluid grid with 24px gutters. Use wide margins to create a "letterboxed" cinematic feel.
- **Mobile:** A 4-column grid. Large display headings should scale down aggressively to fit screen widths while maintaining their weight.
- **Visual Rhythm:** Use generous vertical section padding (120px+) to allow the "glowing" elements space to breathe and prevent the dark interface from feeling cramped.

## Elevation & Depth

Hierarchy is achieved through **Luminance and Blur** rather than traditional shadows.

1.  **Base Layer:** The deepest background (#06131E). Can feature a subtle fixed SVG grid pattern (1px lines at 5% opacity).
2.  **Mid Layer:** Semi-transparent glass cards with a 1px border (#00D9FF at 30% opacity). This layer uses `backdrop-filter: blur(24px)`.
3.  **Top Layer:** Active interactive elements (buttons, tooltips). These feature a "Glow" effect using `box-shadow: 0 0 15px rgba(0, 217, 255, 0.4)`.

Avoid standard black shadows; use colored ambient glows that match the nearest accent color to simulate light emission from the interface.

## Shapes

The shape language is "Soft-Technical." Elements use a **0.25rem (4px)** base radius to feel modern and engineered without becoming overly organic or "bubbly."

- **Small elements (Buttons/Inputs):** 4px radius.
- **Large elements (Cards/Containers):** 8px or 12px radius.
- **Accent Details:** Use 45-degree chamfered corners on specific decorative elements (like project tags) to mimic PCB (Printed Circuit Board) traces.

## Components

- **Buttons:** Primary buttons feature a solid #00D9FF fill with black text, accompanied by a subtle outer glow. Secondary buttons use a transparent background with a 1px #00D9FF border.
- **Glass Cards:** Containers for project highlights. They must have a 1px border. On hover, the border opacity increases from 30% to 100%.
- **Technical Chips:** Used for tech stacks (e.g., "React", "Embedded C"). Use JetBrains Mono font, a dark #0C1F2D background, and a color-coded 1px left-border based on the category (Software = Purple, Hardware = Green).
- **Inputs:** Dark fields with a 1px border. Focus state triggers a full primary color glow and a small "floating" label in monospaced font.
- **Status Indicators:** Small pulsing circles (using Accent Green) to indicate "Available for Work" or "System Online" status.
- **Terminal List:** A specialized list component for "Experience" or "Education" that uses a vertical circuit trace line instead of a standard bullet point.