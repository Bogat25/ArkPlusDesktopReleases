<!-- agent-context:kernel:start sha=a5893754536e5d1e3c7a91f59b8ce4d390600e608ed938e65676d53c3b260c13 -->
# User repository preferences

- Create commits locally when requested or when completing repository changes.
- Never push commits, create or modify pull requests, trigger GitHub workflows,
  publish releases, or otherwise write to GitHub.
- Treat all GitHub access as read-only unless the user explicitly revokes this
  rule in a later message.
- Commit directly on each repository's default branch (`main`, or `master` where applicable); do not create feature branches.
- Never add `Co-Authored-By` trailers or any AI attribution lines/footers to commits, PRs, files, or documentation.
- Keep commits few per feature (1-2 clean conventional commits); squash or amend unpushed fixups.
- Never read, print, echo, substring, or output plaintext secret values or token fragments anywhere. Test existence only (`Test-Path Env:NAME` or `[bool]$env:NAME`).
- Maintain strict isolation between AI agents (`codex`, `claude`, `gemini`): separate service accounts, tokens, and endpoints.
- Write reports, plans and other documents as Markdown (`.md`) files in the relevant repository or folder. Never publish them as hosted pages (claude.ai Artifacts, Claude Docs or any other agent's equivalent) unless strictly necessary or the user explicitly asks for one.
<!-- agent-context:kernel:end -->

## This repository
<!-- agent-context:contract:start sha=b2627545c4cf359734d237e9c1a61ba332eb6359f031e59bd83f25820f41aba9 -->
> Synced from `AgentContext/kernel/repos/ArkPlusReleases.md` by `AgentContext/scripts/sync.ps1`. Edit it there, not here.
> `[[name]]` is a platform doc: `AgentContext/corpus/platform/name.md`, or `read("name")` on the agent-context MCP server.

A placeholder: the repository holds only an empty `Readme.md` (2026-07-12) and `AGENTS.md`. Default branch `main`.

It is **not** the desktop release feed. ArkPlusDesktop publishes its Velopack releases to `Bogat25/ArkPlusDesktopReleases` (`ArkPlusDesktop/.github/workflows/release-desktop.yml`).

### Build, test, deploy
None.
<!-- agent-context:contract:end -->
