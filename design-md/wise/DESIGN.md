---
version: "alpha"
name: "Wise Design System"
omitted:
  - "Brand names, URLs, source-specific copy, personal data, and content-specific imagery"
colors:
  primary: "#0B3B00"
  on-primary: "#9BEA6C"
  primary-hover: "#062900"
  background: "#9BEA6C"
  foreground: "#0B3B00"
  surface: "#FFFFFF"
  on-surface: "#0B3B00"
  border: "#0B3B00"
typography:
  heading:
    fontFamily: "sans-serif"
    fontSize: "90px"
    fontWeight: "900"
    lineHeight: "0.85"
    letterSpacing: "-0.04em"
  body:
    fontFamily: "sans-serif"
    fontSize: "18px"
    fontWeight: "400"
    lineHeight: "26px"
    letterSpacing: "0em"
  navigation:
    fontFamily: "sans-serif"
    fontSize: "18px"
    fontWeight: "600"
    lineHeight: "24px"
    letterSpacing: "0em"
rounded:
  sm: "9999px"
  md: "48px"
  lg: "24px"
spacing:
  xs: "8px"
  sm: "16px"
  md: "24px"
  lg: "32px"
  xl: "48px"
  xxl: "64px"
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
    padding: "{spacing.xl}"
  navigation:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
  primary-action:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.navigation}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm}"
  primary-action-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
  hero:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    padding: "{spacing.xxl}"
  heading:
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  body-copy:
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  rating-summary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    padding: "{spacing.sm}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
    padding: "{spacing.lg}"
  media-surface:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.md}"
    padding: "{spacing.lg}"
  border:
    backgroundColor: "{colors.border}"
    height: "{spacing.hairline}"
---

## Overview

This system uses a vivid lime canvas, deep green typography, oversized heavy headings, generous vertical spacing, and pill-shaped primary actions. Content is centered within a broad responsive layout, with grouped media or information surfaces below the main action.

## Colors

- **Background:** Bright lime canvas used across the primary page region.
- **Foreground:** Deep green for headings, navigation, body copy, and high-emphasis icons.
- **Primary:** Deep green fill for high-emphasis actions.
- **On Primary:** Bright lime content placed on primary controls.
- **Primary Hover:** Darker green interaction state for primary actions.
- **Surface:** White for contained information areas and inset panels.
- **On Surface:** Deep green content on white surfaces.
- **Border:** Deep green for structural separators and outlines.

## Typography

Use a heavy, tightly spaced sans-serif treatment for large display headings. Headings are oversized, strongly weighted, and set with compact line height. Body copy uses a regular sans-serif style with an 18px size and 26px line height. Navigation and utility labels use the same sans-serif family with a semibold weight.

## Layout

Use a centered content column with generous horizontal margins and substantial vertical separation between ratings, headline, supporting copy, action, and lower content surfaces. Keep the main content width constrained so the display heading wraps into a small number of prominent lines. The header uses a horizontal navigation arrangement with utility controls aligned opposite the primary navigation.

## Elevation & Depth

Rely primarily on the contrast between the lime canvas, deep green controls, and white inset surfaces. Use restrained depth treatment rather than prominent shadows; separation should come from color, spacing, rounded containers, and occasional thin structural rules.

## Shapes

Use fully rounded pills for primary actions, compact utility controls, and status elements. Use large rounded corners for grouped media or information surfaces. Keep corners consistently soft and avoid sharp control geometry.

## Components

- **page:** Lime canvas using {colors.background} with deep green default text from {colors.foreground}.
- **header:** Spacious horizontal header using {colors.background}, {colors.foreground}, and {typography.navigation}.
- **navigation:** Semibold navigation labels using {colors.foreground} on {colors.background}.
- **primary-action:** Pill-shaped high-emphasis action using {colors.primary} with {colors.on-primary} text.
- **primary-action-hover:** Independent hover state using {colors.primary-hover} with {colors.on-primary} text.
- **hero:** Centered introductory region using {colors.background}, {colors.foreground}, and generous {spacing.xxl} spacing.
- **heading:** Oversized display text using {colors.foreground} and {typography.heading}.
- **body-copy:** Supporting text using {colors.foreground} and {typography.body}.
- **rating-summary:** Inline rating or trust summary using {colors.background}, {colors.foreground}, and {typography.navigation}.
- **surface:** White grouped panel using {colors.surface}, {colors.on-surface}, and {rounded.lg}.
- **media-surface:** Large rounded lower content surface using {colors.primary}, {colors.on-primary}, and {rounded.md}.
- **border:** Thin structural separator using {colors.border} and {spacing.hairline}.

## Do's and Don'ts

### Do

- Use the lime canvas as the dominant page color.
- Pair deep green text and controls with the lime background for strong contrast.
- Use oversized, compact display headings as the primary visual anchor.
- Keep primary actions pill-shaped and visually prominent.
- Use generous spacing and centered alignment for the main content flow.
- Keep hover states as separate component entries.
- Maintain WCAG AA contrast for all text and interactive controls.

### Don't

- Do not introduce brand names, source-specific copy, or page-specific content into the system.
- Do not replace the lime-and-deep-green contrast with neutral page colors.
- Do not use small, lightly weighted display headings where the captured hierarchy calls for heavy typography.
- Do not use sharp corners for primary controls or major grouped surfaces.
- Do not nest interaction states inside base component definitions.
- Do not hardcode color values inside component definitions.
