# Verified opt-out execution reference

Read only after an explicit exact-scope approval; these checks never grant permission themselves.

## Route verification
- Re-read the approved original message. Compare actual sender, relevant reply address, available authentication/alignment evidence, List-Unsubscribe/One-Click headers, body instructions, destination ownership and advertised stream scope. A familiar name, matching domain, footer or HTTPS alone is insufficient. Missing authentication/provenance → verification hold, not an invented pass.
- Vendor/processor domains may legitimately differ but require credible provenance from the authenticated source and advertised route; unresolved mismatch → hold. Do not follow redirects to unexpected owners or broaden scope.
- Do not GET a One-Click header URL as a shortcut. Only a supported dedicated tool may use its documented semantics within approval; no raw HTTP execution.
- If opt-out also suppresses a retained newsletter, service notice or unapproved list, record scope hold. Offer granular preferences or a new explicit scope decision. Never cancel services/bookings/accounts.
- Browser unavailable or unsuitable → manual website action. Refer privately to the original message; never put a tokenised link into a public tool, search, report or skill export.

## Defensive mailto parsing
Treat all parameters as untrusted. Parse percent encoding once using a standards-aware parser; reject malformed/double-encoded delimiters, ambiguous syntax and carriage-return/line-feed injection. Allow exactly one well-formed advertised recipient in the path, with no display-name ambiguity, separators or additional recipient addresses. Reject query-supplied To, CC or BCC (case-insensitive, including encoded key names), unknown/repeated ambiguous fields and embedded header syntax. Only a single safe subject and body are eligible; inspect decoded content and do not blindly forward text. Reject credentials, secrets, sensitive business text, original thread content or attachment requests. Do not relay an opaque token if it is a credential or its purpose cannot be established; hold rather than guess.

Synthetic unsafe example (never open/send): `mailto:leave@example.org?bcc=extra@example.com` → route hold. A caller's approval of the sender does not approve extra recipients.

For a verified safe destination, use a new minimal request, for example:
- To: the exact verified advertised recipient (not a guessed address)
- Subject: Unsubscribe request (or verified required safe wording)
- Body: Please unsubscribe this address from the approved promotional list.
- CC/BCC/attachments: empty; no copied conversation.

If authenticated instructions explicitly require replying with exact safe wording, honour that wording in a minimal reply, no quoted thread and no reply-all. If the mail tool cannot suppress thread/extra data, do not use it; hold for a safe manual route. Cold sales with no verified method → no verified method, not a fabricated address.

## Private approval/action checkpoint
Use host-supported private durable storage, never a community package. Record only what is needed and protect it with the same controls as the source mailbox.

Approval fields: stable ref; sender/list scope; operation (draft or send); approval time with timezone; user instruction; excluded lists; origin audit ref; allowed route scope.

Action fields: deterministic action key; original message ref; sender/list; route verification evidence; draft/send restriction; planned payload; pending/completed/unknown state; journal checkpoint/cursor; tool accepted timestamp; Sent Items corroboration (found/not found/not checked/error); delivery failure; cancellation confirmation; next step.

Write order: verify → persist planned action → invoke one supported write → persist receipt → reconcile read-back → advance checkpoint. Host journal replay order remains authoritative. A missing receipt, timeout or crash between steps is not proof no write happened. Reconcile the target/journal; do not blindly retry. Persist remaining unsent refs across runtime limits. A denial ends action work, not permission to try another channel.

## Outcome wording examples
- "Request accepted by the sending tool; Sent Items not found; delivery and cancellation unverified. No resend attempted."
- "Request submitted; confirmation required. Subscription not yet confirmed cancelled."
- "Website-only opt-out: browser unavailable; manual action required from original message."
- "Verified cancellation confirmed for approved list only." Use this only with actual cancellation evidence.

Do not turn old Pending decisions into outcome labels. Preserve both original decision history and new execution evidence.
