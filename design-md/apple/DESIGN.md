---
version: "alpha"
name: "Apple Design System"
colors:
  primary: "#0076DB"
  on-primary: "#FFFFFF"
  primary-hover: "#0075D9"
  link: "#005FCC"
  background: "#000000"
  foreground: "#FFFFFF"
  surface: "#F5F5F7"
  on-surface: "#000000"
  border: "#D2D2D7"
  muted: "#86868B"
typography:
  heading:
    fontFamily: "system-ui, sans-serif"
    fontSize: "56px"
    fontWeight: "600"
    lineHeight: "60px"
    letterSpacing: "-1.12px"
  body:
    fontFamily: "system-ui, sans-serif"
    fontSize: "17px"
    fontWeight: "400"
    lineHeight: "25px"
    letterSpacing: "-0.022px"
rounded:
  sm: "9999px"
  md: "12px"
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
  utility-banner:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    padding: "{spacing.lg}"
  navigation:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    padding: "{spacing.md}"
  promotion:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    padding: "{spacing.lg}"
  hero:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
    padding: "{spacing.xl}"
  hero-secondary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.body}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-secondary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.primary}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
    borderColor: "{colors.primary}"
  button-secondary-hover:
    backgroundColor: "{colors.background}"
    textColor: "{colors.primary-hover}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
    borderColor: "{colors.primary-hover}"
  link:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.link}"
    typography: "{typography.body}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
  border:
    backgroundColor: "{colors.border}"
    height: "1px"
---

## Overview

This design system describes a spacious, high-contrast interface with light utility and navigation regions above a dark, centered feature area. Primary actions use bright blue pill-shaped controls, while secondary actions use outlined controls with the same pill geometry.

## Colors

- **Primary:** Bright blue for primary actions and emphasized interactive elements.
- **On Primary:** White content placed on primary controls.
- **Primary Hover:** Alternate blue for hovered primary actions and controls.
- **Link:** Darker blue for inline links on light surfaces.
- **Background:** Black canvas for the main feature area.
- **Foreground:** White high-emphasis content on the dark canvas.
- **Surface:** Very light gray used for utility, navigation, promotional, and grouped regions.
- **On Surface:** Black content placed on light surfaces.
- **Border:** Soft gray for subtle structural separation and outlines.
- **Muted:** Medium gray for secondary content on the dark canvas.

## Typography

Use a system sans-serif stack throughout. Large feature headings are semibold, tightly tracked, and centered. Supporting copy uses regular weight with a relaxed reading line height. Keep the strongest type contrast for the primary feature heading and use muted gray for secondary supporting text on dark backgrounds.

## Layout

- Stack utility, navigation, and promotional regions above the main feature area.
- Keep navigation content in a centered, wide horizontal container.
- Center feature messaging and actions along the main content axis.
- Place related actions in a horizontal group with consistent spacing.
- Use generous vertical spacing around the feature heading, supporting copy, and action group.
- Allow the feature visual to extend beneath the centered content while preserving clear separation from the controls.

## Elevation & Depth

Use minimal elevation in the interface chrome. Rely primarily on contrast, spacing, outlines, and large imagery for hierarchy. Soft shadows may be reserved for floating utility controls or small overlays.

## Shapes

- Use the pill radius for prominent actions, selectors, and compact controls.
- Use the medium radius for grouped surfaces and non-pill containers.
- Keep outlines thin and low contrast against light surfaces or dark backgrounds.
- Avoid mixing sharp rectangular controls with the rounded action language.

## Components

- **utility-banner:** Light, spacious contextual region using `{colors.surface}` and `{colors.on-surface}`.
- **navigation:** Light horizontal navigation region using `{colors.surface}` and `{colors.on-surface}`.
- **promotion:** Centered informational strip using `{colors.surface}` and `{colors.on-surface}`.
- **hero:** Dark feature region using `{colors.background}` and `{colors.foreground}` with large centered typography.
- **hero-secondary:** Supporting hero copy using `{colors.background}` and `{colors.muted}`.
- **button-primary:** Filled pill action using `{colors.primary}` with `{colors.on-primary}` text.
- **button-primary-hover:** Hover state using `{colors.primary-hover}` with `{colors.on-primary}` text.
- **button-secondary:** Outlined pill action using `{colors.background}`, `{colors.primary}`, and `{colors.primary}` for the outline.
- **button-secondary-hover:** Hover state using `{colors.background}`, `{colors.primary-hover}`, and `{colors.primary-hover}` for the outline.
- **link:** Inline emphasized action using `{colors.surface}` and `{colors.link}`.
- **surface:** Light grouped container using `{colors.surface}` and `{colors.on-surface}`.
- **border:** Subtle separator using `{colors.border}`.

## Do's and Don'ts

### Do

- Use token references for all component colors, typography, spacing, and shape values.
- Preserve the contrast between light interface chrome and the dark feature area.
- Center feature messaging and keep related actions aligned as a cohesive group.
- Use blue consistently for interactive emphasis.
- Maintain accessible contrast for text and controls.

### Don't

- Do not hardcode captured colors inside component definitions.
- Do not use rounded rectangles where the pill treatment is appropriate for an action.
- Do not add heavy shadows or decorative borders that compete with the feature visual.
- Do not introduce additional colors or typography styles without a reusable interface need.
