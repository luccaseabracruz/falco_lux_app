---
status: Draft
---
# FalcoLux — Project State

> Update at the end of each sprint. Last updated: 2026-10-19.

## Current phase
Lean Inception / discovery. **There is no code yet.**

## Context (3 lines)
Platform for the operational management of bird control and falconry (Portugal and Spain): staff attendance and safety, raptor management and weighing, field journal and client reports. The client's proposal is a **hypothesis**, not a closed requirement.

## Decisions made
| Date | Decision |
|---|---|
| 2026-10 | The client prioritizes M1 (Attendance) and M2 (Falconry LABS), with weighing from the start. |
| 2026-10 | Milestones are organized by **outcome**, not by module (M0, M1a, M1b, M1c, M2a, M2b). |
| 2026-10 | Documentation lives in the repository (`docs/`), in Markdown. Obsidian is only the editor. |
| 2026-10 | Everything in the repository is in English (see [conventions](conventions.md)). |
| 2026-10 | Weight prediction (M2b) is a hypothesis and stays out of the MVP. |

## Pending decisions
- [ ] ADR-001: PWA vs. native vs. hybrid (blocks M1b and maybe M0).
- [ ] Bird assignment: by site or by technician? (see OQ-01)

## Current milestone
None. Next: **M0 — Walking skeleton**.

## Blockers
See [open-questions.md](product/open-questions.md). Blocking: OQ-01, OQ-02, OQ-05, OQ-06.

## Working pace
2 h/day, 5 days/week (~10 h; assume ~8 productive hours). 2-week sprints.
Measured velocity: _to fill after the first stories._

## Next steps
1. Send the blocking questions to the client.
2. Talk to 1-2 field technicians (real personas and journey).
3. Draft the MVP Canvas (`product/vision-and-mvp-canvas.md`).
4. Start M0 and write ADR-001.

## Changelog
- 2026-10-19: document created.