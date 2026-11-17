# Discover Your Own AI Use Cases

## A practical community guide for Copilot Cowork and Work IQ-enabled experiences

*Community article · 7 November 2026*

The hardest question about AI at work is often not “How do I write a better prompt?” It is “Which part of my actual job should I try it on?”

A product demonstration can show what is possible. A catalogue of prompts can offer inspiration. Neither necessarily tells you where to start on a Monday morning, with your meetings, your open decisions and your unfinished deliverables.

Here is a different starting point: ask your approved AI experience to help you discover useful applications from evidence of your own work. Not from a generic job description. Not from another person’s success story. From the recurring activities, information hand-offs and review tasks you can actually verify.

**Start with your work. Discover the pattern. Test one bounded outcome.**

This article offers a reusable method, a copyable discovery prompt and a way to turn individual experiments into community learning—without sharing private work content.

## One method, two ways to start

**If you have Copilot Cowork:** Microsoft describes Cowork as carrying out multi-step work across Microsoft 365, including research, document creation and scheduled prompts. [1]

**If you use a Work IQ-enabled experience:** Work IQ is Microsoft’s permission-aware workplace intelligence layer for Copilot and agents. [2] It is not a guarantee that every chat surface offers the same tools.

Use the Copilot experience or organisation-approved agent available to you. Ask it to describe which work sources it can actually use for this request. Do not assume that access to work context also means access to file creation, scheduling or business-system actions.

The method stays the same; the delivery route changes:

- **Cowork route:** ask for a new reviewable document or other supported deliverable.
- **Context-enabled route:** ask for a structured response first. If file creation is not supported, copy the result into a new document yourself.
- **Limited-source route:** narrow the exercise to an approved project folder, selected documents or a completed meeting. A smaller, well-evidenced exercise is better than a confident claim to have reviewed everything.

Check licensing, availability, connected sources and organisational policy with your administrator. This is an adoption method, not a promise of feature parity or unlimited access.

## Change the question from capability to evidence

Instead of asking:

> “Give me ten ways AI can improve my productivity.”

Try asking:

> “From the work I can access, identify repeated tasks and difficult hand-offs. Show the evidence, propose a bounded experiment and tell me what still needs human judgement.”

That change matters. A recommendation becomes useful when you can trace it to something real: a recurring review, a repeated request, a report you maintain or a decision that needs several sources brought together.

An invitation is evidence that a meeting was scheduled—not proof that you attended. A recently opened file is not necessarily a file you created. A document title is not proof of its contents. Ask the assistant to preserve those distinctions.

The output should feel like a mirror of your work, not a catalogue of fashionable AI ideas.

## Look for two kinds of value

### 1. Personal productivity: reduce preparation and reconstruction

These opportunities help you do work you already own. Possible patterns to look for—not findings about every reader—include:

- Rebuilding context before a recurring review.
- Turning a long workshop discussion into a usable follow-up list.
- Finding the requests that genuinely need your input.
- Recreating a status narrative from scattered updates.
- Converting a completed walkthrough into reusable notes.

A good first experiment has a small source set, a clear output and an easy way to check whether it helped.

### 2. Business-process value: improve the quality of a hand-off

The second category is not just “write the same document faster”. It asks where better evidence could improve a business outcome.

Illustrative patterns include checking whether a requirement is supported by an approved design, reconciling conflicting milestone updates, comparing a proposed process against documented controls, or turning reporting fields into clear business definitions.

Keep those examples hypothetical until your own activity supports them. The value may be a clearer decision, an earlier risk signal, a more defensible review or less ambiguity between teams. Minutes saved are only one part of the story.

## The discovery prompt: copy, adapt and test

Use the following prompt in an approved work-connected experience. If you need a narrower exercise, replace the four-week scope with a named project and explicit sources.

```text
Act as my personal AI-workflow coach.

OUTCOME
Discover useful AI applications from my actual recent work, not generic examples.

SCOPE
Review the last four weeks of work information accessible to you for this request: relevant business emails, Teams chats/channels, calendar and meeting material, and documents in OneDrive/SharePoint. State the exact date range used.

If access is narrower, continue using the available sources and clearly describe the coverage and gaps. Do not claim an exhaustive review. Distinguish meeting invitations from attendance, file access from authorship, and proposals from approved decisions.

DELIVER
1. A work profile in 5–7 bullets: evidenced responsibilities, recurring rituals, common deliverables, collaboration patterns and visible work themes. Do not infer actual time allocation or rank colleagues.
2. Five personal-productivity use cases grounded in my activity, if evidence supports five.
3. Three to five higher-value, multi-step use cases that could improve decision quality, controls, collaboration or a business-process hand-off, if evidence supports that many.

For EACH use case include:
- Short name and the work pattern it addresses.
- Exact supporting source title/date and a usable link or section reference.
- Evidence strength and what remains unknown.
- What the assistant would do, step by step.
- Reviewable deliverable(s) and suggested frequency.
- Estimated time saved per occurrence, labelled as an unmeasured hypothesis with its assumptions. Say not estimable where appropriate.
- Value beyond time saved.
- Relative effort: light, medium or heavy. Do not present this as measured credit consumption or a pricing promise.
- Whether scheduling could be suitable IF this experience supports it; do not activate anything.
- A ready-to-run test prompt with a small source set, clear output, human review and the same safety boundaries below.

Recommend my top three quick wins and one high-value experiment to try first. If evidence is insufficient, return fewer use cases and explain why; never invent examples to fill the count.

OUTPUT
If supported, create a NEW document called “My AI Use Cases”. Otherwise provide the same content as a structured response for me to copy into a new document. Describe any output limitation clearly.

BOUNDARIES
Use only sources I am authorised to access. Exclude personal/sensitive information and HR topics such as hiring or performance. Do not evaluate colleagues. Do not send email, messages or invitations; create outgoing drafts; modify existing files or business records; or activate schedules, agents or workflows. Keep every recommendation provisional until I review it. Do not infer approval, ownership or deadlines when they are not explicit.
```

The request is deliberately demanding about evidence and modest about action. Its job is to produce a shortlist you can evaluate—not to automate your working life in one run.

## Turn a recommendation into a safe first experiment

Pick one use case and reduce it until the result is easy to inspect.

“Review all my projects and keep everything up to date” is too broad for a first test. A more useful brief is: “Read one review agenda and its supporting thread, then create a new one-page briefing separating facts, proposals and unanswered questions.”

Define four things before you run it:

1. **Source boundary:** which meeting, thread, documents and dates are in scope?
2. **Output boundary:** what new artefact or structured response should exist at the end?
3. **Decision boundary:** what can the assistant recommend, and what must a person decide?
4. **Stop condition:** what should happen if a source is unavailable, contradictory or incomplete?

For analysis that compares requirements with a standard, the stop condition is particularly important. “No matching evidence retrieved” is not the same as “the capability does not exist”. Keep missing evidence separate from a confirmed gap.

## Measure usefulness before you claim savings

A polished output is not automatically a useful output. Review it against the original task:

- Can you open the promised deliverable?
- Can you verify the important claims against their sources?
- Were material risks or questions missed?
- Were assumptions clearly labelled?
- How much checking and correction did you need?
- Did the result help you make a decision or complete a hand-off?

Record a manual baseline when practical, then include prompting, waiting, review and correction in the assisted comparison. Do not count only the time spent typing.

A large output with an impressive saving estimate can be less useful than a small output you trust. Treat every time-saving estimate as a hypothesis until you test it, and avoid adding overlapping opportunities into a headline weekly total.

## Scheduling is a graduation step, not the opening move

Only consider recurrence after the bounded task works reliably—and only if the chosen experience supports scheduling and your organisation permits it.

A recurring brief needs more than “run this every Friday”. Specify its sources, look-back window, destination, handling of no new information, treatment of missing sources and review boundary. Decide whether each run creates a new private output or follows another explicitly authorised process.

For early experiments, keep the task read-only with respect to source systems and create new outputs only. A recurring evidence check should not quietly become an approval, a message to stakeholders or a business-record update.

## Make the community exchange the method, not the data

The most reusable community asset is not someone’s private report. It is a clear description of the pattern and the conditions under which it worked.

Invite participants to share a sanitised experiment card:

- **Work pattern:** what recurring activity or difficult hand-off did you target?
- **Experience used:** Cowork, an approved Work IQ-enabled experience, or another permitted route.
- **Source types:** for example, a meeting transcript and a design document—without names, links or confidential content.
- **Prompt pattern:** a redacted version that someone else can adapt.
- **Output and review:** what was produced, and how was it checked?
- **Observed result:** measured improvement, useful learning or an honest failure.
- **Limitations:** access gaps, corrections, unsupported features and remaining human decisions.

Before sharing, remove identifying details, tenant links, internal project names, customer information and sensitive operational content. A reusable prompt can travel; the evidence behind it should remain inside its authorised boundary.

Community facilitators can group cards by work pattern rather than job title: preparation, evidence checking, decision support, reporting or knowledge transfer. That makes it easier for another person to recognise a relevant pattern without copying an unsuitable process.

## Your first move

You do not need to discover the most ambitious use case first. You need one real task, enough accessible evidence and a result you can check.

Run the discovery exercise. Challenge anything that feels generic. Pick one quick win. Test one higher-value hand-off. Share what you learned—not your private work data.

**The better question is not “What can AI do?” It is “Which evidenced part of my work is worth testing next?”**

---

## Product references and scope

1. Microsoft Learn, **Copilot Cowork overview**: https://learn.microsoft.com/en-us/copilot/cowork/
2. Microsoft Learn, **Work IQ overview**: https://learn.microsoft.com/en-us/microsoft-365/copilot/extensibility/work-iq/

Product references checked on 7 November 2026. The workflow, prompts, examples and community exercise in this article are proposed adoption practices, not Microsoft feature or pricing commitments. No organisation-specific projects, private correspondence or individual work records are reproduced here.
