---
version: "alpha"
name: "Zapier Design System"
colors:
  primary: "#FF4F00"
  on-primary: "#201515"
  primary-hover: "#D83F00"
  background: "#FFFDF9"
  foreground: "#201515"
  surface: "#30342D"
  on-surface: "#FFFFFF"
  media-background: "#9BAAC8"
  border: "#D9D6D0"
typography:
  heading:
    fontFamily: "Degular Display"
    fontSize: "72px"
    fontWeight: "400"
    lineHeight: "1.05"
    letterSpacing: "-0.02em"
  body:
    fontFamily: "Inter"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "1.5"
    letterSpacing: "0em"
  navigation:
    fontFamily: "Inter"
    fontSize: "16px"
    fontWeight: "400"
    lineHeight: "1.5"
    letterSpacing: "0em"
rounded:
  sm: "4px"
  md: "0px"
  lg: "999px"
spacing:
  xs: "4px"
  sm: "8px"
  md: "16px"
  lg: "24px"
  xl: "32px"
  xxl: "48px"
  section: "64px"
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
    borderColor: "{colors.border}"
  navigation:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.navigation}"
    gap: "{spacing.xl}"
  hero-banner:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    padding: "{spacing.xxl}"
  hero-content:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
    padding: "{spacing.section}"
  heading:
    textColor: "{colors.foreground}"
    typography: "{typography.heading}"
  body:
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
  button-primary:
    backgroundColor: "{colors.primary}"
    textColor: "{colors.on-primary}"
    typography: "{typography.body}"
    rounded: "{rounded.lg}"
    padding: "{spacing.sm}"
  button-primary-hover:
    backgroundColor: "{colors.primary-hover}"
    textColor: "{colors.on-surface}"
    typography: "{typography.body}"
    rounded: "{rounded.lg}"
    padding: "{spacing.sm}"
  tab-list:
    backgroundColor: "{colors.background}"
    textColor: "{colors.foreground}"
    typography: "{typography.body}"
    borderColor: "{colors.border}"
  media-panel:
    backgroundColor: "{colors.media-background}"
    textColor: "{colors.foreground}"
    padding: "{spacing.xxl}"
  surface:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.on-surface}"
    rounded: "{rounded.sm}"
  border:
    backgroundColor: "{colors.border}"
    textColor: "{colors.foreground}"
    height: "1px"
---

## Overview

This design system describes a high-contrast, editorial interface with a warm near-white canvas, a dark horizontal banner, bright orange actions, generous centered hero content, and framed tabular navigation. Layouts use wide containers, clear section spacing, and large visual media areas.

## Colors

- **Primary:** Bright orange for high-emphasis actions and selective text emphasis.
- **On Primary:** Deep brown-black for readable content on the bright primary color.
- **Primary Hover:** Darker orange for interactive emphasis while retaining the warm accent.
- **Background:** Warm near-white page canvas.
- **Foreground:** Deep brown-black for primary text and icons.
- **Surface:** Deep muted green-black for full-width banners and dark grouped areas.
- **On Surface:** White for content placed on dark surfaces.
- **Media Background:** Muted periwinkle blue for large visual media or preview panels.
- **Border:** Soft warm gray for dividers, tab boundaries, and light framing.

## Typography

Use a display sans-serif with a light-to-regular weight for large editorial headings. Headings are oversized, tightly spaced, and centered where used in hero content. Use Inter for body copy, navigation, labels, and controls. Keep supporting text smaller and comfortably line-spaced beneath prominent headings.

## Layout

Use a full-width header with horizontally distributed navigation and actions. Follow it with a shallow dark banner, then a spacious centered hero section. Constrain readable text to a wide but finite measure rather than stretching lines across the viewport. Place horizontal tab navigation below the hero copy, using equal-height cells and visible vertical dividers. Large media panels should align to a broad content container and retain generous surrounding whitespace.

Use the spacing scale for header padding, navigation gaps, hero separation, tab dimensions, and media-panel insets. Preserve the responsive horizontal flow and allow navigation and tab cells to wrap or scroll when the viewport is narrower.

## Elevation & Depth

The interface relies primarily on color blocking, borders, and spacing rather than pronounced shadows. Use the dark banner and blue media panel as visual depth layers. Keep surfaces visually flat unless a control or preview requires a subtle separation from its surrounding canvas.

## Shapes

Use square or nearly square corners for tabs, media framing, banners, and structural surfaces. Use a fully rounded pill shape for prominent action buttons. Keep borders thin and understated, and avoid adding rounded cards where the layout is intended to feel editorial and architectural.

## Components

- **header:** Warm canvas header with deep text, compact vertical padding, and a subtle bottom border.
- **navigation:** Horizontal navigation using the body scale, generous gaps, and high-contrast foreground text.
- **hero-banner:** Full-width dark banner with white content and generous internal spacing.
- **hero-content:** Spacious warm canvas section for large centered display text.
- **heading:** Large display typography in the foreground color.
- **body:** Regular supporting copy in the foreground color.
- **button-primary:** Bright orange pill action with deep text for accessible contrast.
- **button-primary-hover:** Darker orange pill action with white text for a distinct hover state.
- **tab-list:** Bordered horizontal navigation row with warm background, dark labels, and cell dividers.
- **media-panel:** Wide muted-blue visual region with deep foreground content and generous inset spacing.
- **surface:** Dark grouped region with white content and minimal rounding.
- **border:** Thin warm-gray structural separator.

## Do's and Don'ts

### Do

- Use the warm near-white canvas as the dominant page background.
- Reserve the dark surface for broad banners and strong visual bands.
- Use orange sparingly for actions and emphasis.
- Keep hero headings large, light, tightly spaced, and centered when used in a landing layout.
- Use borders and spacing to define tabs and content regions.
- Reference all visual values through tokens such as {colors.primary} and {spacing.lg}.

### Don't

- Do not use purple as the primary action color.
- Do not add heavy shadows or highly rounded cards to flat editorial sections.
- Do not make every element orange or dark; preserve the warm canvas and muted media contrast.
- Do not hardcode captured colors or dimensions inside component definitions.
- Do not nest hover or other interaction states inside a base component.
