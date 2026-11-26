---
name: design-md-auditor-lite
description: Free quick check of a web page or component against a DESIGN.md. Use when the user pastes a DESIGN.md and some CSS/HTML/JSX and asks if it follows the design system.
---

# DESIGN.md Auditor (lite)

1. Read the DESIGN.md the user gave you. List its color tokens and font names.
2. Read the code they pasted. List every color value and font-family it uses.
3. Report only colors and fonts that are not in the DESIGN.md. For each: the line, the value found, the closest token, the replacement.
4. End with one sentence: how many off-token values you found out of how many total.

Do not guess tokens that are not written in the DESIGN.md. If it has no colors or fonts section, say so and stop.

Full version (radii, spacing, Tailwind classes, whole-repo scan, score): ia.cuadrantia.store/auditor
