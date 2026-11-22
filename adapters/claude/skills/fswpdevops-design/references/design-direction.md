# Design direction (plan before code)

Write the direction before the first template or block. The plan and the project's `DESIGN.md` (project root, master file) win; this fills only what they leave open. Brand colours or fonts the owner gave are never replaced.

## The plan (one short block in the scratchpad or `DESIGN.md`)
| Item | Decide | WordPress home |
|---|---|---|
| Purpose and tone | who uses it, in what mood, one adjective pair | plan |
| Colours | 4 to 6 roles: base, contrast, one primary, one accent at most, neutrals, error; each with a reason | `settings.color.palette` by role slug, each style variation |
| Typefaces | at most two families, each with a role (headings, body and UI); mono only for code or figures | `typography.fontFamilies` and `fontSizes`, bundled local font files |
| Layout idea | one sentence: grid, density, the one focal point per main template | `layout` content and wide size, patterns |
| Signature detail | one memorable choice (shape, rhythm, motion, illustration), used with restraint | `styles` and presets, never one-off CSS |

## Pick the mode first
Admin screens and tools: consistency with wp-admin beats expression. Front-end landing, home and marketing patterns may carry more of the signature.

## Reject the defaults (keep one only with a reason)
- A stock palette or untouched starter-theme colours with no reason; gradient or glow accents added to look modern; the common generated palettes (purple on white, cream with one rust accent, near-black with one neon accent).
- Decorative tells with no meaning: numbered markers where nothing is a sequence, one highlighted word per headline, all-caps labels above every title, arrows on every link.
- Ask of each choice: would it fit any other brand unchanged? If yes, revise it.
- One weight everywhere; every section a card with the same radius and shadow; everything centred.
- Icon-only controls for main actions; decoration that carries no meaning.

## Limits
- Taste never beats the plan, contrast, or the target-size rule (`fswpdevops/references/accessibility.md`).
- One direction per site, recorded in `DESIGN.md`; new templates follow it instead of re-planning.
- No new font, plugin or package without the owner's yes (licence, size, privacy).
