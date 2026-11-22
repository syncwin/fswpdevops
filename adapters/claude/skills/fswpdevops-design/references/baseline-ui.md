# Baseline UI rules (WordPress)

Hard rules every template, block and admin screen meets before critique. Each line is checkable in code or a screenshot. Accessibility rules live in `fswpdevops/references/accessibility.md`; token mechanics in `fswpdevops-theme`.

## Type and figures
- Numbers that change or line up (prices, counts, tables) use tabular figures: `font-variant-numeric: tabular-nums` set once in a theme.json style, not per element.
- Leave letter spacing at the theme's values; no negative letter spacing on body or labels.
- Loading text ends with an ellipsis character; units keep a non-breaking space to their number.
- Body line height about 1.4 to 1.6; readable width capped (about 70 characters, or the theme's content size).
- Truncation is a choice: line clamp plus the full text reachable (a title attribute is not enough; link to the full item).

## Actions and dialogs
- Destructive or irreversible actions name the object and the consequence and default to the safe button, or offer undo in a notice. Never a silent delete. In admin use core Modal or confirm patterns.
- Buttons show a busy state and block double submit while work runs.
- One primary button per view; others secondary or link style.

## Interaction (web a11y)
- Visible focus on every interactive element (theme.json focus style); never `outline: none` without a replacement.
- Toggles use a real checkbox or `role="switch"` with `aria-checked`; related inputs use fieldset and legend.
- Every field has a visible label tied by `for` and `id`, and error text linked with `aria-describedby`.
- Touch targets at least 24 CSS px (aim for 44) with spacing that prevents mis-taps.
- Links navigate, buttons act; never a clickable div.

## Motion
- Durations from tokens; feedback at most about 200 ms, larger transitions up to about 400 ms; ease-out on entry.
- Looping or auto-playing motion pauses off-screen, offers a pause control past a few seconds, and honours `prefers-reduced-motion`.
- Animate opacity and transform, not layout properties; nothing blocks input.

## Layout and states
- Spacing from the preset step scale only; reserve image and embed space so layout stays stable while loading.
- Empty, error, no-results and 404 states are designed, per `design-language.md`.
