# Open-source sources and how to use them

Reviewed 2026-10-25. These are upstream references, not bundled executable
dependencies. Recheck current facts before recommending installation or versions.

| Source | Concrete use in this skill | Reuse boundary |
|---|---|---|
| [Best-README-Template](https://github.com/othneildrew/Best-README-Template) | Header, short navigation, quick start and documentation structure; inspect `BLANK_README.md` | Upstream Unlicense. Our template is original wording informed by its structure; preserve attribution for adapted material |
| [Shields](https://github.com/badges/shields) / [Shields.io](https://shields.io/) | Small consistent badges for verified facts | Use badge service URLs; no server/library code is bundled. Check upstream terms if vendoring code |
| [awesome-readme](https://github.com/matiassingers/awesome-readme) | Find comparable examples of effective screenshots, demonstrations and hierarchy | Inspiration and links only. Do not treat the list as permission to redistribute linked projects' assets |
| [readme.so](https://github.com/octokatherine/readme.so) | Optional section editing and preview | Upstream MIT. Not required to execute this skill |
| [readme-ai](https://github.com/eli64s/readme-ai) | Optional repository-derived drafts when explicitly useful/requested | Upstream MIT. Validate generated statements; API-backed modes may send repository content to the configured service |

## What we add

The original contribution here is a reusable Codex authoring workflow: determine
facts, select a reading path, adapt layout, verify commands/links/badges, inspect
rendering and report the actual result. We do not claim to have created upstream
template patterns, badge rendering or another README generation engine.

## Applying it to a local backup tool

An opening diagram can show work folder → changed files → external drive, with
old overwritten files retained beside the current copy. A behavior table should
explain unchanged/new/modified/destination-only files. Put preview before copying
and make deletion/overwrite rules visible. Explain the underlying engine's role
in a short comparison, while linking recovery and long-running verification to
dedicated docs. This is an example, not a required layout for other project types.
