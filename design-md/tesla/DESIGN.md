---
version: "alpha"
name: "Tesla Design System"
colors:
  primary: "#3E6AE1"
  on-primary: "#FFFFFF"
  primary-hover: "#3457B2"
  background: "#FFFFFF"
  foreground: "#171A20"
  surface: "#F4F4F4"
  on-surface: "#171A20"
  border: "#393C41"
typography:
  heading:
    fontFamily: "Universal Sans Display"
    fontSize: "48px"
    fontWeight: "500"
    lineHeight: "56px"
    letterSpacing: "0em"
  body:
    fontFamily: "Universal Sans Text"
    fontSize: "14px"
    fontWeight: "400"
    lineHeight: "20px"
    letterSpacing: "0em"
  navigation:
    fontFamily: "Universal Sans Text"
    fontSize: "16px"
    fontWeight: "500"
    lineHeight: "24px"
    letterSpacing: "0em"
  button:
    fontFamily: "Universal Sans Text"
    fontSize: "16px"
    fontWeight: "500"
    lineHeight: "24px"
    letterSpacing: "0em"
rounded:
  sm: "4px"
  md: "8px"
  lg: "999px"
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
  navigation:
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
    height: "1px"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-secondary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.button}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  icon-button:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm}"
  carousel-control:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  carousel-indicator:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xs}"
  floating-action-bar:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
  heading:
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
---

## Overview

This design system describes a clean, spacious interface with a white global canvas, dark neutral text, blue primary actions, rounded controls, and prominent image-led content areas. Navigation and utility controls remain visually restrained so that the central content and calls to action receive emphasis.

## Colors

- **Primary:** Blue emphasis color for primary actions and selected interactive elements.
- **On Primary:** White foreground for content placed on the primary color.
- **Primary Hover:** Darker blue interaction state for primary actions.
- **Background:** White page canvas and light secondary action surfaces.
- **Foreground:** Dark neutral for navigation, headings, labels, and icons.
- **Surface:** Light gray fill for utility controls, grouped areas, and carousel controls.
- **On Surface:** Dark neutral content on light gray surfaces.
- **Border:** Dark neutral structural color for separators and outlined details.

## Typography

Use the captured display face for large headings and the captured text face for navigation, body copy, and controls. Headings use a large 48px size with a 56px line height. Body copy is compact at 14px with a 20px line height, while navigation and button labels use a 16px size with a 24px line height and medium weight.

## Layout

Use a full-width page canvas with a tall horizontal navigation region. Keep navigation content aligned to generous horizontal margins and distribute primary navigation centrally with utility controls at the opposite edge.

Hero content is centered over a large visual media area. Stack the heading, supporting link or label, and primary and secondary actions with generous vertical spacing. Place paired actions in a horizontal row on wide layouts and allow them to stack on narrow layouts.

Use edge-aligned carousel controls over media, centered indicators near the lower edge, and generous spacing between major sections. A persistent lower action area can contain horizontally arranged utility actions while maintaining a white background and clear separation from page content.

## Elevation & Depth

Use a subtle inset or boundary treatment for persistent and floating controls rather than strong shadows. Keep image content visually dominant; utility bars and controls should use restrained separation from the page with a light structural edge or minimal depth.

## Shapes

Use small rounded corners for buttons and compact controls. Use medium rounded corners for grouped surfaces and persistent action areas. Use fully rounded geometry for circular indicators and circular utility controls. Avoid excessive rounding on large content containers unless the component is explicitly a grouped card.

## Components

- **navigation:** White full-width navigation region using {colors.background}, {colors.foreground}, and {typography.navigation}.
- **button-primary:** High-emphasis action using {colors.primary}, {colors.on-primary}, and {typography.button}.
- **button-primary-hover:** Independent hover state using {colors.primary-hover} with {colors.on-primary}.
- **button-secondary:** Light secondary action using {colors.background} with {colors.foreground}.
- **icon-button:** Compact utility control using {colors.surface} with {colors.foreground}.
- **carousel-control:** Edge-positioned media navigation control using {colors.surface} with {colors.foreground}.
- **carousel-indicator:** Small rounded carousel position marker using {colors.surface}.
- **floating-action-bar:** Persistent lower action region using {colors.background} with {colors.foreground}.
- **surface:** Light gray grouped region using {colors.surface} and {colors.on-surface}.
- **border:** Structural separator using {colors.border}.
- **page:** Base canvas using {colors.background} and {colors.foreground}.
- **heading:** Large display text using {colors.foreground} and {typography.heading}.

## Do's and Don'ts

### Do

- Reference design values through tokens such as {colors.primary}.
- Keep primary and secondary actions visually distinct through fill and text contrast.
- Use generous whitespace around hero content and major sections.
- Keep utility controls compact, consistent, and easy to scan.
- Maintain WCAG AA contrast for text and interactive controls.
- Preserve separate flat entries for hover and other interaction states.

### Don't

- Do not hardcode captured colors inside component definitions.
- Do not nest hover, active, or pressed variants inside a base component.
- Do not use heavy shadows that compete with image-led content.
- Do not introduce dense layouts or unnecessary decorative styling.
- Do not add source-specific labels, imagery, or content to reusable component rules.
