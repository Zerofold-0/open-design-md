---
version: "alpha"
name: "Agentic Skills Design System"
colors:
  primary: "#0A0A0A"
  on-primary: "#FFFFFF"
  primary-hover: "#262626"
  background: "#FFFFFF"
  foreground: "#0A0A0A"
  surface: "#FAFAFA"
  on-surface: "#0A0A0A"
  border: "#E1E1E1"
  grid: "#EAEAEA"
  muted: "#666666"
  dark-surface: "#0A0A0A"
  on-dark: "#FFFFFF"
typography:
  heading:
    fontFamily: "sans-serif"
    fontSize: "72px"
    fontWeight: "500"
    lineHeight: "67.68px"
    letterSpacing: "-2.52px"
  body:
    fontFamily: "sans-serif"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "24px"
  label:
    fontFamily: "monospace"
    fontSize: "14px"
    fontWeight: "400"
    lineHeight: "20px"
    letterSpacing: "2.1px"
  terminal:
    fontFamily: "monospace"
    fontSize: "14px"
    fontWeight: "400"
    lineHeight: "24px"
  display-italic:
    fontFamily: "serif"
    fontSize: "72px"
    fontWeight: "400"
    lineHeight: "67.68px"
    letterSpacing: "-2.52px"
rounded:
  sm: "0px"
  md: "0px"
  lg: "0px"
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
  grid-background:
    backgroundColor: "{colors.grid}"
    textColor: "{colors.foreground}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.md}"
  border:
    backgroundColor: "{colors.border}"
    height: "1px"
  muted-label:
    backgroundColor: "{colors.background}"
    textColor: "{colors.muted}"
    typography: "{typography.label}"
  heading:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  display-italic:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.display-italic}"
  body-copy:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
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
  button-secondary:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
    borderColor: "{colors.foreground}"
  search-control:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.muted}"
    typography: "{typography.terminal}"
    rounded: "{rounded.sm}"
    borderColor: "{colors.border}"
  announcement:
    backgroundColor: "{colors.dark-surface}"
    textColor: "{colors.on-dark}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    padding: "{spacing.lg}"
  terminal-panel:
    backgroundColor: "{colors.dark-surface}"
    textColor: "{colors.on-dark}"
    typography: "{typography.terminal}"
    rounded: "{rounded.sm}"
    padding: "{spacing.lg}"
  stat-strip:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    rounded: "{rounded.sm}"
    borderColor: "{colors.border}"
---

## Overview

This design system defines a stark editorial interface built from a white canvas, black structural panels, thin gray rules, a visible square grid, oversized typography, and precise monospaced labels. The layout uses a wide centered container with a split introductory area, compact navigation, prominent rectangular actions, and grouped metrics.

## Colors

- **Primary:** Near-black, reserved for high-emphasis actions and strong structural panels.
- **On Primary:** White content placed on primary controls.
- **Primary Hover:** Slightly lighter black for interactive feedback.
- **Background:** White page canvas.
- **Foreground:** Near-black primary text.
- **Surface:** Very light neutral fill for controls and grouped areas.
- **On Surface:** Near-black content on light surfaces.
- **Border:** Thin neutral rules around controls and structural groups.
- **Grid:** Very light neutral lines forming the background grid.
- **Muted:** Medium gray for metadata, labels, prompts, and secondary information.
- **Dark Surface:** Near-black panels such as announcements and terminal-style demonstrations.
- **On Dark:** White content on dark panels.

## Typography

Use a clean sans-serif for headings and body copy. Headings are large, medium-weight, tightly tracked, and compact in line height. Emphasized display words may use a contrasting italic serif treatment. Use a monospaced face for uppercase metadata, counters, command-line content, and compact interface labels. Keep labels visibly tracked and secondary to the large editorial heading.

## Layout

Use a wide centered content container with generous horizontal margins. Keep the top utility bar and primary navigation compact, with navigation links centered between the identity area and utility controls.

Place announcement content in a full-width dark horizontal panel near the top of the content area. Use the main introductory section as a two-column layout: text and actions on the left, with a dark terminal-style demonstration panel on the right. Align the lower metric strip to the same container and divide it into evenly spaced columns with thin rules. Use the square grid as a subtle page backdrop behind the main introductory content.

Apply generous vertical spacing between the announcement, introductory label, heading, supporting copy, actions, and metrics. Preserve rectangular alignment and avoid excessive inset decoration.

## Elevation & Depth

The interface is intentionally flat. Use contrast between white space, black panels, thin borders, and the background grid to establish hierarchy rather than shadows. Do not add drop shadows or floating-card elevation unless a control requires a clearly visible interaction state.

## Shapes

Use square corners throughout the primary layout, controls, panels, announcement area, and metric strip. Keep borders thin and precise. Avoid pill-shaped controls and rounded cards.

## Components

- **page:** White canvas with near-black body text.
- **grid-background:** Very light grid color used as a repeating structural backdrop.
- **surface:** Nearly white grouped area with near-black content and square corners.
- **border:** One-pixel neutral divider or outline.
- **muted-label:** Monospaced, tracked metadata in medium gray.
- **heading:** Large, tightly tracked sans-serif display heading.
- **display-italic:** Contrasting italic serif treatment for selective display emphasis.
- **body-copy:** Comfortable sans-serif supporting text with a relaxed line height.
- **button-primary:** Black rectangular action with white text and consistent internal spacing.
- **button-primary-hover:** Slightly lighter black hover state with white text.
- **button-secondary:** White rectangular action with near-black text and a near-black outline.
- **search-control:** Light control with muted monospaced prompt text and a thin neutral border.
- **announcement:** High-contrast dark horizontal notice with white content.
- **terminal-panel:** Dark demonstration panel using white monospaced content and generous inset spacing.
- **stat-strip:** Bordered horizontal metric group with strong values and tracked supporting labels.

## Do's and Don'ts

### Do

- Reference design values through tokens such as {colors.primary}.
- Use thin rules, square corners, and strong black-and-white contrast.
- Keep supporting labels monospaced, tracked, and visually subordinate.
- Use the grid sparingly so it supports alignment without overpowering content.
- Maintain WCAG AA contrast for text and interactive controls.
- Preserve separate hover-state entries rather than nesting states.

### Don't

- Do not hardcode captured colors inside component definitions.
- Do not use pill-shaped buttons or rounded promotional cards.
- Do not introduce shadows that compete with the flat geometric hierarchy.
- Do not overuse the dark surface outside strong banners or demonstration panels.
- Do not nest hover, active, or pressed variants inside a base component.
- Do not add page-specific copy, names, or source-specific content to the system.
