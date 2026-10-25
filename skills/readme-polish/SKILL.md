---
name: readme-polish
description: 优化、美化或重写 GitHub 项目 README，让仓库首页更直观。适用于 README 太丑、信息太密、缺少示例或快速开始，以及新项目 README 编写；结合开源模板、真实徽章、示意图与 GitHub 渲染检查。不用于个人主页装饰、学术论文润色或一般文档格式转换。
---

Improve a project's README for its actual audience. Use the open-source layout
patterns in [references/sources.md](references/sources.md) and adapt the original
[assets/README.template.md](assets/README.template.md). The template is a starting
point, not a required list of sections. Read [references/quality-check.md](references/quality-check.md)
for the final validation pass.

## Establish facts and scope

- Locate the intended repository from the message or current workspace. Read its
  current README, project instructions, dependency manifests, entry points,
  license and relevant CI files. Preserve unrelated edits and the user's language.
- Match the request's scope. Research-only means research; an optimization request
  authorizes README and directly supporting documentation/assets. It does not
  authorize a feature change, installing a third-party generator, or pushing to
  GitHub unless publication is already requested in the session.
- Distinguish working behavior, planned behavior and unknowns. Verify install and
  usage commands from the repository. Never invent test counts, performance,
  supported platforms, testimonials, downloads or green CI badges.
- For data-moving tools, state copy direction, overwrite/delete policy and the
  preview path before the real execution example. Do not run a real backup,
  migration, deployment or paid command just to illustrate the README.

## Design the reading path

Make the opening answer: what is this, who is it for, what happens when I use it,
and how do I begin? Diagnose the current hierarchy before adding decoration.

Prefer a short title/tagline, a few truthful badges and useful navigation. Put a
real demo/screenshot or a compact flow diagram near the top when it explains the
tool. Use 3-5 short capability statements or a concrete example rather than
several screens of feature lists.

Give the shortest verified quick start, then link to detailed installation,
recovery, troubleshooting and architecture docs. Keep limitations affecting safe
first use visible; move only the details. Preserve existing inbound section links
where practical, or explicitly record changed anchors.

Adapt to project type: a library needs a minimal API example; a CLI needs a
command/output example; a GUI benefits from a real screenshot; a dataset needs
access/schema/citation. Do not force every project into the same layout.

## Reuse open-source work honestly

- Use Best-README-Template's header/navigation/quick-start patterns as structural
  guidance, with attribution when adapting its material. Do not copy its example
  npm commands, fake API keys, placeholder URLs or irrelevant community sections.
- Use Shields.io for badges only when their labels match evidence. Prefer stable
  facts such as license or runtime. Distinguish a static local-test result from a
  live CI status; a version badge must have an actual matching source.
- Use awesome-readme to find one or two comparable projects when inspiration is
  needed. Learn their hierarchy and demonstration technique; do not copy branding,
  screenshots or assets without checking reuse rights.
- readme.so is an optional editor and readme-ai an optional draft generator.
  Neither is a runtime dependency of this skill. Do not install or call another
  model/API merely to rewrite text that can be authored directly here. If the user
  requests one, verify its current instructions and review its generated facts.

## Implement and inspect

1. Edit the README and only the supporting docs/assets needed for this request.
   Store images inside the repository with descriptive names and relative links.
   Prefer GitHub-supported Markdown, tables, details and small Mermaid diagrams;
   avoid CSS-heavy layouts and oversized decorative banners.
2. Keep real screenshots clearly separate from illustrative mockups. Use a simple
   diagram when no truthful screenshot exists. Label sample output as an example.
3. Run the checks in `references/quality-check.md`. If an existing Markdown linter
   is available, use it; do not add a Node toolchain solely for formatting.
4. Inspect the rendered result using the project's existing preview/browser or,
   for already public content, GitHub's renderer. Check first-screen hierarchy,
   narrow layouts, code wrapping, assets, anchors and light/dark readability.
   Static inspection alone is not a visual render check: disclose that limit.
5. If publishing is authorized, review the final diff, stage named files only,
   preserve upstream attribution, push normally and verify the remote result.
   Leave code, private paths, credentials and runtime logs out of documentation
   changes unless the request specifically requires them.

## Deliver

Lead with what became easier for the reader. Link the README, summarize important
structural/visual changes, report the checks actually completed and name any
unresolved factual or rendering limits. Distinguish a local draft from a published
result. Do not claim a universal quality score from a stylistic preference.
