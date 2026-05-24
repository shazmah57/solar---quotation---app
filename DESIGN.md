---
name: Solar Utility System
colors:
  surface: '#f8f9ff'
  surface-dim: '#cbdbf5'
  surface-bright: '#f8f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#eff4ff'
  surface-container: '#e5eeff'
  surface-container-high: '#dce9ff'
  surface-container-highest: '#d3e4fe'
  on-surface: '#0b1c30'
  on-surface-variant: '#45464d'
  inverse-surface: '#213145'
  inverse-on-surface: '#eaf1ff'
  outline: '#76777d'
  outline-variant: '#c6c6cd'
  surface-tint: '#565e74'
  primary: '#000000'
  on-primary: '#ffffff'
  primary-container: '#131b2e'
  on-primary-container: '#7c839b'
  inverse-primary: '#bec6e0'
  secondary: '#855300'
  on-secondary: '#ffffff'
  secondary-container: '#fea619'
  on-secondary-container: '#684000'
  tertiary: '#000000'
  on-tertiary: '#ffffff'
  tertiary-container: '#002113'
  on-tertiary-container: '#009668'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#dae2fd'
  primary-fixed-dim: '#bec6e0'
  on-primary-fixed: '#131b2e'
  on-primary-fixed-variant: '#3f465c'
  secondary-fixed: '#ffddb8'
  secondary-fixed-dim: '#ffb95f'
  on-secondary-fixed: '#2a1700'
  on-secondary-fixed-variant: '#653e00'
  tertiary-fixed: '#6ffbbe'
  tertiary-fixed-dim: '#4edea3'
  on-tertiary-fixed: '#002113'
  on-tertiary-fixed-variant: '#005236'
  background: '#f8f9ff'
  on-background: '#0b1c30'
  surface-variant: '#d3e4fe'
typography:
  headline-xl:
    fontFamily: Hanken Grotesk
    fontSize: 40px
    fontWeight: '700'
    lineHeight: '1.2'
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Hanken Grotesk
    fontSize: 32px
    fontWeight: '600'
    lineHeight: '1.2'
  headline-lg-mobile:
    fontFamily: Hanken Grotesk
    fontSize: 24px
    fontWeight: '600'
    lineHeight: '1.3'
  body-lg:
    fontFamily: Work Sans
    fontSize: 18px
    fontWeight: '400'
    lineHeight: '1.6'
  body-md:
    fontFamily: Work Sans
    fontSize: 16px
    fontWeight: '400'
    lineHeight: '1.5'
  label-md:
    fontFamily: Hanken Grotesk
    fontSize: 14px
    fontWeight: '600'
    lineHeight: '1.2'
    letterSpacing: 0.05em
  data-display:
    fontFamily: Geist
    fontSize: 24px
    fontWeight: '500'
    lineHeight: '1.2'
rounded:
  sm: 0.125rem
  DEFAULT: 0.25rem
  md: 0.375rem
  lg: 0.5rem
  xl: 0.75rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 80px
  gutter: 24px
  margin-mobile: 16px
  margin-desktop: 64px
---

## Brand & Style
The design system is engineered for high-utility professional environments, specifically tailored for Sustainable Solar Energy Solutions. The brand personality is rooted in **Reliability, Precision, and Optimism**. It avoids the flighty nature of consumer startups in favor of a "Utility-Grade" aesthetic that inspires confidence in high-stakes financial and environmental calculations.

The visual style is **Corporate Modern**, characterized by a rigorous grid, generous whitespace to reduce cognitive load during complex sales tasks, and a color palette that mirrors the transition from deep sky to direct sunlight. The UI must remain legible in high-glare environments, such as field agents working outdoors, necessitating high-contrast ratios and substantial touch targets.

## Colors
The palette is dominated by **Midnight Navy** (#0F172A), representing stability and the vast potential of the sky. This is punctuated by **Solar Amber** (#F59E0B), used sparingly for primary actions and highlights to draw the eye to "energy-producing" elements.

**Emerald Green** (#10B981) serves as a tertiary color, specifically reserved for sustainability metrics, savings indicators, and positive ROI calculations. The neutral scale uses cool grays to maintain a technical, clean feeling, ensuring that white surfaces feel "bleached" and modern rather than muddy.

## Typography
Legibility is the primary metric for this design system. **Hanken Grotesk** provides a sharp, contemporary edge for headlines and labels, ensuring the brand feels "engineered." **Work Sans** is utilized for all body copy and form inputs due to its exceptional performance at various weights and its grounded, neutral character.

For numerical calculations, ROI tables, and energy output data, we employ **Geist**—a technical monospaced/sans hybrid that ensures numbers align vertically for easy comparison during sales presentations.

## Layout & Spacing
The system utilizes an **8px linear scale** to ensure mathematical harmony across all components. For internal sales tools, density is balanced against touch-friendliness. 

On **Mobile (Field Agent View)**, we use a single-column fluid layout with a 16px side margin. Touch targets for form inputs must be a minimum of 48px in height. 
On **Desktop (Office View)**, we utilize a 12-column fixed grid with a 1200px max-width, allowing for multi-pane layouts where calculation parameters sit adjacent to visual charts.

## Elevation & Depth
The design system employs **Tonal Layering** supplemented by **Ambient Shadows** to define hierarchy. 

- **Level 0 (Canvas):** The base background (#FFFFFF).
- **Level 1 (Cards/Panels):** Uses a subtle background tint (#F8FAFC) or a 1px border (#E2E8F0) to define areas without creating visual noise.
- **Level 2 (Modals/Dropdowns):** Elevated using a "Soft Solar" shadow—low opacity Midnight Navy with a large blur radius (e.g., `0px 10px 30px rgba(15, 23, 42, 0.08)`) to suggest a floating state.

We avoid heavy gradients and skeuomorphism, opting for "flat-plus" depth where interaction is signaled by slight shifts in saturation.

## Shapes
A **Soft** shape language is used to balance the clinical nature of energy data with human accessibility. Standard components use a `0.25rem` (4px) radius. Larger containers like calculation cards or modular panels use a `0.5rem` (8px) radius. This subtle rounding prevents the UI from feeling aggressive while maintaining the professional structure required for an enterprise tool.

## Components

### Buttons & Inputs
- **Primary Action:** Solid Midnight Navy with white text. High contrast for outdoor visibility.
- **Solar Action:** Solid Solar Amber for "Generate Quote" or "Finalize Contract" actions.
- **Inputs:** 1px bordered boxes using Work Sans. Labels are always persistent (not floating) to ensure field agents don't lose context during data entry. 

### Calculation Displays
Numerical readouts for "Total Savings" or "System Output" should be framed in a Level 1 surface with a left-accent border in Emerald Green or Solar Amber. These cards use **Geist** for the numerical value to emphasize technical accuracy.

### Dropdowns
Dropdown menus must be full-width on mobile devices for ease of thumb interaction. On desktop, they include search-filtering as standard to handle large equipment catalogs.

### Data Visualization
Charts should use a "Sun-Path" color logic: Amber for solar gain, Navy for consumption, and Green for net-zero offset. Lines should be a minimum of 2px thick to remain legible on mobile screens.