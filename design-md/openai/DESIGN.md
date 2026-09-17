---
version: "alpha"
name: "OpenAI Design System"
colors:
  primary: "#000000"
  on-primary: "#FFFFFF"
  primary-hover: "#2B2B2B"
  background: "#FFFFFF"
  foreground: "#000000"
  surface: "#F5F5F7"
  on-surface: "#000000"
  border: "#E5E5E5"
  muted: "#6B6B6B"
  accent: "#A9A8F5"
  accent-soft: "#E8E7FF"
typography:
  heading:
    fontFamily: "Arial, sans-serif"
    fontSize: "56px"
    fontWeight: "400"
    lineHeight: "1.14"
    letterSpacing: "-1.68px"
  body:
    fontFamily: "Arial, sans-serif"
    fontSize: "24px"
    fontWeight: "400"
    lineHeight: "1.48"
    letterSpacing: "-0.24px"
  navigation:
    fontFamily: "Arial, sans-serif"
    fontSize: "17px"
    fontWeight: "400"
    lineHeight: "1.4"
    letterSpacing: "-0.17px"
  supporting:
    fontFamily: "Arial, sans-serif"
    fontSize: "17px"
    fontWeight: "400"
    lineHeight: "1.5"
rounded:
  sm: "8px"
  md: "16px"
  lg: "32px"
  pill: "999px"
spacing:
  xs: "8px"
  sm: "16px"
  md: "24px"
  lg: "40px"
  xl: "64px"
  xxl: "96px"
components:
  page:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  header:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    padding: "{spacing.md}"
  navigation:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    gap: "{spacing.lg}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.navigation}"
    rounded: "{rounded.pill}"
    padding: "{spacing.sm} {spacing.lg}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
    typography: "{typography.navigation}"
    rounded: "{rounded.pill}"
    padding: "{spacing.sm} {spacing.lg}"
  button-secondary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.navigation}"
    rounded: "{rounded.pill}"
    padding: "{spacing.sm} {spacing.lg}"
  hero:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    padding: "{spacing.xxl} {spacing.lg}"
  heading:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  supporting-text:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
  media-panel:
    backgroundColor: "{colors.accent-soft}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.sm}"
  media-panel-accent:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.sm}"
  border:
    backgroundColor: "{colors.border}"
    height: "1px"
  muted-label:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.muted}"
    typography: "{typography.supporting}"
---

## Overview

This system captures a spacious, monochrome interface with strong black-and-white contrast, pill-shaped actions, restrained navigation, large editorial headings, and soft lavender media panels. Layouts use wide margins, generous vertical spacing, and split content areas that pair visual media with concise text.

## Colors

- **Primary:** Black, reserved for the highest-emphasis action.
- **On Primary:** White text placed on the primary action.
- **Primary Hover:** A slightly lighter black for interactive feedback.
- **Background:** White page canvas.
- **Foreground:** Black high-emphasis text and icons.
- **Surface:** Very light gray for secondary controls and grouped areas.
- **On Surface:** Black content placed on light surfaces.
- **Border:** Subtle light-gray structural separators.
- **Muted:** Medium gray for secondary labels and supporting metadata.
- **Accent:** Soft lavender used in visual media and decorative areas.
- **Accent Soft:** Pale lavender background for media compositions.

## Typography

Use a clean sans-serif family throughout. Large headings are regular-weight, tightly tracked, and set with a generous display size. Supporting copy uses a larger reading size with an open line height. Navigation and controls are smaller and visually direct, with no decorative text treatment.

## Layout

- Use a wide desktop header with the primary navigation arranged horizontally.
- Keep the main canvas white and allow substantial whitespace around content.
- Use split hero compositions in which a large visual panel occupies one side and text occupies the other.
- Align text blocks to a consistent content edge and constrain their measure for readable line lengths.
- Apply generous vertical gaps between major sections.
- Use compact internal gaps for navigation and controls, with larger gaps between content groups.
- Allow visual panels to extend across broad portions of the viewport while preserving consistent outer margins.
- Preserve responsive flow by stacking split compositions on narrower screens.

## Elevation & Depth

The interface is predominantly flat, with no prominent card shadows. Use borders and tonal contrast instead of heavy elevation. Soft media color changes provide depth within visual compositions, while floating controls may use only a very subtle separation from the page.

## Shapes

- Use fully rounded pill shapes for prominent actions and compact utility controls.
- Use modest corner rounding for media panels and grouped surfaces.
- Keep structural separators square or minimally rounded.
- Avoid excessive rounding on large page regions; rounding should clarify grouping or control affordance.

## Components

- **page:** White canvas with black default content using {colors.background} and {colors.foreground}.
- **header:** Spacious horizontal navigation region using {colors.background} and {colors.foreground}.
- **navigation:** Low-emphasis text navigation using {typography.navigation}.
- **button-primary:** High-emphasis black pill action using {colors.primary} with {colors.on-primary} text.
- **button-primary-hover:** Independent hover state using {colors.primary-hover} with {colors.on-primary} text.
- **button-secondary:** Light-gray pill control using {colors.surface} with {colors.on-surface} text.
- **hero:** Generous split-content region using {colors.background} and {colors.foreground}.
- **heading:** Large regular sans-serif heading using {typography.heading}.
- **supporting-text:** Spacious explanatory copy using {typography.body}.
- **surface:** Light grouped region using {colors.surface}, {colors.on-surface}, and {rounded.md}.
- **media-panel:** Soft lavender visual container using {colors.accent-soft} and {rounded.sm}.
- **media-panel-accent:** Lavender visual accent using {colors.accent} and {rounded.sm}.
- **border:** One-pixel structural separator using {colors.border}.
- **muted-label:** Secondary label using {colors.muted} on {colors.surface}.

## Do's and Don'ts

### Do

- Use {colors.primary} and {colors.on-primary} for the strongest action contrast.
- Keep the page predominantly white with restrained gray secondary surfaces.
- Use {colors.accent} and {colors.accent-soft} for visual emphasis rather than dense decoration.
- Preserve generous whitespace and broad horizontal composition.
- Use pill-shaped controls consistently for actions.
- Maintain WCAG AA contrast for all text and interactive control pairs.
- Reference visual values through tokens such as {colors.primary}, {spacing.lg}, and {rounded.pill}.

### Don't

- Do not introduce saturated colors outside the lavender accent range.
- Do not use heavy shadows or dense card treatments.
- Do not make secondary navigation compete with the primary action.
- Do not use large rounded corners on every container.
- Do not hardcode captured colors or dimensions inside component definitions.
- Do not nest hover or other interaction variants inside a base component.
