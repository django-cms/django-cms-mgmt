# dCA Tech Committee – Decision Log

## Rules

1. **Agenda items state what they need.** Whoever adds an item marks it
   *FYI* (information only), *Feedback* (input wanted), or *Decision*
   (the committee needs to settle something).
2. **No champion, no decision.** A proposal becomes *Decided* only when
   someone volunteers to carry it through. Nobody is assigned work.
3. **Agreement without a champion is *Wanted*.** If the committee agrees
   with a direction but nobody volunteers, it goes on the Wanted list with
   the date it was listed.
4. **Reviewers volunteer too.** For work that needs review, the committee
   asks for a volunteer reviewer who commits to responding within a
   reasonable time (e.g. two weeks). Without one, the item stays *Wanted*.
5. **Wanted items are made visible.** Each Wanted item gets a GitHub issue
   labelled `help wanted`, linking its log entry. The list is shared with
   sprints, Djangonauts, and dCA news, and given to the board as candidates
   for funding.
6. **Wanted items expire.** An item with no champion after 6 months moves
   to *Expired*. Anyone willing to champion it can reopen it.
7. **Champions can step back.** A champion who can't continue says so.
   The item returns to *Wanted*, no questions asked.
8. **Decisions are not reversed silently.** A change of course is a new
   entry that marks the old one *Superseded*.
9. **Each meeting starts with the log.** Champions of *Open* items give a
    one-line status, and the Wanted list is checked for new volunteers.
10. **Empty meetings are cancelled.** If there are no items on the agenda
    30 minutes before the meeting, the meeting will be cancelled.

**Status:** *In effect* = policy or convention that applies.
*Done* = delivered. *Open* = decided, completion not yet confirmed by the
champion. *Superseded* = replaced by a later entry.
† = inferred from the meeting notes' wording; to be confirmed by attendees.

## Decided

| ID  | Date       | Decision | Champion | Status |
|-----|------------|----------|----------|--------|
| D1  | 11.02.2022 | Version-number policy for v3/v4 package compatibility goes into the official docs (discussion #7149). † | Mario | ✔️ |
| D2  | 11.02.2022 | Dark-mode workgroup created; work happens in djangocms-admin-style. | Andrew | ✔️ |
| D3  | 25.03.2022 | "JS Frontend Application" workgroup created for the frontend build pipeline. | ? | Expired |
| D4  | 20.05.2022 | Coding style guide is linked from the contributing docs; docs say "we", not "you". † | Andrew | ✔️ |
| D5  | 01.07.2022 | GitHub remains the code host; the committee follows the Django project's response to the SFC call. | Andrew | ✔️ |
| D6  | 26.08.2022 | A separate 4.1 release line keeps community releases apart from the sponsor's 4.0. † | Andrew, Mark | ✔️ |
| D7  | 09.09.2022 | Docs: quick wins on 3.11 now, new 4.x docs long-term. | Luis | Expired |
| D8  | 09.09.2022 | Namespaced-apphooks how-to rewritten with a simpler AppHookConfig. | Jacob | ✔️ |
| D9  | 07.10.2022 | No template linter. Use `{% localize off %}` where IDs are rendered; reviewers check for it (PR #7188). | All reviewers | ✔️ |
| D10 | 07.10.2022 | v3/v4 packages either support both versions or ship as a separate package, possibly using epochs. † | Jacob | ✔️ |
| D11 | 04.11.2022 | Page visibility depends on the page itself, not its parents. Add a setting only if a use case appears. | — | ✔️ |
| D12 | 18.11.2022 | 3.11 is the LTS: feature freeze, supported at least 4 years in line with Django LTS. † | Fabian | ✔️ |
| D13 | 13.01.2023 | Unmaintained `djangocms-*` PyPI names are reclaimed where needed (first: djangocms-events). † | Jens-Erik | ✔️ |
| D14 | 10.03.2023 | Release checklist and documented release process. | Fabian | ✔️ |
| D15 | 10.03.2023 | Demo updated to v4; quickstart moved into the org. † | Nicolai | ✔️ |
| D16 | 21.04.2023 | Release process automation: first merge automated, stale branches removed, PRs to `release/a.b.x` auto-generated, patch-release steps added. | Fabian | ✔️ |
| D17 | 16.06.2023 | django CMS 3.8.1 pins django-treebeard < 4.5. | ? | ✔️ |
| D18 | 16.06.2023 | filer 3.0 keeps its own icons for now (no re-use of CMS core icons). | ? | ✔️ |
| D19 | 30.06.2023 | filer 3.0 released despite breaking changes. | Fabian | ✔️ |
| D20 | 01.12.2023 | 4.1 release plan: RC5, docs merged into develop-4, final release. | Fabian | ✔️ |
| D21 | 01.12.2023 | Website plugin listing pulled from PyPI classifiers; meanwhile packages are sent to Fabian. | Fabian, Jens-Erik | ✔️ |
| D22 | 12.01.2024 | Default branch switches to `develop-4`. Long-term: one `main` plus `release/a.b.x`. | Fabian | ✔️ |
| D24 | 12.01.2024 | v4 education starts with YouTube videos; format decided first. | ? | ✔️ |
| D25 | 09.02.2024 | Users who can change a page can add a translation directly. Target: 4.1.1. | Jacob | ✔️ |
| D26 | 09.02.2024 | 4.2 targets: `PageUrl` uniqueness and Page/TreeNode merge. Superseded by D37; now W2 and W3. | Fabian, Jacob | ✔️ |
| D27 | 08.03.2024 | Re-introduce low-level publication permissions plus a "set home page" permission. Review outstanding, see W5. | Fabian | ✔️ |
| D28 | 08.03.2024 | Docs discourage multi-level `CMSPlugin` inheritance in favour of abstract/proxy models. † | Fabian | ✔️ |
| D29 | 17.05.2024 | Regular maintenance tickets for JS asset updates. | Fabian | ➖ |
| D31 | 12.07.2024 | 4.2 focus: headless mode and performance. New features go through GitHub Discussions. | Fabian | ✔️ |
| D32 | 12.07.2024 | djangocms-4-migration updated and moved under the dCA. | Fabian | ✔️ |
| D33 | 04.10.2024 | Page titles in the tree view are grey, not bold. | Fabian | ✔️ |
| D34 | 01.11.2024 | Issue #8019: language choosers updated and a `Page.languages` fix proposed. | Fabian | ✔️ |
| D35 | 10.01.2025 | djangocms-ckeditor deprecated in favour of djangocms-text. † | Fabian | ✔️ |
| D36 | 24.01.2025 | Feature freeze for django CMS 4.2. | Fabian | ✔️ |
| D37 | 24.01.2025 | Page-creator DB refactor postponed beyond 4.2. Now W1. | — | ➖ |
| D38 | 05.09.2025 | Discord channel for businesses using django CMS. | Fabian | ✔️ |
| D39 | 31.10.2025 | Accidental "Delete all translations" handled via a "marked for removal" state; feature request filed (djangocms-versioning #490). | Jacob | Open |
| D40 | 09.01.2026 | In 5.1: redirects marked in the page tree (#6509); "Show in menu" disabled for published pages (#7780). | ✔️ | Done |

## Wanted

The 6-month expiry clock starts when this log is adopted.

| ID  | Topic | Raised | Needs | Possible champion | Notes |
|-----|-------|--------|-------|-------------------|-------|
| W1  | Normalize `created_by`/`changed_by` to foreign keys | 04.2022 – 01.2025 | Builder + reviewer | Jacob | Raised six times; postponed from 4.2 (D37). |
| W4  | Plugin restriction calculation / endpoint | 04.2025 – 01.2026 | Builder | Fabian | Not completed for 5.1. |
| W5  | Review of publishing permissions PR #7837 | 03.2024 – 05.2024 | Reviewer | Jacob | Implements D27. |
| W6  | Performance workgroup (N+1 issues while editing) | 05.2024 | Lead | Fabian, Jacob | Benchmark repo exists (fsbraun/django-cms-benchmark). |
| W7  | Formatting: `ruff format` via pre-commit vs one-off PR | 11.2023 – 11.2024 | Builder | Mark | Small, well-scoped. |
| W8  | Convention for building JavaScript modules | 07.2025 | Decision | Jacob, Vinit | Two differing approaches in use. |
| W9  | Is django-filer required? Purpose of `finder_public_private` | 07.2025 – 11.2025 | Decision | Jacob | |
| W10 | Prune inactive workgroups | 10.2022 – 09.2025 | Builder | Fabian | Overview of active workgroups was to be produced. |
| W11 | `CMSAppExtension` contract; async app hooks; MCP server | 01.2026 | Builder | Fabian, Mike | Recent; may already be in progress. |
| W12 | AI integration workgroup | 01.2025 | Lead | Mike | |

## Expired

Proposed to expire on adoption: no activity for over a year and no
champion. Anyone can reopen an item by volunteering.

| ID  | Topic | Last raised |
|-----|-------|-------------|
| E1  | Stale issue/PR bot (PR #7298) | 04.2022 |
| E2  | Central UX style/icon guidelines across packages | 06.2023 |
| E3  | Community survey on audience and market fit | 12.2022 |
| E4  | Stop committing generated JS bundles | 01.2024 |
| E5  | Separate the menu app from core | 07.2024 |
| E6  | Discord vs Slack as the single chat platform | 02.2024 |
