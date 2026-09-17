---
version: "alpha"
name: "Slack Design System"
omitted:
  - "source-specific copy"
  - "logos and product marks"
  - "personal imagery"
colors:
  primary: "#611F69"
  on-primary: "#FFFFFF"
  primary-hover: "#4A154B"
  background: "#FFFFFF"
  foreground: "#000000"
  surface: "#FFFFFF"
  on-surface: "#000000"
  border: "#696969"
  wash-pink: "#FFF1F6"
  wash-yellow: "#FFFDEB"
typography:
  heading:
    fontFamily: "sans-serif"
    fontSize: "64px"
    fontWeight: "700"
    lineHeight: "1.25"
    letterSpacing: "-0.64px"
  body:
    fontFamily: "sans-serif"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "1.5"
  navigation:
    fontFamily: "sans-serif"
    fontSize: "20px"
    fontWeight: "700"
    lineHeight: "1.2"
  button:
    fontFamily: "sans-serif"
    fontSize: "20px"
    fontWeight: "700"
    lineHeight: "1.2"
rounded:
  sm: "4px"
  md: "16px"
  full: "999px"
spacing:
  hairline: "1px"
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  2xl: "64px"
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
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
  border:
    backgroundColor: "{colors.border}"
    height: "{spacing.hairline}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
  button-secondary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.primary}"
    borderColor: "{colors.primary}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  heading:
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  hero-background:
    backgroundStartColor: "{colors.wash-pink}"
    backgroundEndColor: "{colors.wash-yellow}"
  app-preview:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
---

## Overview

This system captures a spacious, centered interface with a white canvas, strong typographic hierarchy, purple primary actions, outlined secondary actions, and a large rounded interface preview. Navigation remains compact and horizontal while the main content uses generous vertical spacing.

## Colors

- **Primary:** Deep purple for high-emphasis actions, active indicators, and interface chrome.
- **On Primary:** White content placed on purple controls and surfaces.
- **Primary Hover:** Darker purple for interactive hover states.
- **Background:** White page canvas.
- **Foreground:** Black text for high-contrast headings and navigation.
- **Surface:** White content panels and grouped areas.
- **On Surface:** Black content placed on light surfaces.
- **Border:** Medium gray for structural separators and subtle outlines.
- **Wash Pink:** Pale pink end of the soft lower-page background wash.
- **Wash Yellow:** Pale yellow end of the soft lower-page background wash.

## Typography

Use a bold, condensed-feeling sans-serif treatment for large headings. Headings are approximately 64px with a tight letter spacing and generous line height. Body copy remains 16px with a 1.5 line height. Navigation and buttons use a heavier 20px sans-serif treatment.

## Layout

Use a wide centered content area with generous horizontal margins. Keep the header in a single horizontal row with navigation grouped toward the left and actions aligned toward the right. Center the hero content, place actions in a horizontal group, and separate supporting content from the hero with large vertical spacing. Use the spacing scale rather than fixed page-specific dimensions.

## Elevation & Depth

Use a restrained soft shadow around floating or preview-like surfaces, approximately 0 0 32px with 10% black opacity. Keep the primary page canvas visually flat and reserve depth for grouped interface previews or floating controls.

## Shapes

Use small 4px corners for buttons and controls. Use larger 16px corners for grouped surfaces and the large interface preview. Reserve the full radius for circular status, avatar, or utility controls.

## Components

- **page:** White canvas with black body text using {colors.background}, {colors.foreground}, and {typography.body}.
- **header:** White horizontal navigation area using {colors.background}, {colors.foreground}, and {typography.navigation}.
- **surface:** White grouped panel with black content using {colors.surface}, {colors.on-surface}, and {rounded.md}.
- **border:** One-pixel structural separator using {colors.border} and {spacing.hairline}.
- **button-primary:** Filled purple action with white text using {colors.primary}, {colors.on-primary}, {typography.button}, and {rounded.sm}.
- **button-primary-hover:** Darkened filled action using {colors.primary-hover} and {colors.on-primary}.
- **button-secondary:** White outlined action with purple text and border using {colors.background}, {colors.primary}, {typography.button}, and {rounded.sm}.
- **heading:** Large black display text using {colors.foreground} and {typography.heading}.
- **hero-background:** Subtle lower-page wash transitioning between {colors.wash-pink} and {colors.wash-yellow}.
- **app-preview:** Large purple interface preview with white content using {colors.primary}, {colors.on-primary}, and {rounded.md}.

## Do's and Don'ts

### Do

- Use {colors.primary} for the strongest action and active emphasis.
- Pair purple controls with {colors.on-primary} for readable contrast.
- Keep hero content centered and allow generous whitespace around it.
- Use separate flat entries for interactive states such as button-primary-hover.
- Preserve the distinction between filled primary actions and outlined secondary actions.
- Maintain WCAG AA contrast for all text and interactive controls.

### Don't

- Do not hardcode captured colors inside component definitions.
- Do not nest hover, active, or pressed variants inside a base component.
- Do not use large rounded corners on compact controls.
- Do not overcrowd the header or hero with dense spacing.
- Do not add source-specific copy, marks, or imagery to reusable components.
