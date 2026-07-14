<!-- Satellite context file — extends the global hub (~/.claude/CLAUDE.md | ~/.pi/agent/AGENTS.md). Host-neutral; project-specific only. Do not duplicate hub standards here. -->

# getlumos/.github

> Organization-wide GitHub configuration (the special `.github` meta repo) for the getlumos organization.

This repo holds default community-health files and org-wide config that GitHub
automatically applies to every repo under `getlumos`, unless overridden locally.

## What lives here

- **`.github/FUNDING.yml`** — enables the "Sponsor" button on all getlumos repos,
  linking to [@rz1989s](https://github.com/sponsors/rz1989s).
- **`profile/README.md`** — the organization profile README shown on the
  `github.com/getlumos` landing page (ecosystem overview, editor support matrix,
  quick start, roadmap, community links).

## Notes

- Per-repo overrides win: a repo's own `.github/FUNDING.yml` (or other default
  health file) takes precedence over the org-level one here.
- The profile README is Markdown rendered on GitHub's org page; keep its tables
  and badges in sync with the actual ecosystem (see
  [getlumos/lumos/AGENTS.md](https://github.com/getlumos/lumos/blob/main/AGENTS.md)
  for the canonical repo list/versions).