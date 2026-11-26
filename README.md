# DESIGN.md Auditor (lite)

A free Claude skill. You paste your `DESIGN.md` and some code (CSS, HTML, JSX). Claude lists the colors and fonts in the code that are not in your DESIGN.md, with the closest token and the fix.

AI site builders (Lovable, Cursor, v0) often ignore the design system you gave them. This is a quick way to see how far the code drifted.

## Use it

1. Copy `SKILL.md` into your Claude skills folder as `design-md-auditor-lite/SKILL.md`.
2. In Claude, paste your DESIGN.md and the code, and ask: "Audit this against my DESIGN.md".
3. You get a short list: line, value found, closest token, replacement.

## What lite does not do

- Checks colors and fonts only. No radii, spacing or Tailwind classes.
- No script, no whole-repo scan, no score. Claude reads what you paste.
- It cannot judge how a page looks, only whether the code disagrees with your DESIGN.md.

## Full version

The full Auditor adds a Python script (no dependencies) that scans a whole project: colors, fonts, border radii, padding, margin and gap, Tailwind arbitrary values, plus a 0-100 consistency score and the most repeated fixes.

https://ia.cuadrantia.store/auditor

Made by [Cuadrantia](https://ia.cuadrantia.store). Questions: hola@cuadrantia.store

License: MIT.
