---
version: "alpha"
name: "Stripe Design System"
colors:
  primary: "#533AFD"
  on-primary: "#FFFFFF"
  primary-hover: "#4530D4"
  background: "#FFFFFF"
  foreground: "#0A2540"
  surface: "#F6F9FC"
  on-surface: "#0A2540"
  border: "#D8DEE8"
typography:
  heading:
    fontFamily: "sohne-var"
    fontSize: "48px"
    fontWeight: "400"
    lineHeight: "1.15"
    letterSpacing: "-0.96px"
  body:
    fontFamily: "sohne-var"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "1.5"
  stat:
    fontFamily: "sohne-var"
    fontSize: "28px"
    fontWeight: "400"
    lineHeight: "1.2"
rounded:
  sm: "6px"
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
  content-container:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    padding: "{spacing.xl}"
  heading:
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  body:
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
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
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
  button-secondary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.primary}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-secondary-hover:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.primary}"
  media-frame:
    backgroundColor: "{colors.surface}"
    rounded: "{rounded.md}"
  statistics-row:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    padding: "{spacing.lg}"
  statistic-value:
    textColor: "{colors.foreground}"
    typography: "{typography.stat}"
  divider:
    backgroundColor: "{colors.border}"
    height: "1px"
---

## Overview

This design system describes a spacious editorial layout with a white canvas, dark navy typography, vivid purple actions, wide media panels, and supporting statistics. Content is arranged in a centered container with generous horizontal margins and clear vertical separation.

## Colors

- **Primary:** Vivid purple for prominent actions and interactive accents.
- **On Primary:** White content placed on primary controls.
- **Primary Hover:** Darker purple for hovered primary controls.
- **Background:** White page canvas and light control surfaces.
- **Foreground:** Deep navy for headings, body copy, and high-emphasis values.
- **Surface:** Very light cool gray for subtle grouping and secondary hover states.
- **On Surface:** Deep navy content on light surfaces.
- **Border:** Pale cool gray for outlined controls and separators.

## Typography

Use **sohne-var** throughout the hierarchy. Large headings use a 48px size, regular weight, tight tracking, and a 1.15 line height. Body copy uses 16px regular text with a 1.5 line height. Prominent statistics use 28px regular text with compact line spacing.

## Layout

Use a centered content container with generous horizontal padding. Stack the introductory row, full-width media frame, statistics row, and subsequent content sections vertically. Keep the primary media presentation wide and visually dominant. Use a three-column arrangement for related statistics at wide widths, allowing the columns to collapse responsively on smaller screens. Separate repeated content groups with a subtle horizontal divider.

## Elevation & Depth

The reference uses minimal elevation. Prefer flat white surfaces and thin borders; reserve a soft, low-contrast shadow for floating controls or overlays when separation from the page is necessary.

## Shapes

Use a 12px radius for large media frames and grouped surfaces. Use a 6px radius for buttons and compact controls. Keep dividers square and one pixel high.

## Components

- **content-container:** Centered page region using {colors.background}, with {spacing.xl} padding.
- **heading:** Large dark-navy editorial heading using {colors.foreground} and {typography.heading}.
- **body:** Regular supporting copy using {colors.foreground} and {typography.body}.
- **button-primary:** High-emphasis action using {colors.primary} with {colors.on-primary} text.
- **button-primary-hover:** Hover state using {colors.primary-hover} with {colors.on-primary} text.
- **button-secondary:** Outlined or light-background action using {colors.background} with {colors.primary} text.
- **button-secondary-hover:** Secondary hover state using {colors.surface} with {colors.primary} text.
- **media-frame:** Wide visual content region using {colors.surface} with {rounded.md}.
- **statistics-row:** Horizontal supporting-information region using {colors.background}, {colors.foreground}, and {spacing.lg}.
- **statistic-value:** Prominent numeric or short-value treatment using {colors.foreground} and {typography.stat}.
- **surface:** Light grouped area using {colors.surface}, {colors.on-surface}, and {rounded.md}.
- **divider:** Subtle section separator using {colors.border}.

## Do's and Don'ts

### Do

- Use wide media areas as the dominant visual element in a content section.
- Preserve generous whitespace and consistent container alignment.
- Use dark navy for readable text and purple for high-emphasis actions.
- Reference spacing, typography, colors, and shapes through tokens.
- Maintain WCAG AA contrast for text and interactive controls.
- Keep hover states as separate flat component entries.

### Don't

- Do not hardcode captured colors inside component definitions.
- Do not use strong shadows or excessive decorative effects.
- Do not crowd the media frame, statistics, or section headings.
- Do not nest hover, active, or pressed variants inside a base component.
- Do not introduce source-specific copy, names, logos, or page content into reusable patterns.
