# Nothing Design Skill

A design system skill adapted for Codex/OpenAI-style coding agents, inspired by Nothing's visual language. Monochrome, typographic, industrial.

I kept describing the same design rules over and over — Swiss typography, OLED blacks, segmented progress bars, dot-matrix motifs. So I packaged it into a reusable skill.

![Preview](preview.gif)

## What you get

Tell the agent to use "Nothing style" or apply the Nothing design system and it will generate UI following these principles:

- Three-layer visual hierarchy (display, body, metadata — that's it)
- Space Grotesk + Space Mono + Doto font stack
- Full dark and light mode token system
- Segmented progress bars, mechanical toggles, instrument-style widgets
- Output as HTML/CSS, SwiftUI, or React/Tailwind

## Install

Copy the `nothing-design` folder into your Codex skills/instructions directory or reuse `nothing-design/SKILL.md` as a project instruction file, depending on your Codex setup.

## What's inside

| File | |
|------|---|
| `nothing-design/SKILL.md` | Design philosophy, craft rules, workflow |
| `nothing-design/references/tokens.md` | Colors, fonts, spacing, motion tokens |
| `nothing-design/references/components.md` | Buttons, cards, lists, tables, overlays |
| `nothing-design/references/platform-mapping.md` | CSS, SwiftUI, React output mappings |

## Notes for Codex

This repository was originally written for Claude Code. The skill frontmatter and instructions have been rewritten so the core prompt can be pasted into Codex-compatible instruction files without Claude-specific tool declarations or slash-command assumptions.

## License

MIT
