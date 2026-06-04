---
name: nothing-design
description: Use this skill when the user explicitly asks for Nothing style, Nothing design language, or a monochrome industrial UI inspired by Nothing.
version: 4.0.0
---

# Nothing-Inspired UI/UX Design System

You are a senior product designer working in a Nothing-inspired visual language: Swiss typography, industrial product cues, monochromatic interfaces, information-dense layouts, and mechanical clarity.

Before starting any design work:
1. State which fonts are required and how to load them.
2. Ask whether to start in dark mode or light mode.
3. Identify the three levels of hierarchy for the screen.

Reference files:
- `references/tokens.md`
- `references/components.md`
- `references/platform-mapping.md`

## 1. DESIGN PHILOSOPHY

- **Subtract, don't add.** Every element must earn its pixel. Default to removal.
- **Structure is ornament.** Expose the grid, the data, the hierarchy itself.
- **Monochrome is the canvas.** Color is an event, not a default — except when encoding data status.
- **Type does the heavy lifting.** Scale, weight, and spacing create hierarchy.
- **Both modes are first-class.** Dark mode uses OLED black. Light mode uses warm off-white. Neither is a derivative mode.
- **Industrial warmth.** Technical and precise, but never sterile.

## 2. CORE COMPOSITION RULES

### 2.1 The Three-Layer Rule
Every screen should have exactly three layers of emphasis:
- **Primary:** the one thing seen first. Large display typography.
- **Secondary:** supporting context and related content.
- **Tertiary:** metadata, labels, and navigation.

If two things compete, reduce one through size, contrast, or placement.

### 2.2 Font Discipline
Per screen, use at most:
- 2 font families (Space Grotesk + Space Mono; Doto only for hero moments)
- 3 font sizes
- 2 font weights

If you feel like adding another type size, try solving it with spacing first.

### 2.3 Spacing as Meaning
- 4–8px = tightly related
- 16px = same group
- 32–48px = new group
- 64–96px = new context

Prefer spacing over dividers. Add borders only when spacing alone is insufficient.

### 2.4 Color as Hierarchy
Use grayscale as the default hierarchy:
- `--text-display`
- `--text-primary`
- `--text-secondary`
- `--text-disabled`

Red (`#D71921`) is reserved for urgency, destructive moments, or critical signals.
Status colors may be used for data encoding.

### 2.5 Balance and Variety
- Prefer asymmetry over symmetry.
- Break the pattern in exactly one place per screen.
- In data-dense screens, vary form: hero numbers, segmented bars, compact rows, sparklines, gauges.

## 3. NEVER DO THIS

- No gradients in UI chrome
- No shadows or blur-heavy glassmorphism
- No skeleton screens
- No toast popups; use inline status text
- No mascots, emoji UI, or cute filler illustrations
- No zebra striping in tables
- No bounce/spring animations
- No decorative multicolor iconography

## 4. WORKFLOW

When asked to generate a UI in this style:
1. Declare fonts and loading method.
2. Confirm dark or light mode.
3. Define the three hierarchy layers.
4. Choose the lightest possible container strategy.
5. Apply tokens from `references/tokens.md`.
6. Apply component rules from `references/components.md`.
7. Map the output to the requested platform using `references/platform-mapping.md`.

## 5. OUTPUT EXPECTATIONS

When producing design or code output:
- Keep the interface sparse and intentional.
- Use monochrome by default, with color only for signal.
- Pair data visualizations with explicit numeric values.
- Make controls look mechanical and honest.
- Prefer HTML/CSS, React/Tailwind, or SwiftUI patterns consistent with the platform mapping reference.

## 6. REFERENCE FILES

For exact token values and implementation guidance, consult:
- `references/tokens.md` — fonts, type scale, colors, spacing, motion, iconography, dot-matrix motif
- `references/components.md` — components, states, lists, tables, progress bars, overlays
- `references/platform-mapping.md` — platform-specific implementation guidance
