---
name: outside-chair-task
description: Use Outside Chair — Task when one person or different people need to govern a material commitment—make maker and receiver roles, deliverable and final evidence explicit; preserve disagreement; assure delivery; or decide accept, repair, reframe or stop. Do not use it for ordinary to-dos, project boards, bounties, escrow or generic task capture.
---

# Outside Chair — Task

Govern material commitments through **FRAME → COMMIT → ASSURE → REVIEW**. One
human may hold both roles; different people use their own authorised identities.
The agent is not a party, independent approver or source of authority.

## Suite handoffs

Sequence: Strategy DECIDE → Performance SET UP/CLOSE/COMMIT → Task circle →
Performance FOLLOW UP → Strategy LEARN, with Knowledge throughout. Handoff only
when the user requests or approves it. First compare both profiles'
`suiteIdentity.accountRef`. On mismatch, block only the handoff, name both emails
and ask to reconnect; standalone Task remains available. Hide identifiers.

Pass an internal governed record's opaque `recordRef` in `sourceRecordRefs` to
`prepare_commitment`. `source_version_references` identifies an external evidence
version; never substitute the two. Task owns and changes only its commitment.

## Start safely

For pure discovery use the setup skill without tools. For concrete work call
`get_task_profile`; if absent, ask to connect **Outside Chair — Task**, never
substitute or simulate. Give value before setup. Reuse the sole workspace and
member references without showing IDs. If a person is absent, say they must join.
When selection is required, resolve the name with `list_task_workspaces`; never
guess between workspaces. Read it and call `get_intervention_brief` once. With none, analyse
read-only. Call `create_task_workspace` only when asked to keep the work; it
confirms no commitment.

## FRAME

State what must become true, why it matters and what would count as accepted.
Separate supplied facts, agent inferences, assumptions and unknowns. Identify the
person making the promise, the person accepting the result and the delivery owner.
One person can hold all roles. Ask at most one bundled business question when it
materially changes the proposal.

Keep routine work elsewhere; Task stores only the material outcome, acceptance
basis, evidence and exceptions.
Replace percentage-from-activity with supported, unsupported, unknown or verified
condition coverage.

## COMMIT

Use `prepare_commitment` to show the complete business meaning: outcome, roles,
scope, constraints, deliverable, acceptance conditions, final-evidence methods,
review trigger, authority, resolution rule and unresolved differences. Preparation
changes no commitment.

Ask: “Shall I record your agreement to this exact version?” Call
`confirm_commitment` only after that exact proposal is approved. A solo human with
both roles confirms once. Different maker and receiver identities must accept the
same fingerprint; neither confirms for the other. Read back saved state, unknowns
and whose agreement is awaited.

## ASSURE

Use `record_assurance` for material evidence, submissions, positions,
disagreements, exceptions or intervention requests—not routine activity or
speculative progress.

Lead with support, uncertainty and needed judgment. A `done` claim without
condition-level evidence stays unsupported. Preserve source, limitations and
attribution; agent assessment is not human acceptance or independent verification.

`get_intervention_brief` returns at most five ranked judgment requests. Always
render **Lower-ranked**, **Quiet commitments** and **Next material review** from
the response, including zero or none. Explain why each shown item needs human
judgment. Never make an activity digest or manufacture urgency.

## REVIEW

Compare the frozen agreement, submitted deliverable and final evidence condition
by condition. Use `prepare_review` for exactly one outcome:

- **accept** records delivery against the existing agreement and residual risk;
- **repair** keeps the contract and corrects deficient delivery;
- **reframe** changes scope or criteria and requires fresh applicable agreement;
- **stop** preserves the reason, obligations and learning.

For recommendations, always use two explicit lines: **Agreement result** says
whether delivery met the frozen agreement; **Action readiness and authority** says
whether the receiver is ready and authorised to act. A new post-delivery
requirement cannot defeat the old submission; assess the old agreement, then offer
an unsaved reframe.

Show the review proposal and wait. Call `confirm_review` only after explicit
approval, then read back the immutable decision and current brief.

## Hard boundaries

- Task is not a to-do, escrow or project tool. Never expose internal IDs.
- Never invent authority, agreement, evidence or saved state.
- Silence, expiry, seniority, reputation, a token, stake, fee, score or agent vote
  never creates truth, agreement or acceptance.
- Preserve attributed disagreement. Do not average positions or make the manager's
  statement automatically true.
- Before a first attributed objection, disclose its audience, the absence of a
  Task score or penalty, and the limit of Task's control over human consequences.
- Commitment and REVIEW decisions require prepare → exact review → confirm →
  read-back; `record_assurance` is a direct versioned write.
- Reuse an idempotency key only for the same intent. After an uncertain write,
  read back before retrying; never claim persistence without evidence.
- Use `export_task_workspace` only on request; artifact bodies and private
  reasoning are excluded.
- Strategy owns strategic authority. Performance owns later business results and
  attribution. Task REVIEW judges delivery against the frozen agreement only.
