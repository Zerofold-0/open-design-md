---
version: "alpha"
name: "Arc Design System"
omitted:
  - "Source-specific copy, names, logos, URLs, and imagery"
colors:
  primary: "#3737F5"
  on-primary: "#FFFFFF"
  primary-hover: "#2929C9"
  background: "#FFFCEC"
  foreground: "#000000"
  surface: "#FFFFFF"
  on-surface: "#000000"
  border: "#D9D9D9"
typography:
  heading:
    fontFamily: "Marlin Soft SQ"
    fontSize: "45.51px"
    fontWeight: "700"
    lineHeight: "42.25px"
    letterSpacing: "-1.8204px"
  body:
    fontFamily: "Marlin"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "1.5"
  supporting:
    fontFamily: "Marlin"
    fontSize: "24px"
    fontWeight: "400"
    lineHeight: "1.35"
rounded:
  sm: "8px"
  md: "16px"
  lg: "48px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
components:
  page:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  header:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    padding: "{spacing.xl}"
  navigation:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    padding: "{spacing.md}"
  scalloped-divider:
    backgroundColor: "{colors.primary}"
    height: "{spacing.sm}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
  browser-preview:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    borderColor: "{colors.border}"
    padding: "{spacing.sm}"
  border:
    backgroundColor: "{colors.border}"
    height: "1px"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
  assistant-cta:
    backgroundColor: "{colors.foreground}"
    textColor: "{colors.background}"
    typography: "{typography.supporting}"
    rounded: "{rounded.lg}"
    padding: "{spacing.md}"
  chat-bubble:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.lg}"
    padding: "{spacing.md}"
  heading:
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  supporting-text:
    textColor: "{colors.foreground}"
    typography: "{typography.supporting}"
---

## Overview

This system uses a vivid blue navigation band, a warm near-white canvas, high-contrast dark typography, generous open spacing, and rounded interface surfaces. The primary composition is centered, with a prominent heading, supporting text, dark pill-shaped call to action, and a large browser-style preview.

## Colors

- **Primary:** Saturated blue used for the header, navigation, selected controls, and highlighted interface elements.
- **On Primary:** White content placed on the blue primary color.
- **Primary Hover:** A darker blue interaction state for primary controls.
- **Background:** Warm near-white page canvas.
- **Foreground:** Black, used for headings, body text, and dark high-emphasis controls.
- **Surface:** White used for the browser-style preview and grouped content.
- **On Surface:** Black content placed on white surfaces.
- **Border:** Very light neutral gray used for structural outlines and separators.

## Typography

Use Marlin Soft SQ for the large, distinctive heading treatment. Headings are heavy, tightly tracked, and use a compact line height. Use Marlin for body and supporting text, with the supporting scale reserved for prominent explanatory text. Keep text centered in the hero composition and use black for high-emphasis copy.

## Layout

- Use a centered hero stack with a large vertical gap between supporting text, the primary call to action, and the preview surface.
- Keep the header content in a horizontal navigation row with generous horizontal padding.
- Use broad page gutters around the large browser-style preview.
- Allow the preview to scale fluidly while preserving its rounded outer frame.
- Maintain substantial whitespace around the hero content rather than filling the canvas with dense controls.
- Use a blue band above and below the main light content area, with a repeating scalloped transition at the boundary.

## Elevation & Depth

The browser-style preview uses a subtle neutral outline and soft shadow to separate it from the warm canvas. The dark call-to-action pill also has a restrained shadow that lifts it from the page. Keep depth soft and diffuse; avoid heavy borders or dramatic elevation.

## Shapes

- Use small rounded corners for standard controls and borders.
- Use medium rounded corners for large grouped surfaces and the browser-style preview.
- Use a large pill radius for the prominent dark call to action and chat-style bubbles.
- Preserve the repeating scalloped edge where the blue band meets the light content area.
- Keep interface controls geometric and rounded without introducing sharp decorative shapes.

## Components

- **header:** Blue full-width band using {colors.primary} with {colors.on-primary} content and generous padding.
- **navigation:** Horizontal header navigation using {colors.primary} and {colors.on-primary}.
- **scalloped-divider:** Repeating blue transition using {colors.primary}.
- **page:** Warm canvas using {colors.background} with {colors.foreground} text.
- **surface:** White grouped area using {colors.surface} and {colors.on-surface}.
- **browser-preview:** Large rounded white preview using {colors.surface}, {colors.on-surface}, and {colors.border}.
- **border:** Thin structural separator using {colors.border}.
- **button-primary:** High-emphasis blue action using {colors.primary} and {colors.on-primary}.
- **button-primary-hover:** Darkened blue hover state using {colors.primary-hover} and {colors.on-primary}.
- **assistant-cta:** Dark pill-shaped action using {colors.foreground} with {colors.background} content.
- **chat-bubble:** Rounded highlighted message using {colors.primary} with {colors.on-primary} content.
- **heading:** Large centered heading using {colors.foreground} and {typography.heading}.
- **supporting-text:** Prominent supporting copy using {colors.foreground} and {typography.supporting}.

## Do's and Don'ts

### Do

- Reference visual values through tokens such as {colors.primary} and {spacing.xl}.
- Preserve the strong blue-and-warm-white contrast between the outer bands and central content.
- Use generous whitespace and centered alignment for the primary hero stack.
- Maintain WCAG AA contrast for text and interactive controls.
- Keep hover states as separate flat component entries.
- Preserve the soft shadow treatment and rounded browser-preview frame.

### Don't

- Do not hardcode captured colors inside component definitions.
- Do not nest hover, active, or pressed variants inside a base component.
- Do not replace the pill-shaped call to action with a sharp rectangular control.
- Do not introduce dense layouts, heavy outlines, or additional decorative styles unsupported by the interface.
- Do not use source-specific copy, logos, names, or imagery as part of the reusable system.
