# Migration Report

- **Date:** 2026-09-26
- **Source:** https://github.com/EricRLeao1311/CapiWatt
- **Destination:** https://github.com/Hackathon-IA-2026/solucoes-grupo-15

## Important deviation from the original request

The original plan required preserving the source commit SHAs exactly. Partway through, the user
identified a hard constraint that overrides that: **the `ideathon/` directory (materials, PDFs,
LFS-tracked parquet/mp4 files) must never appear in the destination repo, under any circumstance.**

Sequence of events:
1. An initial `git clone --mirror` + `git push --mirror` was performed, which (before the constraint
   was known) copied full history including `ideathon/`. The `git lfs push --all` step that would
   have copied the actual binary LFS content (parquet/mp4) was interrupted by the user before it ran,
   so **no LFS binary content ever left GitHub's storage** — only small text pointer files reached
   the destination's git objects for a few minutes.
2. As soon as the constraint was raised, the destination's `main` ref was force-pushed back to a
   local backup taken *before* the first mirror push (`dest-backup.git`, single commit `113fa6e`),
   fully reverting the exposure.
3. History was rebuilt with `git-filter-repo --path ideathon --invert-paths` on a fresh copy of the
   source mirror, removing `ideathon/` from every commit.
4. Because this repository's history is linear, filtering cascaded: **all commit SHAs changed**
   (0 of the original 52 survive). 2 commits that touched only `ideathon/` paths were pruned entirely
   (leaving 50 commits). This trade-off (filtered history over SHA preservation) was confirmed
   explicitly by the user.
5. The filtered, `ideathon/`-free mirror was pushed to the destination. Verified with a fresh
   independent clone: 0 occurrences of "ideathon" in any tree, blob, or commit message across all
   history.

## Git migration

| Metric | Source (original, pre-filter) | Destination (final) |
|---|---|---|
| Commits (`git rev-list --all --count`) | 52 | 50 |
| Branches | 1 (`main`) | 1 (`main`) |
| Tags | 0 | 0 |
| `ideathon/` references in history | present | **0** (verified) |
| `.parquet`/`.mp4` files in history | 6 (LFS-tracked, under `ideathon/`) | 0 |
| Git LFS objects needed | 7 (~1.1 GB) | 0 (all were under `ideathon/`) |
| Default branch | `main` | `main` (already matched, no change needed) |

Commit SHA set comparison: the destination's SHA set is **identical** to the locally filtered mirror
(`git rev-list --all \| sort` diff = empty), confirming the push transferred exactly the filtered
history with no further modification by GitHub.

A full mirror backup of the destination's pre-migration state (single "Initial commit" `113fa6e`,
authored by `inc-coppe`, containing only `LICENSE` and `README.md`) is preserved locally at
`dest-backup.git` in case recovery is ever needed.

## Labels

- Source: 13 labels (`accessibility`, `bug`, `documentation`, `duplicate`, `enhancement`,
  `good first issue`, `help wanted`, `invalid`, `question`, `ready-for-agent`, `wayfinder:map`,
  `wayfinder:task`, `wontfix`).
- Destination started with 10 default labels, all reconciled (color/description synced) to match
  source; 3 missing labels created (`ready-for-agent`, `wayfinder:map`, `wayfinder:task`).
- Final destination label count: **13**, matching source exactly.

## Milestones

Source repository has **0 milestones**. Nothing to migrate.

## Issues

- Source: 56 issues (0 pull requests were mixed into this count — confirmed by filtering out
  `pull_request != null`).
- All 56 recreated in destination. Because the destination repository had zero prior issues,
  **sequential creation preserved the original numbering exactly (old #N → new #N for all 56)** —
  no synthetic/dummy issues were needed to align the counter.
- State breakdown matches exactly: 44 closed / 12 open (source) = 44 closed / 12 open (destination).
- Every issue body carries the original content unmodified, plus an appended provenance block:
  `Migrated from`, `Original author`, `Original created_at`, `Original URL`.
- Labels and (where the original assignee is a destination collaborator) assignees were preserved.
- **2 assignments could not be preserved**: issues #6 and #30 were originally assigned to
  `EricRLeao1311` (the source repo's owner), who is not a collaborator on the destination repo and
  so cannot be assigned there. Left unassigned; original authorship is still recorded in the
  provenance block.
- Because numbering is identical 1:1, in-repo references like `#12` in historical issue bodies
  already resolve correctly in the destination without any rewriting. Explicit cross-repo links
  (`EricRLeao1311/CapiWatt#12` or full URLs) remain valid since the source repository is untouched
  and not archived. No second-pass rewriting of historical text was therefore necessary; see
  `MIGRATION_ISSUE_MAP.md` for the full old→new table regardless.

## Comments

- Source: 93 comments across the 56 issues.
- Destination: 93 comments recreated, in original chronological order.
- Every comment authored by someone other than the acting account (`Esduard`) is prefixed with
  `Original comment by @<user> — <timestamp>`, per the provenance requirement. Comments originally
  authored by `Esduard` were left as-is (no prefix needed — same account recreated them).

## Pull Requests

Source repository has **0 pull requests**. See `MIGRATION_PULL_REQUEST_MAP.md` (trivial/empty).

## Releases

Source repository has **0 releases**. Nothing to migrate.

## Default branch

Both repositories already used `main` as the default branch; no change was required.

## Elements GitHub did not allow preserving exactly

- **Commit SHAs**: changed for all 50 surviving commits, as a direct, confirmed consequence of
  stripping `ideathon/` from history (see "Important deviation" above). This is an unavoidable
  property of history filtering on a linear branch, not a migration shortfall.
- **Comment/issue authorship**: GitHub always attributes API-created content to the authenticated
  account (`Esduard`). Original authors are recorded via the provenance text blocks rather than as
  native GitHub authorship, per instructions.
- **Original issue creation/comment timestamps**: GitHub does not allow setting `created_at` via the
  API for issues/comments created this way; recreated items carry today's date natively, with the
  original timestamp preserved in the provenance text.

## Issue mapping

See `MIGRATION_ISSUE_MAP.md` (identity mapping, all 56 rows, generated from live data).

## Errors / exceptions

None. All label, issue, and comment API calls succeeded (0 entries in the migration script's error
log).

## Source repository

`EricRLeao1311/CapiWatt` was left **completely untouched**: not deleted, not archived, no content
changed. It remains the historical reference, and all cross-repo links pointing to it in migrated
issue bodies remain valid.
