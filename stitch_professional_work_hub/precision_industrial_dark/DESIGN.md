---
name: Precision Industrial Dark
colors:
  surface: '#0e1416'
  surface-dim: '#0e1416'
  surface-bright: '#343a3c'
  surface-container-lowest: '#090f11'
  surface-container-low: '#171d1e'
  surface-container: '#1b2122'
  surface-container-high: '#252b2d'
  surface-container-highest: '#303638'
  on-surface: '#dee3e6'
  on-surface-variant: '#bcc9cd'
  inverse-surface: '#dee3e6'
  inverse-on-surface: '#2b3133'
  outline: '#869397'
  outline-variant: '#3d494c'
  surface-tint: '#4cd7f6'
  primary: '#4cd7f6'
  on-primary: '#003640'
  primary-container: '#06b6d4'
  on-primary-container: '#00424f'
  inverse-primary: '#00687a'
  secondary: '#bec6e0'
  on-secondary: '#283044'
  secondary-container: '#3f465c'
  on-secondary-container: '#adb4ce'
  tertiary: '#bcc7de'
  on-tertiary: '#263143'
  tertiary-container: '#9ca7be'
  on-tertiary-container: '#313c4f'
  error: '#ffb4ab'
  on-error: '#690005'
  error-container: '#93000a'
  on-error-container: '#ffdad6'
  primary-fixed: '#acedff'
  primary-fixed-dim: '#4cd7f6'
  on-primary-fixed: '#001f26'
  on-primary-fixed-variant: '#004e5c'
  secondary-fixed: '#dae2fd'
  secondary-fixed-dim: '#bec6e0'
  on-secondary-fixed: '#131b2e'
  on-secondary-fixed-variant: '#3f465c'
  tertiary-fixed: '#d8e3fb'
  tertiary-fixed-dim: '#bcc7de'
  on-tertiary-fixed: '#111c2d'
  on-tertiary-fixed-variant: '#3c475a'
  background: '#0e1416'
  on-background: '#dee3e6'
  surface-variant: '#303638'
  status-online: '#10b981'
  status-offline: '#ef4444'
  status-warning: '#f59e0b'
  status-info: '#3b82f6'
  background-deep: '#020617'
  border-subtle: '#334155'
typography:
  display-lg:
    fontFamily: Inter
    fontSize: 32px
    fontWeight: '700'
    lineHeight: 40px
    letterSpacing: -0.02em
  headline-md:
    fontFamily: Inter
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  headline-sm:
    fontFamily: Inter
    fontSize: 18px
    fontWeight: '600'
    lineHeight: 24px
  body-lg:
    fontFamily: Inter
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  body-md:
    fontFamily: Inter
    fontSize: 14px
    fontWeight: '400'
    lineHeight: 20px
  body-sm:
    fontFamily: Inter
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 16px
  label-caps:
    fontFamily: Inter
    fontSize: 11px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  data-mono:
    fontFamily: JetBrains Mono
    fontSize: 13px
    fontWeight: '400'
    lineHeight: 18px
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  container-margin: 1.5rem
  gutter: 1rem
  widget-padding: 1.25rem
  row-height-dense: 2.5rem
  row-height-standard: 3.5rem
---

## Brand & Style

The design system is engineered for mission-critical infrastructure management. It balances industrial-grade reliability with a high-tech, modern aesthetic. The visual narrative focuses on "Management by Exception," where the interface remains quiet and sophisticated until human intervention is required.

The style is **Corporate Modern with Glassmorphic accents**. It utilizes a deep, layered dark theme to reduce eye strain during long monitoring shifts, while employing vibrant cyan accents to guide the eye toward primary actions. High-density data is managed through crisp borders and subtle translucent layers, creating a UI that feels precise, authoritative, and futuristic.

## Colors

The palette is anchored by `background-deep` for the base canvas, with `secondary_color_hex` and `tertiary_color_hex` used to define surface hierarchies and container levels. 

The primary brand color, a vibrant Cyan (#06b6d4), is reserved exclusively for interactive elements, progress indicators, and active states. Semantic colors follow industry standards for immediate recognition:
- **Online/Success:** Emerald green for operational health.
- **Offline/Critical:** Bright red for immediate system failures.
- **Warning/High Priority:** Amber for maintenance requirements and alerts.
- **In-Progress/Neutral:** Azure blue for active workflows.

## Typography

This design system uses **Inter** for all UI and prose elements due to its exceptional legibility in low-light environments. For technical data—such as IP addresses, asset codes, and sensor readings—**JetBrains Mono** is utilized to ensure character distinction and vertical alignment in dense tables.

**Hierarchy Rules:**
- **Headlines:** Use Bold or Semi-Bold weights to anchor page sections.
- **Data Grids:** Use `body-sm` for standard rows to maximize information density.
- **Monospaced Data:** Reserved for machine-readable strings and technical logs.
- **Labels:** Use uppercase for table headers and form category labels to create clear structural separation.

## Layout & Spacing

The layout utilizes a **fixed sidebar** for primary navigation (240px width) with a **fluid content area** for dashboards and tables. 

**Grid & Alignment:**
- Use a 12-column grid for dashboard widgets.
- Widgets should span 3, 4, 6, or 12 columns depending on data complexity.
- Horizontal alignment is prioritized in tables to allow for rapid scanning of status columns.

**Responsive Behavior:**
- **Desktop:** Full 12-column visibility.
- **Tablet:** 8-column grid; sidebar collapses to an icon-only rail.
- **Mobile:** Single column flow; charts simplify to key metrics; horizontal scrolling enabled for technical tables.

## Elevation & Depth

Visual hierarchy is achieved through **Tonal Layering** combined with **subtle Glassmorphism**.

- **Level 0 (Base):** Deepest charcoal background.
- **Level 1 (Card/Widget):** Raised surface with a 1px border (`#334155`). Use a subtle backdrop blur (8px) and 5% white opacity to create a "glass" effect on top of background gradients.
- **Level 2 (Modals/Popovers):** Higher contrast surfaces with a soft, tinted shadow (Blur: 24px, Spread: -4px, Color: `rgba(0, 0, 0, 0.5)`).
- **Interactive States:** Buttons and active navigation items use a soft glow (box-shadow with primary cyan at 20% opacity) rather than heavy physical elevation.

## Shapes

The shape language is **Soft (0.25rem / 4px)**. This maintains a professional, engineered feel that avoids the "playfulness" of highly rounded corners while appearing more modern than sharp edges.

- **Standard Buttons & Inputs:** 4px radius.
- **Dashboard Cards:** 8px (Large) radius for better container definition.
- **Status Pills:** 100px (Full Pill) to distinguish them from interactive buttons.
- **Progress Bars:** Flat or slightly rounded (2px) to emphasize the linear, technical nature of the data.

## Components

**Buttons:**
- **Primary:** Solid Cyan background with dark navy text. No shadow in rest state; subtle cyan glow on hover.
- **Secondary:** Ghost style with a 1px border of `border-subtle`.
- **Destructive:** Solid or outlined Red, reserved for "Hapus" or "Batal" in high-risk contexts.

**Data Tables:**
- Alternate row striping is not used; instead, use 1px horizontal dividers.
- Row hover states must change the background to `tertiary_color_hex` for focus.
- Status indicators must be a colored dot paired with a text label for accessibility.

**Input Fields:**
- Darker than the card surface with a 1px `border-subtle`.
- Focus state uses a 1px Cyan border and a tiny inner glow.

**Charts:**
- Use high-contrast stroke colors for line charts.
- Donut charts for equipment status should use the semantic green/amber/red palette.
- Tooltips should be glassmorphic with high-contrast mono typography.

**Status Chips:**
- High-contrast text on a low-opacity background of the same semantic color (e.g., Red text on 10% Red background).