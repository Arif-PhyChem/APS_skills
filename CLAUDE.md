# APS Editorial Intelligence — Claude Code

Follow [AGENTS.md](AGENTS.md). It is the single, vendor-neutral instruction file
for this repository; nothing here overrides it.

Two Claude-specific notes:

- The skills are plain files, not registered Claude Code skills. Read them with
  the Read tool; do not expect them under `/`. To register one, symlink or copy
  its directory into `~/.claude/skills/`.
- `journals.aps.org` blocks WebFetch (HTTP 403). Use the Bash + reader-proxy
  method documented in AGENTS.md instead.
