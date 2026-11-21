# Focused passes

A pass is a narrow edit with one goal. A verdict lists at most two passes per screen, and the design skill runs them while the critic stays read-only. A pass leaves behaviour, copy meaning, tokens and accessibility as they are, and the screen is shot again at 390x844 and 1440x900 afterwards.

| Pass | Suits findings of | Typical changes | Not included |
|---|---|---|---|
| bolder | flat, generic, no focal point | one stronger focal element (size, weight, colour role), wider contrast between levels, the signature detail from `DESIGN.md` | new colours, gradients, decoration |
| quieter | busy, loud, everything competes | fewer borders and shadows that carry no meaning, merged duplicate labels, lighter secondary weight, more space | hiding actions the task needs |
| typeset | weak text hierarchy, uneven rhythm | text mapped to theme.json font-size presets, tuned line height and width, tabular figures for numbers | a third font family |
| layout | misalignment, cramped or empty areas, breaks at a width | grid alignment, spacing on the preset scale, rechecks at 390 and 1440 | changing navigation without the plan |
| polish | ready but rough | states (hover, focus, active, disabled), motion tokens, truncation, empty and error copy | starting before Critical and Important findings are fixed |

Usual order when several apply: layout, typeset, quieter or bolder (never both on one screen), polish last.
