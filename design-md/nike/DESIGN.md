---
version: "alpha"
name: "Nike Design System"
colors:
  primary: "#111111"
  on-primary: "#FFFFFF"
  primary-hover: "#333333"
  background: "#FFFFFF"
  foreground: "#111111"
  surface: "#F5F5F5"
  on-surface: "#111111"
  border: "#707072"
typography:
  heading:
    fontFamily: "sans-serif"
    fontSize: "76px"
    fontWeight: "500"
    lineHeight: "68.4px"
    letterSpacing: "0em"
  navigation:
    fontFamily: "sans-serif"
    fontSize: "32px"
    fontWeight: "500"
    lineHeight: "38px"
    letterSpacing: "0em"
  body:
    fontFamily: "sans-serif"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
    letterSpacing: "0em"
rounded:
  sm: "30px"
  md: "24px"
  circle: "50%"
spacing:
  hairline: "1px"
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  xxl: "64px"
  page-gutter: "96px"
components:
  page:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  header:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    padding: "{spacing.lg}"
  navigation:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    gap: "{spacing.xl}"
  search:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  icon-button:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    padding: "{spacing.md}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
  media-grid:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    gap: "{spacing.lg}"
    padding: "{spacing.page-gutter}"
  media-card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
  border:
    backgroundColor: "{colors.border}"
    height: "{spacing.hairline}"
  floating-control:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.circle}"

---

## Overview

This design system describes a spacious commerce-style interface built around a white navigation header, restrained monochrome controls, and a large three-column media grid. The visual hierarchy relies on generous gutters, strong image presentation, bold navigation, and minimal ornamentation.

## Colors

- **Primary:** Near-black emphasis color for high-priority actions.
- **On Primary:** White content placed on primary controls.
- **Primary Hover:** Slightly lighter near-black interaction state.
- **Background:** White page canvas and header background.
- **Foreground:** Near-black navigation, icon, and text color.
- **Surface:** Light gray fill used for search controls, media areas, and floating controls.
- **On Surface:** Near-black content placed on light gray surfaces.
- **Border:** Mid-gray structural separator and outline color.

## Typography

Use a clean sans-serif family throughout. Navigation is large, bold, and horizontally centered. Body text uses a smaller regular weight with a compact, readable line height. Display headings use a large, tightly set treatment when present.

## Layout

Use a full-width white header with the primary navigation centered horizontally and utility controls grouped at the opposite side. Keep the header visually distinct from the content with its solid background.

Below the header, allow a wide visual band to span the viewport before the primary content begins. Present major media in three equal columns with consistent gaps and generous outer gutters. Preserve the large image-first composition and avoid dense text overlays.

## Elevation & Depth

The interface is predominantly flat. Use subtle soft shadows only for floating controls or elements that sit above the page, such as a persistent circular utility control. Avoid shadows on the primary media grid unless needed to communicate separation.

## Shapes

Use pill-shaped corners for search and primary controls. Keep media panels mostly rectangular and allow the imagery to provide visual emphasis. Use a circular shape for persistent floating controls. Avoid decorative corner treatments that compete with the large media panels.

## Components

- **header:** Full-width white navigation region using {colors.background}, {colors.foreground}, and {typography.navigation}.
- **navigation:** Centered horizontal navigation using {colors.background}, {colors.foreground}, and {typography.navigation}.
- **search:** Light gray rounded utility field using {colors.surface}, {colors.on-surface}, and {rounded.sm}.
- **icon-button:** Minimal utility control using {colors.background} and {colors.foreground}.
- **button-primary:** High-emphasis dark action using {colors.primary} with {colors.on-primary} text.
- **button-primary-hover:** Independent hover state using {colors.primary-hover} with {colors.on-primary} text.
- **media-grid:** Spacious multi-column content region using {colors.background} with {spacing.lg} gaps and {spacing.page-gutter} outer padding.
- **media-card:** Large image-led panel using {colors.surface} and {colors.foreground}.
- **border:** Thin structural separator using {colors.border} and {spacing.hairline}.
- **floating-control:** Circular persistent control using {colors.surface}, {colors.foreground}, and {rounded.circle}.

## Do's and Don'ts

### Do

- Use the white header and page canvas as the dominant visual foundation.
- Preserve generous horizontal gutters and consistent media-column spacing.
- Keep navigation prominent, bold, and centered.
- Use light gray surfaces for compact utility controls and image-panel backgrounds.
- Reference visual values through tokens such as {colors.primary} and {spacing.lg}.
- Maintain WCAG AA contrast for text and interactive controls.

### Don't

- Do not introduce saturated colors or heavy decorative effects.
- Do not make the media grid dense or narrow.
- Do not use rounded corners on every element.
- Do not hardcode captured colors inside component definitions.
- Do not nest hover, active, or pressed variants inside a base component.
- Do not add page-specific copy, branding, or imagery descriptions to reusable component rules.
