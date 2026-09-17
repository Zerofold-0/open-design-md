---
version: "alpha"
name: "Airbnb Design System"
colors:
  primary: "#C8103C"
  on-primary: "#FFFFFF"
  primary-hover: "#A90D32"
  background: "#FFFFFF"
  foreground: "#222222"
  surface: "#F7F7F7"
  on-surface: "#222222"
  muted: "#6A6A6A"
  border: "#DDDDDD"
  shadow: "#D9D9D9"
typography:
  heading:
    fontFamily: "sans-serif"
    fontSize: "30px"
    fontWeight: "700"
    lineHeight: "36px"
    letterSpacing: "-0.02em"
  body:
    fontFamily: "sans-serif"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
    letterSpacing: "0em"
  label:
    fontFamily: "sans-serif"
    fontSize: "14px"
    fontWeight: "700"
    lineHeight: "20px"
    letterSpacing: "0em"
  metadata:
    fontFamily: "sans-serif"
    fontSize: "14px"
    fontWeight: "400"
    lineHeight: "20px"
    letterSpacing: "0em"
rounded:
  sm: "8px"
  md: "12px"
  lg: "24px"
  pill: "999px"
  circle: "50%"
spacing:
  hairline: "1px"
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
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    padding: "{spacing.md} {spacing.xl}"
  navigation:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    padding: "{spacing.sm} {spacing.md}"
  navigation-active:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.label}"
    padding: "{spacing.sm} {spacing.md}"
  search-bar:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "{spacing.md} {spacing.lg}"
    borderColor: "{colors.border}"
    boxShadow: "{colors.shadow} 0px 2px 6px 0px"
  search-field:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    padding: "{spacing.sm} {spacing.md}"
  search-action:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.circle}"
    padding: "{spacing.md}"
  search-action-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.circle}"
  icon-button:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.circle}"
    padding: "{spacing.sm}"
  icon-button-hover:
    backgroundColor: "{colors.border}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.circle}"
    padding: "{spacing.sm}"
  section:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    padding: "{spacing.xl} 0"
  section-heading:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  card:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    rounded: "{rounded.lg}"
  card-title:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.label}"
    padding: "{spacing.sm} 0 0"
  card-metadata:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.metadata}"
  card-image:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.lg}"
  favorite-button:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.circle}"
    padding: "{spacing.sm}"
  feature-badge:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "{spacing.sm} {spacing.md}"
  avatar:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.circle}"
    padding: "{spacing.xs}"
  divider:
    backgroundColor: "{colors.border}"
    height: "{spacing.hairline}"
---

## Overview

This system uses a bright, spacious interface with a strong black text hierarchy, restrained gray utility surfaces, and a saturated accent for primary actions. Content is organized into horizontal card rails beneath a prominent header and search area.

## Colors

- **Primary:** Saturated accent reserved for the main search or primary action.
- **On Primary:** White content used on the primary accent.
- **Primary Hover:** Darker accent for hovered primary actions.
- **Background:** White page canvas and card background.
- **Foreground:** Near-black text and high-emphasis icon color.
- **Surface:** Very light gray used for circular utility controls and soft badges.
- **On Surface:** High-contrast text used on light surfaces.
- **Muted:** Medium gray for supporting metadata and secondary information.
- **Border:** Light gray for dividers, outlines, and subtle control boundaries.
- **Shadow:** Pale neutral used for restrained search-container depth.

## Typography

Use a clean sans-serif family throughout. Large section headings are bold and compact, while labels use a smaller bold treatment. Body and metadata text use regular weight, with muted color reserved for supporting information. Keep heading tracking slightly tight and maintain the captured line-height hierarchy.

## Layout

- Use a broad header with primary navigation distributed horizontally across the top.
- Keep the main search control centered and visually prominent below the navigation.
- Separate the header region from the content area with a subtle divider.
- Organize content into full-width horizontal rails with a heading, an optional circular directional control, and a row of cards.
- Keep consistent horizontal gutters and generous vertical spacing between content rails.
- Cards should preserve a consistent image-first structure with text metadata directly below.
- Allow card rails to scroll or clip horizontally at narrower widths rather than forcing dense wrapping.

## Elevation & Depth

Use shallow depth for the prominent search control through a light border and restrained shadow. Utility controls and badges should rely primarily on their surface contrast rather than strong elevation. Avoid heavy shadows on content cards.

## Shapes

- Use a pill shape for the search container and compact feature badges.
- Use circular shapes for search, profile, favorite, and directional icon controls.
- Use a large consistent radius for card imagery and card containers.
- Keep borders subtle and avoid mixing sharp and highly rounded treatments within the same control group.

## Components

- **header:** Provides the white top-level navigation region with generous horizontal padding.
- **navigation:** Displays neutral navigation items with regular body typography.
- **navigation-active:** Emphasizes the selected navigation item using bold foreground text and an active indicator.
- **search-bar:** Uses a pill-shaped white container, light border, and shallow shadow to group search fields.
- **search-field:** Presents a labeled search segment with dark primary text and spacious internal padding.
- **search-action:** Uses {colors.primary} with {colors.on-primary} for the circular primary search control.
- **search-action-hover:** Uses {colors.primary-hover} with {colors.on-primary} as the independent hover state.
- **icon-button:** Uses {colors.surface} with {colors.foreground} for circular utility actions.
- **icon-button-hover:** Uses {colors.border} with {colors.foreground} for utility-control hover feedback.
- **section:** Groups a heading and a horizontal collection of content cards.
- **section-heading:** Uses {colors.foreground} and {typography.heading} for high-emphasis rail headings.
- **card:** Combines a rounded image area with concise supporting information below.
- **card-title:** Uses {colors.foreground} and {typography.label} for the primary card label.
- **card-metadata:** Uses {colors.muted} and {typography.metadata} for dates, prices, ratings, or other supporting details.
- **card-image:** Uses {colors.surface} as a loading or fallback background with {rounded.lg} corners.
- **favorite-button:** Places a high-contrast foreground icon on a circular {colors.surface} control over card imagery.
- **feature-badge:** Uses {colors.surface} with {colors.on-surface} text in a compact pill-shaped overlay.
- **avatar:** Uses a circular {colors.surface} container for a small profile representation.
- **divider:** Uses {colors.border} at {spacing.hairline} thickness for structural separation.

## Do's and Don'ts

### Do

- Reference visual values through tokens such as {colors.primary}, {spacing.md}, and {rounded.lg}.
- Preserve the strong contrast between white canvases, near-black text, and muted supporting metadata.
- Keep primary actions distinct from neutral utility controls.
- Maintain consistent image proportions, rounded corners, and metadata spacing across card rails.
- Use independent flat entries for hover and active states.

### Don't

- Do not hardcode captured colors inside component definitions.
- Do not use the primary accent for every control or decorative element.
- Do not add heavy shadows or sharp corners to the card-based content system.
- Do not nest hover, active, or pressed variants inside a base component.
- Do not introduce page-specific copy, identities, or content into reusable patterns.
