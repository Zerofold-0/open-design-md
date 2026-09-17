---
version: "alpha"
name: "Claude Design System"
omitted:
  - "Source-specific labels, copy, logos, illustrations, imagery, and personal data"
colors:
  primary: "#141413"
  on-primary: "#FFFFFF"
  primary-hover: "#2A2927"
  background: "#FAF9F5"
  foreground: "#141413"
  surface: "#FFFFFF"
  on-surface: "#141413"
  border: "#E5E3DC"
  muted: "#625F5B"
  accent: "#D97757"
  on-accent: "#141413"
  accent-hover: "#C9684C"
typography:
  display:
    fontFamily: "serif"
    fontSize: "72px"
    fontWeight: "400"
    lineHeight: "1.08"
    letterSpacing: "-0.03em"
  heading:
    fontFamily: "serif"
    fontSize: "48px"
    fontWeight: "400"
    lineHeight: "1.1"
    letterSpacing: "-0.025em"
  body:
    fontFamily: "sans-serif"
    fontSize: "20px"
    fontWeight: "400"
    lineHeight: "1.6"
    letterSpacing: "0em"
  navigation:
    fontFamily: "sans-serif"
    fontSize: "18px"
    fontWeight: "400"
    lineHeight: "1.4"
    letterSpacing: "0em"
  control:
    fontFamily: "sans-serif"
    fontSize: "18px"
    fontWeight: "500"
    lineHeight: "1.4"
    letterSpacing: "0em"
rounded:
  xs: "8px"
  sm: "12px"
  md: "16px"
  lg: "32px"
spacing:
  hairline: "1px"
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  panel: "64px"
  hero: "96px"
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
    textColor: "{colors.muted}"
    typography: "{typography.navigation}"
    padding: "{spacing.xl}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.lg}"
  content-panel:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.lg}"
    padding: "{spacing.panel}"
  heading:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    typography: "{typography.display}"
  section-heading:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  input:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.muted}"
    typography: "{typography.body}"
    rounded: "{rounded.md}"
    padding: "{spacing.md}"
    borderColor: "{colors.border}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.control}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-primary}"
    typography: "{typography.control}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-accent:
    backgroundColor: "{colors.accent}"
    textColor: "{colors.on-accent}"
    typography: "{typography.control}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  button-accent-hover:
    backgroundColor: "{colors.accent-hover}"
    textColor: "{colors.on-accent}"
    typography: "{typography.control}"
    rounded: "{rounded.sm}"
    padding: "{spacing.md}"
  notification-panel:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.foreground}"
    rounded: "{rounded.md}"
    padding: "{spacing.lg}"
  support-control:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    rounded: "{rounded.lg}"
  border:
    backgroundColor: "{colors.border}"
    height: "{spacing.hairline}"
---

## Overview

This design system captures a spacious, editorial interface with a warm off-white canvas, white rounded surfaces, dark serif display typography, restrained sans-serif navigation, and high-contrast actions. Layouts use broad horizontal margins, generous vertical whitespace, and clear separation between navigation, content panels, and floating utilities.

## Colors

- **Primary:** Near-black color for high-emphasis actions and controls.
- **On Primary:** Light content color for use on primary surfaces.
- **Primary Hover:** Slightly lighter near-black interaction state.
- **Background:** Warm off-white page canvas.
- **Foreground:** Near-black high-emphasis text.
- **Surface:** White content and utility surfaces.
- **On Surface:** Foreground color for content on white surfaces.
- **Border:** Very light warm-gray outlines and separators.
- **Muted:** Soft dark gray for secondary navigation and supporting text.
- **Accent:** Warm terracotta action color.
- **On Accent:** Dark content color selected for accessible contrast on accent surfaces.
- **Accent Hover:** Darker terracotta interaction state.

## Typography

Use a serif family for large display and section headings, with a sans-serif family for navigation, controls, and supporting text. Display headings are large, relaxed, and slightly tracked inward. Body and navigation text remain highly legible with generous line height.

## Layout

Use a full-width warm off-white canvas with horizontal navigation bands separated by thin rules. Keep primary content inside a wide rounded white panel with generous internal padding. Favor two-column arrangements at large widths, placing prominent heading content beside a compact input-and-action control. Preserve substantial open space between major sections and allow the layout to collapse into a vertical flow on smaller screens.

## Elevation & Depth

Surfaces are primarily distinguished through white-on-warm-background contrast and subtle warm-gray outlines. Use a restrained soft shadow for floating notification panels and detached utility controls; avoid strong or extensive shadows on the main content panel.

## Shapes

Use large rounded corners for primary content panels and floating utility surfaces. Use medium rounding for inputs and compact rounding for buttons. Keep borders thin and understated, with simple geometric controls and minimal ornamentation.

## Components

- **page:** Full-width warm canvas using {colors.background}, {colors.foreground}, and {typography.body}.
- **header:** Spacious primary navigation band using {colors.background}, {colors.foreground}, and {typography.navigation}.
- **navigation:** Secondary navigation band using {colors.background}, {colors.muted}, and {typography.navigation}.
- **surface:** White rounded grouping surface using {colors.surface}, {colors.on-surface}, and {rounded.lg}.
- **content-panel:** Large rounded white container using {colors.surface}, {colors.foreground}, {rounded.lg}, and {spacing.panel}.
- **heading:** Large serif display treatment using {colors.surface}, {colors.foreground}, and {typography.display}.
- **section-heading:** Serif section title using {colors.background}, {colors.foreground}, and {typography.heading}.
- **input:** White bordered input treatment using {colors.surface}, {colors.muted}, {colors.border}, {rounded.md}, and {spacing.md}.
- **button-primary:** Dark high-emphasis action using {colors.primary}, {colors.on-primary}, {typography.control}, {rounded.sm}, and {spacing.md}.
- **button-primary-hover:** Hover state using {colors.primary-hover} and {colors.on-primary}.
- **button-accent:** Terracotta emphasis action using {colors.accent}, {colors.on-accent}, {typography.control}, {rounded.sm}, and {spacing.md}.
- **button-accent-hover:** Hover state using {colors.accent-hover} and {colors.on-accent}.
- **notification-panel:** Floating informational surface using {colors.surface}, {colors.foreground}, {rounded.md}, and {spacing.lg}.
- **support-control:** Detached rounded utility control using {colors.primary}, {colors.on-primary}, and {rounded.lg}.
- **border:** One-pixel structural separator using {colors.border} and {spacing.hairline}.

## Do's and Don'ts

### Do

- Use tokens such as {colors.primary} and {spacing.xl} instead of repeating visual values.
- Preserve the warm neutral canvas and strong white-surface contrast.
- Use serif typography for prominent headings and sans-serif typography for navigation and controls.
- Keep primary actions visually distinct through dark or terracotta fills and accessible text contrast.
- Maintain generous whitespace, broad margins, thin separators, and subtle depth.
- Keep hover, focus, active, disabled, loading, error, and empty states visually consistent with the same restrained system.

### Don't

- Do not hardcode captured colors inside component definitions.
- Do not introduce saturated colors, heavy shadows, or sharp square containers.
- Do not use display typography for dense navigation or form controls.
- Do not nest hover, active, or pressed variants inside a base component.
- Do not add source-specific labels, copy, logos, imagery, or page content to reusable patterns.
