# Credits

Full-Stack WP DevOps is one MIT-licensed package. Every skill, script, and reference in it was written for this plugin. No third-party skill is forked, bundled, or copied. The projects below shaped ideas or are linked as sources of truth; their licenses are named for reference only and do not apply to this package.

| Project | What we learned from it | License (reference) |
|---|---|---|
| WordPress developer documentation and Core Contributor Handbook (WordPress community) | Source of truth for APIs, standards, and contribution workflow. Linked from `adapters/claude/skills/fswpdevops/references/official-docs.md`, not copied | See each site |
| [WordPress/agent-skills](https://github.com/WordPress/agent-skills) | Which WordPress domains an agent skill set should cover | GPL-2.0-or-later |
| [Anthropic claude-plugins-official](https://github.com/anthropics/claude-plugins-official) (pr-review-toolkit) | The idea of confidence-scored review that reports only high-certainty findings | Apache-2.0 |
| [OWASP secure-agent-playbook](https://github.com/OWASP/secure-agent-playbook) | The idea of structured security review with weakness IDs | CC BY 4.0 |
| [alibaba/open-code-review](https://github.com/alibaba/open-code-review) | The idea of path-scoped, project-owned review rules | Apache-2.0 |
| [dietrichgebert/ponytail](https://github.com/dietrichgebert/ponytail) | The minimal-code order of operations (the lean ladder in `adapters/claude/skills/fswpdevops/references/lean-coding.md`, rewritten in our own words) and reviewing for over-engineering | MIT |
| [anthropics/skills](https://github.com/anthropics/skills) `frontend-design`, `webapp-testing` | A short design plan before code and a check against generic generated defaults; look before acting (shoot, fix, re-shoot) (`fswpdevops-design/references/design-direction.md`) | Apache-2.0 |
| [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | Product-type anti-pattern lists and a master design file (`fswpdevops-design/references/anti-patterns.md`) | MIT |
| [pbakaus/impeccable](https://github.com/pbakaus/impeccable) | Lens scores 0 to 4 and narrow focused passes (`fswpdevops-critic/references/focused-passes.md`) | Apache-2.0 |
| [ibelick/ui-skills](https://github.com/ibelick/ui-skills) `baseline-ui` | Strict baseline rules (`fswpdevops-design/references/baseline-ui.md`) | MIT |
| [vercel-labs/web-interface-guidelines](https://github.com/vercel-labs/web-interface-guidelines) | Web accessibility checks: visible focus, switch roles, labelled fields, target size | MIT |
| Public talks on agent-written PRs | SDLC agent-factory pattern (`fswpdevops/references/factory-workflow.md`) | n/a (idea only) |

Tools such as PHPCS, WordPress Coding Standards, PHPStan, and WordPress stubs are downloaded on demand by the `setup_toolchain` recipe from their own projects and are not part of this package.

WordPress and WP are trademarks of the WordPress Foundation; WP-CLI is a WordPress Foundation project; Claude and Anthropic are trademarks of Anthropic, PBC. This project is independent and not affiliated with or endorsed by any of them. See `docs/trademarks.md`.
