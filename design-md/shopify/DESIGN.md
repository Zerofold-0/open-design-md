---
version: "alpha"
name: "Shopify Design System"
colors:
  primary: "#FFFFFF"
  on-primary: "#000000"
  primary-hover: "#F5F5F5"
  background: "#02090A"
  foreground: "#FFFFFF"
  surface: "#041E18"
  on-surface: "#FFFFFF"
  border: "#E5E7EB"
  overlay: "#000000"
typography:
  heading:
    fontFamily: "Inter"
    fontSize: "96px"
    fontWeight: "300"
    lineHeight: "103.68px"
    letterSpacing: "-1.92px"
  body:
    fontFamily: "Inter"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
rounded:
  sm: "8px"
  md: "16px"
  lg: "9999px"
  xl: "48px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  xxl: "48px"
components:
  page:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  hero-media:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.foreground}"
  hero-heading:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  hero-body:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  navigation:
    backgroundColor: "{colors.overlay}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.xl}"
  border:
    backgroundColor: "{colors.border}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.lg}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
  button-secondary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.border}"
    typography: "{typography.body}"
    rounded: "{rounded.lg}"
    padding: "{spacing.md}"
  button-secondary-hover:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    borderColor: "{colors.border}"
  heading:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
---

## Overview

This design system describes a full-bleed, image-led interface with a darkened media layer, high-contrast light typography, a compact top navigation, and prominent pill-shaped actions. Content is anchored within the hero while remaining responsive and spacious.

## Colors

- **Primary:** White high-emphasis action color.
- **On Primary:** Black text used on primary actions.
- **Primary Hover:** Slightly softened white for primary interaction states.
- **Background:** Near-black page canvas and dark secondary-control background.
- **Foreground:** White text and high-emphasis interface content.
- **Surface:** Deep green-black color for grouped or raised content.
- **On Surface:** White content placed on surfaces.
- **Border:** Light neutral outline for secondary controls and structural separation.
- **Overlay:** Black media treatment used to improve text legibility over imagery.

## Typography

Use **Inter** throughout the interface. Large display text is thin, tightly tracked, and set at approximately 96px with a 103.68px line height. Supporting copy and navigation use a 16px regular style with a 24px line height.

## Layout

Use a full-viewport media region as the primary visual field, with a dark overlay supporting legibility. Place navigation along the top edge and align hero content toward the lower-left with generous outer margins. Keep supporting text above a horizontal action group, allowing the group to wrap on narrow screens. Use the spacing scale to maintain consistent gaps between navigation items, text blocks, and controls.

## Elevation & Depth

Depth is created primarily through the contrast between the dark overlay, bright foreground content, and underlying media rather than through visible shadows. Use dark surfaces and subtle outlines to distinguish grouped content and secondary controls without adding heavy elevation.

## Shapes

Use fully rounded pill shapes for primary and secondary actions, compact circular controls, and other prominent interactive elements. Use a large radius for broad grouped surfaces and medium radii only where a softer rectangular grouping is needed. Keep outlines light and clearly visible against dark backgrounds.

## Components

- **page:** Near-black responsive canvas with white body content.
- **hero-media:** Full-bleed visual region with a black readability overlay.
- **hero-heading:** Large, thin white display text over the media treatment.
- **hero-body:** White supporting copy positioned beneath the hero heading.
- **navigation:** Compact top-level navigation with white text over the media treatment.
- **surface:** Deep green-black grouped content region with a large rounded shape.
- **border:** Light neutral structural separator or outline.
- **button-primary:** White pill-shaped action with black text.
- **button-primary-hover:** Softened-white pill-shaped action with black text.
- **button-secondary:** Dark outlined pill-shaped action with white text.
- **button-secondary-hover:** Deep green-black outlined action with white text.

## Do's and Don'ts

### Do

- Use the media overlay to preserve readable white content over varied imagery.
- Keep primary actions visually dominant through white fill and pill geometry.
- Use outlined dark controls for secondary actions.
- Preserve the thin, oversized display hierarchy and generous hero spacing.
- Reference design values through tokens such as {colors.primary} and {spacing.md}.
- Maintain WCAG AA contrast for text and interactive controls.

### Don't

- Do not hardcode captured colors inside component definitions.
- Do not use heavy shadows when contrast and overlay provide sufficient depth.
- Do not replace pill-shaped actions with sharp rectangular controls.
- Do not nest hover or other interaction variants inside a base component.
- Do not introduce source-specific copy, imagery, branding, or page content into reusable patterns.
