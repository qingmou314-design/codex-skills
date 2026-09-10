---
name: beautiful-html-templates
description: Build or restyle design-led HTML slide decks using a curated library of 34 complete templates. Use for web-based presentations and standalone HTML decks; do not use when the required deliverable is PPTX or Google Slides.
---

# Beautiful HTML Templates

Use the bundled template library as a visual system, not as loose inspiration.

## Library

- Template catalog: `assets/library/index.json`
- Template files: `assets/library/templates/<slug>/`
- Shared runtime: `assets/library/runtime/deck-stage.js`
- Detailed upstream workflow: `references/upstream-agent-guide.md`

Never edit the installed library in place. Copy the selected template and any
required sibling assets into the user's project workspace before adapting it.

## Workflow

1. Establish the deck's occasion, audience, topic, and desired mood. Ask a short
   question only when those signals are missing or genuinely ambiguous.
2. Read `assets/library/index.json`. Match the brief against `mood`, `tone`,
   `best_for`, `formality`, `density`, and `scheme`; treat `occasion` as a soft
   signal. Shortlist three visually distinct candidates when the user has not
   already chosen a template.
3. Read only the shortlisted templates. Create one real-content cover preview
   for each candidate, keeping its fonts, palette, decorations, and runtime.
   Present the previews and let the user choose before building the full deck.
4. Copy the chosen template folder into the working project and replace all
   placeholder text, numbers, names, dates, and images with the user's content.
5. Add or remove slides as needed. New layouts must use the chosen template's
   existing fonts, colors, spacing rhythm, decorative vocabulary, components,
   chrome, and navigation behavior. Do not mix visual systems from other
   templates.
6. Open previews and the final HTML in an available browser, verify navigation
   and visual fit, then provide the absolute output path.

Read `references/upstream-agent-guide.md` before building a complete deck. It
contains the detailed matching fields, adaptation rules, and layout-extension
guidance. Adapt platform-specific commands to the current environment rather
than assuming macOS shell commands are available.

## Source

Adapted for Codex from
[`zarazhangrui/beautiful-html-templates`](https://github.com/zarazhangrui/beautiful-html-templates).
The bundled library is provided under its upstream MIT license.
