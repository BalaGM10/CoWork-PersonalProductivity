# Marketing Email Review & Approval-Gated Unsubscribe

A reusable Cowork skill that audits promotional mail, protects operational correspondence, produces an approval register and handles only explicitly approved, verified opt-outs. Version 1.0.0. Original generic package; MIT licensed.

## Install in Cowork
1. Review this ZIP before installing. It contains instructions and synthetic tests, not a mailbox connector or executable app.
2. Extract the folder `marketing-email-unsubscribe-review` into your Cowork personal skills folder, normally **Documents/Cowork/skills/**. The resulting entry point must be `Documents/Cowork/skills/marketing-email-unsubscribe-review/SKILL.md`; avoid an extra nested copy of the same folder. Your organisation may configure a different Cowork root or managed skills-import UI: use that host-supported location/UI instead.
3. Allow your Cowork skill folder to sync and begin a new session if the skill is not detected. Do not overwrite another modified copy without reviewing it.
4. This package does not install tools or grant mailbox permissions. Live work depends on supported host tools and the user's authorisation. If your host supports importing a skill ZIP, select this archive; otherwise use the folder layout above. This is not a Microsoft Store/MOS3 plugin package.

## Use
- "Review marketing emails for the last 90 days." Read-only audit; no unsubscribing.
- "Create an unsubscribe report and approval register; exclude these organisation domains: example.org." All illustrative domains here are synthetic. Configure your own domains privately at run time.
- "Unsubscribe A-001 only from the register; keep all other lists." Separate explicit sender/list approval; verification can still hold an unsafe/global opt-out.
- "Prepare drafts only for A-001 and A-003. Do not send." Saved drafts require supported mail tools and that explicit request.

Default time window is the previous 90 completed local calendar days, with exact bounds stated. Configure dates/timezone, folders, organisation domains, affiliates, protected relationships and output format per request. No future scheduling is created.

## What you receive
An evidence-based audit, historical message counts and sender/list-level Pending decisions. A private saved report/register is created only where supported and verified; otherwise the skill supplies an inline version and says no saved file was created. Later results distinguish approval, request acceptance, Sent Items evidence, delivery, cancellation, holds and manual steps.

## Files
- `SKILL.md`: entry point, routing, audit, approval and reconciliation workflow.
- `README.md`: installation and usage.
- `references/execution.md`: route verification, safe mailto rules and checkpointing.
- `tests/README.md`: portable offline acceptance checklist.
- `tests/cases.json`: synthetic behavioural fixtures with expected outcomes.
- `LICENSE`: permission and disclaimer.

## Privacy and sharing
Only this generic package is intended for sharing. Do not add real email, identities, domains, address lists, message subjects, headers, tracking tokens, private links, reports, workbooks, checkpoints, journals, receipts or credentials. Examples use example.org/example.com; no live endpoints are supplied. Installing/sharing the package never grants permission to send or unsubscribe. No external publication, community delivery or permission change is performed by this package.

## Testing and limitations
Use `tests/README.md` in offline mode before a live run. No executable helper, network client or embedded tool identity is bundled. Independent isolated model tests can test instructions against synthetic situations, but do not prove connector compatibility, real authentication, delivery or actual cancellation. Tool availability, mailbox pagination limits, browser availability and Office features differ by host. Safety holds are intentional, not a reason to bypass unavailable tools.

Validation reports are delivered separately from the shareable ZIP so private test trajectories and local paths cannot accidentally become part of the reusable skill. Absolute rubric scores are advisory, not security guarantees or community/store certification. Human review and host-specific dry runs remain recommended before community deployment.
