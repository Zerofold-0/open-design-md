---
version: "alpha"
name: "Spotify Design System"
omitted: []
colors:
  primary: "#1ED760"
  on-primary: "#000000"
  primary-hover: "#1ED760"
  background: "#121212"
  foreground: "#FFFFFF"
  surface: "#242424"
  on-surface: "#FFFFFF"
  border: "#727272"
  banner: "#1F73C9"
  on-banner: "#FFFFFF"
  muted: "#B3B3B3"
typography:
  heading:
    fontFamily: "sans-serif"
    fontSize: "128px"
    fontWeight: "900"
    lineHeight: "0.85"
    letterSpacing: "-0.04em"
  body:
    fontFamily: "sans-serif"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "1.5"
    letterSpacing: "0em"
  navigation:
    fontFamily: "sans-serif"
    fontSize: "16px"
    fontWeight: "700"
    lineHeight: "1.25"
    letterSpacing: "0em"
rounded:
  sm: "9999px"
  md: "24px"
  full: "50%"
spacing:
  hairline: "1px"
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
  announcement:
    backgroundColor: "{colors.banner}"
    textColor: "{colors.on-banner}"
    typography: "{typography.body}"
    padding: "{spacing.md}"
  header:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    padding: "{spacing.xl}"
  hero:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
    padding: "{spacing.xxl}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
  divider:
    backgroundColor: "{colors.border}"
    height: "{spacing.hairline}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.navigation}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
  button-secondary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
    borderColor: "{colors.border}"
    borderWidth: "{spacing.hairline}"
  media-frame:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.full}"
  media-control:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.full}"
  supporting-text:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.body}"
---

## Overview

This system captures a dark, high-contrast interface with a bright announcement strip, a spacious navigation header, oversized display typography, pill-shaped actions, and large rounded media treatments.

## Colors

- **Background:** Near-black page canvas and primary navigation surface.
- **Foreground:** White high-emphasis text and iconography.
- **Primary:** Bright green used for prominent actions.
- **On Primary:** Black text placed on bright green controls.
- **Banner:** Saturated blue used for the top announcement area.
- **Surface:** Dark gray used for raised controls and media-related surfaces.
- **Border:** Medium gray used for outlined controls and separators.
- **Muted:** Light gray used for supporting text.

## Typography

Use a heavy sans-serif display style for oversized hero headings. Display text is very large, tightly tracked, and closely stacked. Use a regular sans-serif style for supporting copy and a bold sans-serif style for navigation and actions.

## Layout

Use a full-width dark canvas with a compact announcement strip above the main header. Keep navigation content horizontally distributed with generous side padding. Place the hero content in a spacious composition with oversized text, prominent actions, and a large rounded media area. Use the spacing scale to maintain clear separation between navigation, hero text, controls, and supporting text.

## Elevation & Depth

Depth is communicated primarily through contrast between the near-black canvas and dark gray controls or media surfaces. Avoid prominent shadows. Use solid surface changes, outlined controls, and the circular media control to establish hierarchy.

## Shapes

Use fully rounded pill shapes for prominent actions and compact controls. Use a full circular shape for circular media controls and large media treatments. Use a medium radius for grouped surfaces. Keep separators and outlines crisp and minimal.

## Components

- **announcement:** Full-width blue strip with white content and compact vertical padding.
- **header:** Dark navigation bar with bold, high-contrast labels and generous horizontal spacing.
- **hero:** Oversized white display typography on the dark canvas.
- **button-primary:** Green pill-shaped action with black text.
- **button-primary-hover:** Separate hover entry retaining the green action treatment and black text.
- **button-secondary:** Dark outlined pill-shaped action with white text.
- **surface:** Dark gray grouped area with white content and medium rounding.
- **media-frame:** Large circular or rounded media treatment using the surface color.
- **media-control:** Circular dark control with white iconography.
- **divider:** Thin gray structural separator.
- **supporting-text:** Muted gray text for secondary information.

## Do's and Don'ts

### Do

- Use {colors.primary} sparingly for the highest-priority actions.
- Maintain strong white-on-dark and black-on-primary contrast.
- Keep primary and secondary actions pill-shaped and visually distinct.
- Use oversized display typography for the main visual statement.
- Preserve generous spacing around hero content and controls.
- Keep interaction states as separate flat component entries.

### Don't

- Do not introduce bright colors outside the blue announcement and green action treatments.
- Do not use rounded cards or shadows where a flat dark surface is sufficient.
- Do not use low-contrast text on the dark canvas.
- Do not replace the strong display hierarchy with small, tightly packed headings.
- Do not nest hover or other interaction states under a base component.
