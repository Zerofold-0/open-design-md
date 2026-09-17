---
version: "alpha"
name: "Starbucks Design System"
colors:
  primary: "#00754A"
  on-primary: "#FFFFFF"
  primary-hover: "#006241"
  background: "#FFFFFF"
  foreground: "#000000"
  surface: "#FFFFFF"
  on-surface: "#000000"
  border: "#000000"
  muted-border: "#D9D9D9"
  deep-green: "#006241"
typography:
  heading:
    fontFamily: "sans-serif"
    fontSize: "48px"
    fontWeight: "700"
    lineHeight: "56px"
    letterSpacing: "-0.5px"
  body:
    fontFamily: "sans-serif"
    fontSize: "18px"
    fontWeight: "400"
    lineHeight: "28px"
  navigation:
    fontFamily: "sans-serif"
    fontSize: "16px"
    fontWeight: "700"
    lineHeight: "24px"
    letterSpacing: "2px"
  modal-heading:
    fontFamily: "sans-serif"
    fontSize: "48px"
    fontWeight: "400"
    lineHeight: "1.4"
  button:
    fontFamily: "sans-serif"
    fontSize: "16px"
    fontWeight: "700"
    lineHeight: "24px"
rounded:
  sm: "999px"
  md: "16px"
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
  header:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    padding: "{spacing.lg}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
  modal:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    borderColor: "{colors.muted-border}"
    padding: "{spacing.xxl}"
  hero:
    backgroundColor: "{colors.deep-green}"
    textColor: "{colors.on-primary}"
    padding: "{spacing.xxl}"
  border:
    backgroundColor: "{colors.border}"
    height: "1px"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm} {spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
  button-secondary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    borderColor: "{colors.border}"
    padding: "{spacing.sm} {spacing.lg}"
  button-dark:
    backgroundColor: "{colors.foreground}"
    textColor: "{colors.background}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm} {spacing.lg}"
  button-hero:
    backgroundColor: "{colors.deep-green}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    borderColor: "{colors.on-primary}"
    padding: "{spacing.sm} {spacing.lg}"
  heading:
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  hero-heading:
    textColor: "{colors.on-primary}"
    typography: "{typography.heading}"
  modal-heading:
    textColor: "{colors.on-surface}"
    typography: "{typography.modal-heading}"
  link:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
    typography: "{typography.body}"

---

## Overview

This design system describes a spacious, high-contrast interface with a white global canvas, dark green promotional sections, strong typographic hierarchy, pill-shaped actions, and a centered modal overlay.

## Colors

- **Primary:** Green used for prominent actions and links.
- **On Primary:** White content placed on green action and promotional backgrounds.
- **Primary Hover:** Darker green interaction state.
- **Background:** White global page canvas.
- **Foreground:** Black high-emphasis text and dark actions.
- **Surface:** White content surfaces and overlays.
- **On Surface:** Black content placed on white surfaces.
- **Border:** Black structural and outlined-control color.
- **Muted Border:** Light gray edge used around elevated overlays.
- **Deep Green:** Dark green promotional section background.

## Typography

Use a clean sans-serif family throughout the interface. Large headings are bold and tightly spaced, while modal headings use a large regular weight. Body text uses an 18px size with generous line height. Navigation labels and buttons are bold, with navigation labels using visibly expanded letter spacing.

## Layout

Use a full-width white header with horizontally distributed navigation and actions. Promotional content uses broad two-column compositions, pairing imagery or visual content with a centered text-and-action panel. Maintain generous outer margins and whitespace between stacked sections. Center modal overlays above page content with a constrained desktop width and substantial internal padding.

## Elevation & Depth

Use a soft layered shadow for centered modal overlays, with a subtle border to define the edge against light content. Keep the page and promotional sections visually flat; depth should primarily distinguish overlays from the underlying interface.

## Shapes

Use pill-shaped controls for buttons and compact actions. Use a medium radius for cards, dialogs, and grouped surfaces. Keep image and content sections rectangular unless a component specifically calls for a rounded control shape.

## Components

- **header:** White, full-width navigation region using {colors.surface}, {colors.foreground}, and {typography.navigation}.
- **hero:** Dark green promotional region using {colors.deep-green} and {colors.on-primary}, with spacious internal alignment.
- **modal:** Centered elevated surface using {colors.surface}, {colors.on-surface}, {colors.muted-border}, and {rounded.md}.
- **button-primary:** Green pill action using {colors.primary} and {colors.on-primary}.
- **button-primary-hover:** Dark green pill interaction state using {colors.primary-hover} and {colors.on-primary}.
- **button-secondary:** White outlined action using {colors.surface}, {colors.foreground}, and {colors.border}.
- **button-dark:** Black filled action using {colors.foreground} and {colors.background}.
- **button-hero:** Outlined action on a dark green section using {colors.deep-green} and {colors.on-primary}.
- **heading:** Large black heading using {colors.foreground} and {typography.heading}.
- **hero-heading:** Large white heading for dark sections using {colors.on-primary} and {typography.heading}.
- **modal-heading:** Large regular black dialog heading using {colors.on-surface} and {typography.modal-heading}.
- **link:** Green text link on a white surface using {colors.primary}, {colors.surface}, and {typography.body}.
- **border:** One-pixel black structural separator using {colors.border}.

## Do's and Don'ts

### Do

- Reference visual values through tokens such as {colors.primary} and {spacing.lg}.
- Preserve the strong contrast between white surfaces, black text, and dark green promotional regions.
- Use generous whitespace and consistent horizontal alignment.
- Keep dialog overlays clearly separated from the page with a light border and soft elevation.
- Use pill shapes for buttons and medium rounding for grouped surfaces.

### Don't

- Do not hardcode captured colors inside component definitions.
- Do not use rounded rectangles where the interface calls for pill-shaped controls.
- Do not flatten a modal into the page flow when it needs to sit above the underlying content.
- Do not introduce decorative colors, dense spacing, or additional visual effects that compete with the primary hierarchy.
