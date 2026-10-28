<!-- agent-context:kernel:start sha=bc480b1655265682a15a137e9090cd0029723794c5b82eeb54c4cdc7f1eff76f -->
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
- Maintain separate MCP service accounts, tokens, and endpoints for `codex`, `claude`, and `gemini`.
- GitHub exception: all three agents intentionally share one Linux/T3 security boundary. Use your own GitHub App by convention: Codex = `codex` (5516570), Claude = `claude` (5516624), Gemini/Antigravity = `antigravity` (5517659). Never select another agent's App or fall back to a personal GitHub credential. This is an instruction, not enforced isolation between agents.
- For authenticated Git or GitHub CLI commands, use `python3 /home/agent/repos/AgentContext/scripts/setup_github_apps.py run --agent <your-agent> --repo <repository-name> -- git ...` (or `gh ...`). Keep the existing human commit author identity; App credentials identify the pusher and PR author, not the local commit author. Never run credential/token-display commands. If your App is unavailable, report it instead of using another credential. This does not authorize GitHub writes prohibited above.
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
