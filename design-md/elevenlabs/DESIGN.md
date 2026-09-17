---
version: "alpha"
name: "ElevenLabs Design System"
colors:
  primary: "#000000"
  on-primary: "#FFFFFF"
  primary-hover: "#1F1F1F"
  background: "#FFFFFF"
  foreground: "#000000"
  surface: "#F5F3F1"
  on-surface: "#000000"
  border: "#DEDEDE"
typography:
  heading:
    fontFamily: "Waldenburg"
    fontSize: "48px"
    fontWeight: "300"
    lineHeight: "52px"
    letterSpacing: "-0.96px"
  body:
    fontFamily: "Inter"
    fontSize: "18px"
    fontWeight: "400"
    lineHeight: "28.8px"
  navigation:
    fontFamily: "Inter"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
rounded:
  sm: "9999px"
  md: "24px"
  lg: "40px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  xxl: "64px"
  hairline: "1px"
components:
  page:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  navigation:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
  border:
    backgroundColor: "{colors.border}"
    height: "{spacing.hairline}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm} {spacing.lg}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm} {spacing.lg}"
  button-secondary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.border}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm} {spacing.lg}"
  button-secondary-hover:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.border}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.sm} {spacing.lg}"
  heading:
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  tab-group:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    borderColor: "{colors.border}"
    rounded: "{rounded.lg}"
    padding: "{spacing.xs}"
  tab:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.md}"
    padding: "{spacing.sm} {spacing.lg}"
  tab-active:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    borderColor: "{colors.border}"
    typography: "{typography.body}"
    rounded: "{rounded.md}"
    padding: "{spacing.sm} {spacing.lg}"
---

## Overview

This system uses a high-contrast monochrome interface with generous whitespace, large lightweight headings, pill-shaped controls, and softly rounded grouped surfaces. Content is arranged in a wide centered container with clear separation between navigation, introductory content, actions, and an interactive content panel.

## Colors

- **Primary:** Black, reserved for high-emphasis actions and selected controls.
- **On Primary:** White, used for content on primary controls.
- **Primary Hover:** Slightly lighter black for primary interaction feedback.
- **Background:** White page canvas and control background.
- **Foreground:** Black text and high-emphasis content.
- **Surface:** Warm off-white background for grouped content and inactive navigation areas.
- **On Surface:** Black content placed on surfaces.
- **Border:** Very light neutral gray used for outlines, separators, and subtle panel definition.

## Typography

Use the lightweight heading style for prominent introductory statements, with a compact line height and slightly negative tracking. Use the body style for descriptive text and actions. Navigation uses a smaller, regular-weight version of the body family with a comfortable line height.

## Layout

Use a wide centered content container with consistent horizontal page margins. Keep the primary navigation in a single horizontal row, with navigation links grouped separately from account actions.

Arrange introductory content as a two-column composition: a large heading and action group on the left, and supporting body copy on the right. Maintain generous vertical spacing between navigation, introductory content, actions, and the main content surface.

Use grouped content panels beneath the introductory region. Tab controls should span the panel width and distribute items horizontally, with the active item visually elevated inside the group.

## Elevation & Depth

Use very subtle gray borders and restrained inset or ambient shadows to separate white controls from the white canvas. Active controls and grouped surfaces should rely primarily on contrast, borders, and rounded shapes rather than pronounced shadows.

## Shapes

Use fully rounded pill shapes for buttons and compact interactive controls. Use a larger rounded radius for broad grouped surfaces and tab groups. Keep borders fine and low contrast, with no sharp decorative corners competing with the soft panel geometry.

## Components

- **page:** White canvas with black body text using {colors.background}, {colors.foreground}, and {typography.body}.
- **navigation:** Horizontal navigation treatment using {colors.background}, {colors.foreground}, and {typography.navigation}.
- **surface:** Warm off-white grouped panel using {colors.surface}, {colors.on-surface}, and {rounded.lg}.
- **border:** One-pixel structural separator using {colors.border} and {spacing.hairline}.
- **button-primary:** Black pill-shaped action with white text, using {colors.primary}, {colors.on-primary}, {typography.body}, {rounded.sm}, {spacing.sm}, and {spacing.lg}.
- **button-primary-hover:** Independent primary hover state using {colors.primary-hover} and {colors.on-primary}.
- **button-secondary:** White outlined pill-shaped action using {colors.background}, {colors.foreground}, {colors.border}, {typography.body}, {rounded.sm}, {spacing.sm}, and {spacing.lg}.
- **button-secondary-hover:** Independent secondary hover state using {colors.surface}, {colors.foreground}, and {colors.border}.
- **heading:** Large lightweight heading using {colors.foreground} and {typography.heading}.
- **tab-group:** Rounded surface for a horizontal set of tabs using {colors.surface}, {colors.on-surface}, {colors.border}, {rounded.lg}, and {spacing.xs}.
- **tab:** Inactive tab using {colors.surface}, {colors.on-surface}, {typography.body}, {rounded.md}, {spacing.sm}, and {spacing.lg}.
- **tab-active:** White selected tab with a subtle border using {colors.background}, {colors.foreground}, {colors.border}, {typography.body}, {rounded.md}, {spacing.sm}, and {spacing.lg}.

## Do's and Don'ts

### Do

- Use black and white contrast to establish interaction priority.
- Keep headings large, lightweight, and tightly set.
- Preserve generous whitespace around introductory content.
- Use pill-shaped actions and softly rounded grouped surfaces.
- Use borders and restrained shadows to distinguish adjacent white elements.
- Keep component states as separate entries and reference tokens consistently.
- Maintain WCAG AA contrast for text and interactive controls.

### Don't

- Do not introduce saturated colors into the primary interface hierarchy.
- Do not use sharp corners for buttons, tabs, or broad grouped surfaces.
- Do not rely on heavy shadows to create hierarchy.
- Do not compress the navigation and introductory layout into a dense arrangement.
- Do not hardcode visual values inside component definitions.
- Do not nest hover or other interaction states inside a base component.
