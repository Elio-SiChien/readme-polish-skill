# Validation checklist

## Facts and commands

- Trace feature statements, runtime/platform requirements, license and status to
  repository evidence. Clearly mark plans, examples and untested platforms.
- Verify install/usage commands against real entry points, manifests and CLI help.
  Use safe samples when execution is needed. Do not perform a real destructive,
  external, paid or data-moving operation merely to test README instructions.
- A green CI badge needs the named workflow to exist and the displayed branch to
  be correct. Do not turn local test results into a fake CI signal.
- Generated examples must not imply a package is published, a release exists or
  a benchmark was measured without checking.

## Links and structure

- Check Markdown inline links, reference-style definitions and HTML `href`/`src`.
  Resolve relative paths from the document's directory, including image paths.
- Check heading anchors, duplicate heading suffixes and explicit HTML anchors.
  Account for existing inbound links when renaming sections.
- Remove placeholders (`{{...}}`, `example.com`, `github_username`) from delivered
  README files. Authoring templates may retain labeled replacement fields.
- Keep key install/usage/safety information outside collapsed details blocks.
  Use tables for comparisons, not long paragraphs squeezed into narrow columns.
- Check `git diff --check`, but do not call it a Markdown or semantic validator.

## Render

- Inspect a GitHub-supported rendering, including Mermaid where used. A generic
  Markdown renderer may differ from GitHub; label it as an approximate preview.
- Never submit private README content to an external renderer without a basis
  for sharing it. Use a local preview for private repositories.
- Confirm hierarchy at desktop and narrow widths, working images, readable code,
  meaningful alt text and contrast in both themes when images/badges are involved.
- If no browser/renderer is available, finish static checks and explicitly state
  that visual verification remains unperformed. Do not fabricate screenshots.

## Publication

- Review only intended documentation/asset changes and upstream credit notices.
- Exclude personal absolute paths, credentials, logs and private research files.
- If publishing is authorized, stage named paths, push without force and verify
  the remote README and referenced assets. Report the final URL and actual checks.
