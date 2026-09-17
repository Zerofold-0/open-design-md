---
version: "alpha"
name: "xAI Dark Design System"
colors:
  primary: "#FFFFFF"
  on-primary: "#0A0A0A"
  primary-hover: "#E6E6E6"
  background: "#080808"
  foreground: "#FFFFFF"
  surface: "#171717"
  on-surface: "#FFFFFF"
  border: "#292929"
  muted: "#A0A0A0"
typography:
  heading:
    fontFamily: "universalSansDisplay"
    fontSize: "60px"
    fontWeight: "500"
    lineHeight: "60px"
    letterSpacing: "-1.5px"
  body:
    fontFamily: "universalSans"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
    letterSpacing: "0px"
  navigation:
    fontFamily: "universalSans"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
    letterSpacing: "0px"
rounded:
  sm: "9999px"
  md: "28px"
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
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    padding: "{spacing.lg}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
    padding: "{spacing.xl}"
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
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-secondary-hover:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
  heading:
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  navigation-link:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.navigation}"
  footer:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.body}"
    padding: "{spacing.xxl}"
  footer-heading:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  support-control:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
---

## Overview

This design system describes a dark, spacious interface with a persistent top navigation, high-contrast pill-shaped actions, grouped content surfaces, and a multi-column footer. It excludes source-specific names, copy, imagery, and other identifying content.

## Colors

- **Background:** Near-black page canvas used across the header and footer.
- **Foreground:** Bright white for primary text and high-emphasis controls.
- **Surface:** Slightly lighter charcoal for cards and grouped content.
- **Primary:** White action background for the highest-emphasis buttons.
- **On Primary:** Near-black text placed on primary actions.
- **Muted:** Gray text for navigation, secondary links, and supporting information.
- **Border:** Subtle dark gray used for separators and outlined controls.
- **Primary Hover:** Slightly softened white for hovered primary actions.

## Typography

Use the display sans-serif style for large headings and the regular sans-serif style for navigation, body copy, links, and controls. Body text uses a compact 16px size with a 24px line height. Navigation and footer content remain restrained in size and weight, with muted text providing hierarchy against the dark canvas.

## Layout

Use generous horizontal margins and broad content bands. Keep primary navigation in a single horizontal row with links grouped separately from right-aligned actions. Arrange grouped content in large rounded surfaces with consistent internal padding. Use a full-width divider before the footer, then organize footer content into multiple vertical link columns with a distinct identity or utility area separated by a vertical rule. Preserve large open areas between major sections.

## Elevation & Depth

The interface relies on tonal separation rather than pronounced shadows. Use the surface color to distinguish cards from the page background, and use a subtle one-pixel border for separators and outlined controls. Avoid heavy drop shadows.

## Shapes

Use fully rounded pill shapes for buttons, compact controls, and utility elements. Use a larger consistent radius for cards and grouped surfaces. Keep dividers square and one pixel thick.

## Components

- **header:** Persistent dark navigation band with muted links and high-contrast action controls.
- **navigation-link:** Low-emphasis navigation item using {colors.muted} on {colors.background}.
- **surface:** Rounded grouped content area using {colors.surface} and {colors.on-surface}.
- **button-primary:** High-emphasis pill action using {colors.primary} with {colors.on-primary} text.
- **button-primary-hover:** Independent hover state using {colors.primary-hover} with {colors.on-primary} text.
- **button-secondary:** Outlined or low-emphasis pill action using {colors.surface} with {colors.foreground} text.
- **button-secondary-hover:** Independent hover state using {colors.background} with {colors.foreground} text.
- **border:** One-pixel structural separator using {colors.border}.
- **footer:** Spacious multi-column footer using {colors.background} with {colors.muted} text.
- **footer-heading:** Higher-emphasis footer label using {colors.foreground} on {colors.background}.
- **support-control:** Small fixed utility control using {colors.background} with {colors.foreground} text.

## Do's and Don'ts

### Do

- Use near-black backgrounds and subtle charcoal surfaces to establish depth.
- Reserve bright white backgrounds for primary actions and high-emphasis controls.
- Use pill-shaped controls consistently.
- Maintain generous spacing between content groups and footer columns.
- Keep secondary navigation and footer links visibly muted.
- Reference design values through tokens such as {colors.primary}.
- Maintain WCAG AA contrast for all text and interactive controls.

### Don't

- Do not introduce colorful accents that are not present in the captured interface.
- Do not use heavy shadows or strong gradients.
- Do not mix sharp-cornered controls with the rounded interaction language.
- Do not hardcode captured colors inside component definitions.
- Do not nest hover or other interaction states inside a base component.
- Do not add source-specific names, copy, imagery, or page content.
