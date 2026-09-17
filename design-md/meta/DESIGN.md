---
version: "alpha"
name: "Meta Design System"
colors:
  primary: "#0457CB"
  on-primary: "#FFFFFF"
  primary-hover: "#0346A5"
  background: "#FFFFFF"
  foreground: "#1C2B33"
  muted: "#52606D"
  surface: "#F5F7FA"
  on-surface: "#1C2B33"
  border: "#D9DDE2"
typography:
  heading:
    fontFamily: "sans-serif"
    fontSize: "48px"
    fontWeight: "500"
    lineHeight: "52.8px"
    letterSpacing: "-0.48px"
  body:
    fontFamily: "sans-serif"
    fontSize: "18px"
    fontWeight: "400"
    lineHeight: "26px"
    letterSpacing: "0px"
  navigation:
    fontFamily: "sans-serif"
    fontSize: "16px"
    fontWeight: "500"
    lineHeight: "24px"
    letterSpacing: "0px"
  footer:
    fontFamily: "sans-serif"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
    letterSpacing: "0px"
rounded:
  sm: "8px"
  md: "32px"
  pill: "999px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  xxl: "64px"
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
    gap: "{spacing.xxl}"
  hero:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    gap: "{spacing.xxl}"
    padding: "{spacing.xxl}"
  hero-heading:
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
    marginBottom: "{spacing.lg}"
  hero-copy:
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    marginBottom: "{spacing.xxl}"
  media:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.navigation}"
    rounded: "{rounded.pill}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
    typography: "{typography.navigation}"
    rounded: "{rounded.pill}"
    padding: "{spacing.md}"
  icon-control:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.lg}"
  divider:
    backgroundColor: "{colors.border}"
    height: "1px"
  footer:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.footer}"
    padding: "{spacing.xxl}"
  footer-column:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.footer}"
    gap: "{spacing.sm}"
  footer-heading:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    marginBottom: "{spacing.sm}"
  footer-link:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.footer}"
  floating-control:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.pill}"
    padding: "{spacing.sm}"
---

## Overview

This design system defines a spacious, high-contrast interface with a horizontal navigation header, split hero composition, rounded media, pill-shaped primary actions, and a multi-column footer. It emphasizes generous whitespace, dark neutral typography, vivid blue actions, and restrained structural borders.

## Colors

- **Primary:** Bright blue for high-emphasis actions and selected interactive elements.
- **On Primary:** White content placed on primary blue.
- **Primary Hover:** Darker blue for the hover state of primary actions.
- **Background:** White page and section canvas.
- **Foreground:** Dark blue-gray for primary text and navigation.
- **Muted:** Medium blue-gray for secondary links and supporting text.
- **Surface:** Very light neutral used for grouped or media-adjacent areas.
- **On Surface:** Dark text placed on the light surface.
- **Border:** Pale gray for thin section dividers and structural rules.

## Typography

Use a clean sans-serif family throughout. Apply the medium-weight heading style to prominent headings, the regular body style to descriptive copy, and the smaller medium-weight navigation style to links, controls, and footer headings. Maintain the captured generous line spacing and slightly tightened heading tracking.

## Layout

Use a full-width page canvas with a compact horizontal header. Align the primary navigation across the header with utility controls grouped at the opposite edge. Build the main hero as a two-part composition: a text-and-action area alongside a large media area. Preserve generous horizontal gutters and substantial unused space around the hero content.

Use a full-width divider before the footer. Arrange footer content in multiple columns with a separate identity and social-control area, followed by grouped link lists. Allow the columns to collapse into a vertical flow at narrower widths.

## Elevation & Depth

The interface is primarily flat, with no visible card shadows or strong elevation treatment. Use spacing, section separation, rounded media, and contrast changes to establish hierarchy. Reserve subtle elevation for floating controls when needed to distinguish them from the page canvas.

## Shapes

Use a pill radius for prominent action buttons and compact floating controls. Use a larger rounded radius for large media areas, with rounding visible at the lower corners of the media container. Keep navigation and footer controls lightly rounded rather than fully pill-shaped.

## Components

- **header:** Full-width white navigation bar using {colors.background}, {colors.foreground}, and {typography.navigation}.
- **navigation:** Horizontal link group with consistent spacing and dark foreground text.
- **hero:** Spacious split composition using {colors.background}, large gutters, and a generous gap between text and media.
- **hero-heading:** Prominent medium-weight heading using {typography.heading}.
- **hero-copy:** Supporting descriptive text using {typography.body}.
- **media:** Large visual region using {colors.surface} with {rounded.md}.
- **button-primary:** Pill-shaped high-emphasis action using {colors.primary} and {colors.on-primary}.
- **button-primary-hover:** Separate hover state using {colors.primary-hover} and {colors.on-primary}.
- **icon-control:** Compact utility control using {colors.background} and {colors.foreground}.
- **surface:** Light grouped region using {colors.surface} and {colors.on-surface}.
- **divider:** One-pixel structural separator using {colors.border}.
- **footer:** Spacious multi-column footer using {colors.background} and {colors.foreground}.
- **footer-column:** Secondary link grouping using {colors.background}, {colors.muted}, and {typography.footer}.
- **footer-heading:** High-emphasis footer label using {colors.foreground} and {typography.navigation}.
- **footer-link:** Muted footer link using {colors.background} and {colors.muted}.
- **floating-control:** Small rounded persistent control using {colors.background} and {colors.foreground}.

## Do's and Don'ts

### Do

- Use {colors.primary} only for the strongest interactive emphasis.
- Keep primary action text at {colors.on-primary} for accessible contrast.
- Preserve the wide gutters, open whitespace, and split hero composition.
- Use {rounded.pill} for primary actions and {rounded.md} for large media.
- Keep footer groups aligned in consistent vertical columns.
- Maintain visible contrast between foreground text, muted links, surfaces, and the white canvas.

### Don't

- Do not introduce heavy shadows, gradients, or dense card treatments.
- Do not use dark surfaces as the default grouped-content background.
- Do not replace the pill-shaped primary action with a small rectangular control.
- Do not crowd the header, hero, or footer with tight spacing.
- Do not nest interaction states inside a base component.
- Do not hardcode colors or spacing values inside component definitions.
