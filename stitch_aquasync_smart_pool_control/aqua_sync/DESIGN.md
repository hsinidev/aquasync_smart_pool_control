---
name: Aqua-Sync
colors:
  surface: '#f9f9ff'
  surface-dim: '#d7dae4'
  surface-bright: '#f9f9ff'
  surface-container-lowest: '#ffffff'
  surface-container-low: '#f1f3fe'
  surface-container: '#ebedf8'
  surface-container-high: '#e6e8f3'
  surface-container-highest: '#e0e2ed'
  on-surface: '#181c23'
  on-surface-variant: '#414754'
  inverse-surface: '#2d3039'
  inverse-on-surface: '#eef0fb'
  outline: '#717786'
  outline-variant: '#c1c6d7'
  surface-tint: '#005cbc'
  primary: '#005ab7'
  on-primary: '#ffffff'
  primary-container: '#0072e5'
  on-primary-container: '#fefcff'
  inverse-primary: '#abc7ff'
  secondary: '#645e49'
  on-secondary: '#ffffff'
  secondary-container: '#e8dfc5'
  on-secondary-container: '#68634d'
  tertiary: '#9d3f00'
  on-tertiary: '#ffffff'
  tertiary-container: '#c45100'
  on-tertiary-container: '#fffbff'
  error: '#ba1a1a'
  on-error: '#ffffff'
  error-container: '#ffdad6'
  on-error-container: '#93000a'
  primary-fixed: '#d7e2ff'
  primary-fixed-dim: '#abc7ff'
  on-primary-fixed: '#001b3f'
  on-primary-fixed-variant: '#004590'
  secondary-fixed: '#ebe2c8'
  secondary-fixed-dim: '#cec6ad'
  on-secondary-fixed: '#1f1c0b'
  on-secondary-fixed-variant: '#4c4733'
  tertiary-fixed: '#ffdbcc'
  tertiary-fixed-dim: '#ffb693'
  on-tertiary-fixed: '#351000'
  on-tertiary-fixed-variant: '#7a2f00'
  background: '#f9f9ff'
  on-background: '#181c23'
  surface-variant: '#e0e2ed'
typography:
  display-lg:
    fontFamily: Manrope
    fontSize: 48px
    fontWeight: '700'
    lineHeight: 56px
    letterSpacing: -0.02em
  headline-lg:
    fontFamily: Manrope
    fontSize: 32px
    fontWeight: '600'
    lineHeight: 40px
    letterSpacing: -0.01em
  headline-md:
    fontFamily: Manrope
    fontSize: 24px
    fontWeight: '600'
    lineHeight: 32px
  body-lg:
    fontFamily: Manrope
    fontSize: 18px
    fontWeight: '400'
    lineHeight: 28px
  body-md:
    fontFamily: Manrope
    fontSize: 16px
    fontWeight: '400'
    lineHeight: 24px
  label-caps:
    fontFamily: Manrope
    fontSize: 12px
    fontWeight: '700'
    lineHeight: 16px
    letterSpacing: 0.05em
  stat-value:
    fontFamily: Manrope
    fontSize: 40px
    fontWeight: '300'
    lineHeight: 48px
rounded:
  sm: 0.25rem
  DEFAULT: 0.5rem
  md: 0.75rem
  lg: 1rem
  xl: 1.5rem
  full: 9999px
spacing:
  base: 8px
  xs: 4px
  sm: 12px
  md: 24px
  lg: 48px
  xl: 80px
  gutter: 20px
  margin-mobile: 16px
  margin-desktop: 40px
---

## Brand & Style

The design system is defined by a **Fluid-Modern** aesthetic, capturing the refreshing and serene essence of water management. It prioritizes a high-end, sanctuary-like experience for pool and spa owners, moving away from industrial utility toward lifestyle wellness. 

The style is a sophisticated blend of **Minimalism** and **Glassmorphism**. It utilizes expansive white space to evoke cleanliness, while translucent "glass" layers suggest the depth and clarity of water. Interaction design focuses on organic movement, featuring soft transitions and "liquid" feedback to create an atmosphere of effortless control and luxury.

## Colors

This design system utilizes a high-clarity palette to mirror a sunlit aquatic environment. 

- **Azure Blue (Primary):** A vibrant, deep sky blue used for primary actions, active states, and critical water metrics.
- **Crisp White (Surface/Background):** Pure white serves as the foundation, ensuring the UI feels airy and hygienic.
- **Sand (Secondary/Accent):** A warm, neutral tone used sparingly for secondary buttons, subtle dividers, and high-end tactile details to balance the coolness of the blue.
- **Water Tints:** Soft gradients moving from Azure to a pale cyan are used for data visualizations and glassmorphic backgrounds.

## Typography

The typography strategy employs **Manrope** for its geometric yet organic structure, bridging the gap between technical precision and human friendliness. 

The scale is intentionally airy. Headlines use tighter tracking and heavier weights to anchor the page, while body copy remains spacious to ensure legibility even in bright, outdoor poolside environments. A specific "stat-value" style is utilized for temperature and chemical levels, using a lighter weight to emphasize the "fluid" and modern feel of the data.

## Layout & Spacing

The layout follows a **Fluid Grid** model, ensuring the management dashboard scales gracefully from mobile handsets to wall-mounted tablets. 

A 12-column system is used for desktop, while a 4-column system is used for mobile. The rhythm is dictated by an 8px base unit. Generous external margins (40px on desktop) create a "frame" effect that makes the central content feel like a curated view. Internal component spacing (padding) is intentionally large to prevent the UI from feeling cramped or overly "utility-heavy."

## Elevation & Depth

Hierarchy is established through **Glassmorphism** and **Ambient Shadows**. 

- **Level 0 (Canvas):** Crisp white background.
- **Level 1 (Cards):** Subtle 1px Azure-tinted borders with a very soft, diffused shadow (15% opacity Azure) to give the impression of floating on water.
- **Level 2 (Modals/Overlays):** High-blur backdrop filters (20px - 30px) with a semi-transparent white fill (70% opacity). This creates a frosted glass effect that maintains the color context of the layers beneath.
- **Depth Cues:** Interactive elements should appear to "sink" slightly when pressed, using a transition from an ambient shadow to a subtle inner glow.

## Shapes

The shape language is consistently **Rounded**, avoiding sharp corners to maintain the fluid and safe brand personality. 

Standard components utilize a 0.5rem radius, while larger containers like cards and featured dashboard modules use the `rounded-xl` (1.5rem) setting. Interactive elements like sliders and status pills use a full "pill" radius (3rem) to evoke the smoothness of polished river stones.

## Components

### Buttons & Inputs
- **Primary Buttons:** Solid Azure Blue with rounded-pill shapes. Hover states trigger a subtle "ripple" expansion effect.
- **Secondary Buttons:** Sand-colored surfaces with Azure text, emphasizing a tactile, organic feel.
- **Input Fields:** Soft-grey borders that glow Azure when focused. Backgrounds are slightly off-white to distinguish from the primary canvas.

### Fluid Controls
- **Interactive Sliders:** Used for temperature and lighting. The "thumb" of the slider is a large, easy-to-target circle that grows slightly when touched. The track should fill with a gradient representing the intensity.
- **Ripple Effects:** Any touch or click event should trigger a subtle, radial "water ripple" animation originating from the point of contact.

### Indicators & Status
- **Status Indicators:** Small, glowing "pulses" indicate active systems (e.g., filtration, heating). 
- **Glass Cards:** Data summaries (pH levels, Chlorine) are housed in glassmorphic cards with high-contrast Azure typography for the primary metrics.

### Specialized Components
- **Water Level Graphic:** A container with a dynamic, animated wave line to visually represent the current pool/spa water level.
- **Status Rings:** Circular progress indicators used for chemical balances, utilizing soft gradients rather than solid color blocks.