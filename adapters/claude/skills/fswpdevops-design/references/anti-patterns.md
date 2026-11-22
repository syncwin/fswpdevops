# Anti-patterns by product type

Pick the row for the product (the plan names it), copy the chosen lines into `DESIGN.md` under "Avoid", and add project-specific ones there. The critic checks screens against that list.

| Product type | Avoid |
|---|---|
| All | hard-coded colours, sizes or figures in templates and patterns (use presets and dynamic sources); colour as the only signal; layout shift from late images; hidden destructive actions with no confirm; text in images |
| Business and marketing sites | stock hero with no proof; several competing calls to action; walls of equal-weight cards; autoplay sliders; pop-ups on first load |
| Shops and money | prices rounded so cents disappear; red and green as the only signal; confirm text that does not repeat the amount; surprise costs late in checkout |
| Blog, content, reading | line length past about 70 characters; no visible date or author where trust matters; unlabelled icon-only actions; infinite scroll with no end or position |
| Health and wellbeing | alarming colour for neutral data; medical-sounding claims in copy; tiny targets for tired or older users |
| Plugin settings and admin | settings that apply nothing until a hidden Save; jargon labels; destructive and safe actions side by side in the same style; a custom look that fights wp-admin |
| Forms and onboarding | placeholder used as the label; errors only on submit; blocking paste; more than one question per step on a phone |

Lines are short on purpose: prompts for judgement, not a style database.
