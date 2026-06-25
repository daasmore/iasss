---
name: Precision Industrial Interface
colors:
  surface: '#121415'
  surface-dim: '#121415'
  surface-bright: '#38393a'
  surface-container-lowest: '#0c0e0f'
  surface-container-low: '#1a1c1d'
  surface-container: '#1e2021'
  surface-container-high: '#282a2b'
  surface-container-highest: '#333536'
  on-surface: '#e2e2e3'
  on-surface-variant: '#b9cacb'
  inverse-surface: '#e2e2e3'
  inverse-on-surface: '#2f3132'
  outline: '#849495'
  outline-variant: '#3a494b'
  surface-tint: '#00dbe7'
  primary: '#e1fdff'
  on-primary: '#00363a'
  primary-container: '#00f2ff'
  on-primary-container: '#006a71'
  inverse-primary: '#00696f'
  secondary: '#ffdb9d'
  on-secondary: '#412d00'
  secondary-container: '#feb700'
  on-secondary-container: '#6b4b00'
  tertiary: '#fff5f4'
  on-tertiary: '#680008'
  tertiary-container: '#ffd0cb'
  on-tertiary-container: '#c2031a'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#74f5ff'
  primary-fixed-dim: '#00dbe7'
  on-primary-fixed: '#002022'
  on-primary-fixed-variant: '#004f54'
  secondary-fixed: '#ffdea8'
  secondary-fixed-dim: '#ffba20'
  on-secondary-fixed: '#271900'
  on-secondary-fixed-variant: '#5e4200'
  tertiary-fixed: '#ffdad6'
  tertiary-fixed-dim: '#ffb3ad'
  on-tertiary-fixed: '#410003'
  on-tertiary-fixed-variant: '#930010'
  background: '#121415'
  on-background: '#e2e2e3'
  surface-variant: '#333536'
typography:
  display-tech:
    fontFamily: JetBrains Mono
    fontSize: 24px
    fontWeight: '700'
    lineHeight: 32px
    letterSpacing: -0.02em
  headline-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '500'
    lineHeight: 16px
  label-xs:
    fontFamily: JetBrains Mono
    fontSize: 10px
    fontWeight: '700'
    lineHeight: 12px
    letterSpacing: 0.1em
  data-mono-mobile:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '500'
    lineHeight: 14px
spacing:
  unit: 4px
  gutter: 12px
  module-padding: 16px
  grid-overlay-size: 32px
---

## Brand & Style
The design system is built upon the "Precision Engineering" narrative, transforming the IAS Maintenance platform into a high-stakes mission control environment. The aesthetic prioritizes density and technical utility over consumer-grade simplicity, targeting professional engineers and operators who require immediate access to complex data.

The style is a hybrid of **Industrial Tech** and **Technical Brutalism**. It utilizes micro-borders, atmospheric glassmorphism, and subtle scanline textures to evoke the feeling of high-end hardware interfaces. Visual hierarchy is established through "active" glowing indicators and razor-sharp structural alignments rather than traditional elevation.

## Colors
The palette is rooted in an obsidian-dark environment to minimize eye strain in control-room settings. 

- **Base Colors:** Obsidian (#0f1214) for the main canvas and Deep Charcoal (#0a0c0d) for inset modular panels.
- **Accents:** Neon Cyan serves as the primary action and "online" state color. Amber is reserved for warnings and secondary data highlights.
- **Status:** A critical Red (#ff3e3e) is used sparingly for hardware alerts and system failures.
- **Grids:** All structural lines use a low-opacity white (8-12%) to maintain a technical "schematic" feel without distracting from content.

## Typography
This design system employs a dual-font strategy to differentiate between interface navigation and technical data.

- **Inter:** Used for UI labels, titles, and descriptive text to ensure readability and a modern professional tone.
- **JetBrains Mono:** Used for all telemetry, timestamps, hardware IDs, and status readouts. It reinforces the "engineered" aesthetic and ensures numerical alignment in data tables.
- **Styling:** Headings and labels frequently use uppercase with increased letter spacing to mimic industrial equipment labeling.

## Layout & Spacing
The layout follows a high-density, fixed-grid philosophy. The screen is treated as a "Dashboard Console" where whitespace is filled with technical metadata (coordinates, versioning, system uptime) rather than being left empty.

- **Modular Layout:** Content is housed in discrete "Modules" that align to a 12-column grid.
- **Tight Gutters:** 12px gutters create a sense of compact, efficient machinery.
- **Grid Overlay:** A subtle, non-functional 32px background grid is visible in the negative space to reinforce the engineering theme.
- **Dividers:** Use 1px solid lines rather than margins to separate logical groups, maximizing screen real estate for data.

## Elevation & Depth
Traditional drop shadows are strictly prohibited. Depth is achieved through layering and luminosity:

- **Glassmorphism:** Use low-opacity fills (4-6% white) with a 10px backdrop blur for modal overlays or floating tooltips.
- **Z-Axis Layers:** "Inner" modules use a slightly darker background (#0a0c0d) than the main canvas to appear recessed.
- **Luminous Glow:** Active elements (selected tabs, running motors) use a soft outer glow (0px 0px 8px) in the primary accent color (#00f2ff) to simulate hardware LEDs.
- **Micro-Borders:** Every module has a 1px border. Default state is low-opacity; active/hover state is high-opacity Cyan.

## Shapes
The design system utilizes a sharp-edge aesthetic to reflect precision and structural integrity. 

- **Radius:** A strict 0px radius is preferred for all modules and major buttons.
- **Micro-Chamfer:** For small interactive components like chips or checkboxes, a maximum radius of 2px may be applied only if necessary for optical balance.
- **Technical Accents:** Use 45-degree angled corners (clipped corners) on decorative module headers to enhance the military/industrial hardware look.

## Components

### Buttons & Controls
- **Action Buttons:** Sharp corners, 1px border, transparent background. On hover, fill with 10% Cyan and apply a 4px Cyan outer glow.
- **Toggle Switches:** Designed as small horizontal sliders that look like physical hardware toggles. Use Neon Cyan for the "ON" position.

### Data Modules (Cards)
- **Structure:** Modules consist of a header bar with a "Technical ID" in the top left (e.g., MOD-082) and the title.
- **Background:** Solid obsidian with a subtle scanline texture (horizontal 1px lines at 2% opacity).

### Status Indicators
- **LEDs:** Small square indicators. Static Gray = Off; Pulsing Cyan = Active; Solid Amber = Standby; Blinking Red = Critical.

### Form Inputs
- **Fields:** Bottom-border only or full 1px border. Use JetBrains Mono for input text. Label text should be placed outside the box in `label-xs` style.

### Lists & Tables
- **Grid Lines:** Vertical and horizontal 1px lines for every cell. High-density padding (8px top/bottom).
- **Row Hover:** Highlight the entire row with a 5% white tint and a left-aligned 2px Cyan "active indicator" strip.