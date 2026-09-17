---
version: "alpha"
name: "Cursor Design System"
colors:
  primary: "#26251E"
  on-primary: "#FFFFFF"
  primary-hover: "#26251E"
  background: "#F7F7F4"
  foreground: "#000000"
  surface: "#F2F1ED"
  on-surface: "#000000"
  border: "#D8D7D2"
typography:
  heading:
    fontFamily: "sans-serif"
    fontSize: "48px"
    fontWeight: "400"
    lineHeight: "56px"
    letterSpacing: "-0.5px"
  body:
    fontFamily: "sans-serif"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
    letterSpacing: "0px"
  navigation:
    fontFamily: "sans-serif"
    fontSize: "20px"
    fontWeight: "400"
    lineHeight: "28px"
    letterSpacing: "-0.1px"
rounded:
  sm: "4px"
  md: "8px"
  lg: "24px"
  pill: "9999px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  xxl: "48px"
  section: "64px"
  gutter: "6.5vw"
  hairline: "1px"
components:
  page:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  header:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    padding: "{spacing.md} {spacing.gutter}"
  navigation:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
  hero:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
    padding: "{spacing.xl} {spacing.gutter} {spacing.section}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
  media-frame:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.sm}"
  border:
    backgroundColor: "{colors.border}"
    height: "{spacing.hairline}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "{spacing.md} {spacing.lg}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.pill}"
  button-secondary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "{spacing.md} {spacing.lg}"
  heading:
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  floating-control:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.pill}"
---

## Overview

This design system describes a restrained light interface with a warm off-white canvas, near-black typography, generous horizontal gutters, large open spacing, and pill-shaped actions. Content is organized into a simple header, spacious introductory area, and large rounded media surfaces.

## Colors

- **Primary:** Near-black emphasis color for prominent actions.
- **On Primary:** White content color used on primary actions.
- **Primary Hover:** Primary action state color.
- **Background:** Warm off-white page canvas.
- **Foreground:** Black high-emphasis text.
- **Surface:** Slightly darker warm neutral for secondary controls and grouped areas.
- **On Surface:** Black content color used on surfaces.
- **Border:** Light neutral separator and outline color.

Keep the palette quiet and neutral. Use the primary color sparingly for the strongest action emphasis, while surfaces provide subtle separation without introducing strong contrast between adjacent regions.

## Typography

Use a clean sans-serif family throughout the interface. Large headings are regular-weight, tightly tracked, and set with generous line height across multiple lines. Body and navigation text use a regular weight with a comfortable reading line height. Avoid decorative, condensed, or heavy type treatments in the surrounding interface.

## Layout

Use a wide, centered content region with consistent viewport-relative horizontal gutters. The header aligns its mark, navigation, and actions to the same content edges as the main content.

Place the introductory heading toward the upper left with substantial whitespace around it. Keep primary and secondary actions in a horizontal row with a moderate gap. Separate the introductory area from the large media surface with generous vertical spacing.

Large visual content should use broad rectangular proportions, rounded corners, and responsive width rather than fixed page-specific dimensions. Preserve the open composition and avoid dense card grids or narrow text columns.

## Elevation & Depth

Use restrained depth. Large visual surfaces may use a soft, diffuse shadow and a subtle outline to distinguish them from the page canvas. Floating controls can use a small neutral outline and light shadow. Avoid strong shadows, glossy effects, or layered elevation when flat spacing and tonal contrast provide sufficient hierarchy.

## Shapes

Use pill geometry for prominent actions and compact header controls. Use a small radius for large media frames and a medium radius for grouped surfaces. Keep separators straight and subtle. Do not use sharp decorative angles or excessive rounding on ordinary content containers.

## Components

- **page:** Uses `{colors.background}` as the canvas, `{colors.foreground}` for text, and `{typography.body}` as the base type.
- **header:** Aligns interface elements to shared horizontal gutters using `{colors.background}`, `{colors.foreground}`, and `{typography.navigation}`.
- **navigation:** Uses `{colors.background}` and `{colors.foreground}` with the regular navigation type style.
- **hero:** Uses `{colors.background}`, `{colors.foreground}`, and `{typography.heading}` with spacious vertical padding.
- **surface:** Groups secondary content with `{colors.surface}`, `{colors.on-surface}`, and `{rounded.md}`.
- **media-frame:** Presents large visual content on `{colors.surface}` with `{colors.on-surface}` and `{rounded.sm}`.
- **border:** Uses `{colors.border}` as a one-pixel structural separator.
- **button-primary:** Uses `{colors.primary}` with `{colors.on-primary}` text, `{rounded.pill}`, and generous horizontal padding.
- **button-primary-hover:** Remains a high-emphasis control using `{colors.primary-hover}` and `{colors.on-primary}`.
- **button-secondary:** Uses `{colors.surface}` with `{colors.on-surface}` text, `{rounded.pill}`, and the same comfortable control padding as the primary action.
- **heading:** Uses `{colors.foreground}` and `{typography.heading}` for prominent introductory text.
- **floating-control:** Uses `{colors.surface}`, `{colors.on-surface}`, and `{rounded.pill}` for a compact control positioned above the page content.

## Do's and Don'ts

### Do

- Use shared horizontal gutters for the header, introductory content, and major visual surfaces.
- Preserve generous whitespace between major sections.
- Use pill-shaped actions with clear primary and secondary emphasis.
- Keep primary text and control pairs at WCAG AA contrast.
- Reference design values through tokens such as `{colors.primary}` and `{spacing.lg}`.
- Use subtle borders and shadows only to clarify grouping or floating placement.

### Don't

- Do not hardcode captured colors inside component definitions.
- Do not nest hover, active, or pressed variants inside a base component.
- Do not replace the warm neutral canvas with stark white or dark page backgrounds.
- Do not use heavy font weights, ornamental type, or dense spacing that changes the quiet hierarchy.
- Do not add prominent gradients, decorative effects, or page-specific content.
