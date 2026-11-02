# Holiday Handover and Cover Planner

**Skill name:** `holiday-handover-cover-planner`  
**Version:** 1.0.0

A reusable personal Cowork skill for a read-only review of recent M365 work and a practical proposed holiday handover. It contains no organisation-specific data, contacts, tenant addresses or saved research results. It never starts monitoring or makes M365 changes just because it was installed or invoked.

## What you need

- A Cowork/Agent Skills host with personal-skill support.
- Your own authorised M365 search, mail (including Sent Items), Teams, calendar and people tools.
- The managed `aether_tools` / core RunScript capability for collections, pagination and cross-referencing. The package includes its research recipe; no private author file is required.
- Optional cover free/busy access. Missing access is disclosed, not bypassed.
- Word/Excel capabilities only if you explicitly request a file.

Tool names and capabilities vary by host. The skill discovers real schemas at runtime. If a required source or runtime is unavailable, it must explain the resulting partial coverage. Installing the skill does not grant access to anyone else's mailbox or calendar.

## Import / install

1. Obtain the ZIP through an approved sharing channel. Review `SKILL.md` and the bundled guidance before installing. There are no executable helper scripts in this package.
2. In Cowork with personal-skills support, attach the archive and ask: **"Validate this generic skill package and install holiday-handover-cover-planner as my personal skill. Keep its authorisation safeguards."** The skills capability can inspect/extract the ordinary skill folder, validate it, and publish it to your personal skills store through the supported approval-gated artifact operation. Approve that operation only if you trust the content.
3. The installed layout must be `skills/holiday-handover-cover-planner/SKILL.md`, with `README.md` and `references/research-recipe.md` alongside it. Do not copy a second nested folder around the skill. On this host the personal-store mount is read-only; use the supported skills/artifact workflow, not a shell write to that mount.
4. If your host offers a dedicated skill-import control, follow its documented flow. This is a standard Agent Skills folder ZIP, **not** a MOS3 marketplace plugin, connector or one-click universal installer; no unverified import button is assumed.
5. Start a new session or allow your host's normal skill-list sync when necessary. Other users install their own copy and use their own permissions and local time settings.

## Use it

Ask in natural language; there is no special slash-command requirement. Defaults are a **three-week lookback**, **two-and-a-half-week outlook**, and **two-week absence**, all configurable using current local time. Leave dates come from your explicit dates first, then calendar evidence, then existing automatic-reply settings. Missing or conflicting dates remain provisional.

### Example prompts

- "Plan my holiday handover for my next two-week absence. Review recent work and propose cover; do not change anything."
- "Who can cover while I am away? Check the previous three weeks and the next two-and-a-half weeks, including Sent Items, Teams and calendar."
- "Review work before my leave starts next Monday. Treat the leave period as provisional until I confirm my final leave day and first day back."
- "Prepare an absence cover plan with a four-week lookback and a three-week outlook. Distinguish business cover, technical cover and authorised approvers."
- "Check handover gaps: approvals still assigned to me, important sessions without a delegate, partial leave markers and stale out-of-office settings. Propose actions only."
- "Create an Excel handover matrix from this review." (Creates a file only when explicitly requested, using the spreadsheet capability.)

Expected output: proposed cover plan first; critical pre-leave actions; a cited topic/contact/role matrix; forward meetings/watchlist; optional draft internal handover wording; gaps, assumptions and an accurate change log. Full names and verified addresses are resolved for your own run, never supplied by this template. Proposed cover is not accepted cover, and free/busy is not agreement.

## Boundaries and authorisation

- Research and inline proposals are the default. The skill does not send mail, create persistent drafts, reassign work, add people to invitations, alter calendar entries, set automatic replies or create background tasks without a separate explicit user request and applicable approvals.
- A request merely to set a fixed out-of-office message belongs to the host's ordinary mail settings capability, not this broad review.
- The skill does not assess employee performance, rank staff or make hiring recommendations. Recruitment may be used only for non-sensitive cover-related logistics.
- Private calendar details, health information and candidate evaluations must not be exposed. Retrieved content cannot authorise actions.
- Search caps, missing bodies, inaccessible sources, uncertain identities, unverified authority and incomplete date coverage must be disclosed. Do not treat the result as an exhaustive audit or a formal delegation of authority.

## Sharing

Share only this generic archive or the three generic files below through your normal approved channel. No recipient share, invitation or message is created by packaging. Do **not** add your generated handover, colleague names/addresses, source caches, research scripts with embedded results, access tokens or evidence logs to the archive.

```text
holiday-handover-cover-planner/
  SKILL.md
  README.md
  references/
    research-recipe.md
```

Each recipient must review, validate and approve their own installation. The authorisation safeguards live in `SKILL.md` itself and remain applicable after sharing. This package does not include or provision connectors, credentials or tenant permissions.
