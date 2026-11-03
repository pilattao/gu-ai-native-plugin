---
name: adapt-anthropic-legal
description: Use when a Green Unicorn contract task needs structured agreement review, NDA triage, SaaS terms analysis or an escalation draft.
---
# Legal-method adapter

Apply [GU policy](../../references/gu-policy.md) and [the shared workflow](../../references/workflow.md) independently, including direct invocation. Read them if absent or changed; reuse current confirmed context. Use the current agent and conversation, not source agents/matter-workspace machinery.

## Select exact original methods

Read the relevant pinned originals and included dependencies, bound by [source provenance](../../upstream/sources.json):

| Need | Original |
|---|---|
| Identify agreement structure and integrate reviews | [review](../../upstream/anthropic-legal/commercial-legal/skills/review/SKILL.md) |
| General vendor terms, liability/indemnity and data clauses | [vendor-agreement-review](../../upstream/anthropic-legal/commercial-legal/skills/vendor-agreement-review/SKILL.md) |
| Playbook-based confidentiality triage | [nda-review](../../upstream/anthropic-legal/commercial-legal/skills/nda-review/SKILL.md) |
| Subscription/renewal/price/data-exit/SLA overlay | [saas-msa-review](../../upstream/anthropic-legal/commercial-legal/skills/saas-msa-review/SKILL.md) |
| Match issue to an actual authority matrix; draft ask | [escalation-flagger](../../upstream/anthropic-legal/commercial-legal/skills/escalation-flagger/SKILL.md) |

The vendor-agreement-review dependency supplies general contract checks underlying review/SaaS; read its original when selected. A source reference to another method outside the reviewed selection is a gap, not permission to install or improvise a purported full review.

## Map playbook, matter and tools

Map source `~/.claude/.../CLAUDE.md`, playbook, matter.md, side/positions, house style and authority matrix to applicable installed GU rules plus explicitly supplied, accessible task context. Do not run cold-start-interview, create a source config/matter workspace, import another matter or permanently save a new corporate position automatically. Record task-only decisions with scope; permanent defaults/approvers require the Plugin policy-change process. If the relevant side, term position or matrix is missing, state the gap and obtain necessary task input before claiming playbook conformance or naming an approver.

Map Drive/CLM/legal-research/destination placeholders only to actual public Core capabilities and authorized task data. No new connector, hidden web/model-knowledge supplement, provider or research subscription. Preserve original source labels and “verify” caveats. Thin legal-source coverage is disclosed and blocks the dependent current-law conclusion; use provided primary evidence or a separately authorized supported retrieval path rather than inventing citations.

## Review and output contract

Route by main/exhibit titles before clause keywords and state coverage, missing annexes and routed methods. Adapt the source's confirm_routing default to the authorized task: choose the applicable reviewed route and state its scope, using an explicit task routing decision when supplied. Ask only when unresolved routing or matter ambiguity materially changes the legal analysis or external effect. Ordinary authorized review needs no separate route-confirmation stop; method transparency is distinct from mutation approval. Integrate applicable methods into one review; preserve separate legal-risk and business-impact severity when the source method calls for them. Establish sales/purchasing side, governing law, venue, parties/authority, performance place, dates and language/amendment priority; jurisdiction-specific examples apply only when verified.

Preserve source method limits: NDA triage is sorting, not negotiation or substantive drafting. Complex NDA restructuring/new language goes to Legal; simple mechanical changes may be shown within that method. GREEN means no identified playbook flags in examined scope, never permission to sign. SaaS overlays retain general vendor checks, legal-source/jurisdiction caveats and liability-cap decision review. Missing expertise does not prohibit a separately permissible clearly scoped draft.

Privilege/confidentiality markings depend on applicable jurisdiction, purpose, recipients and reviewed playbook; the source template's default header/removal language is not GU policy. A header cannot guarantee privilege, and destination changes require reassessing disclosure rather than applying universal waiver claims. Preserve signed originals and meaningful clause context/comments/tracked changes or disclose losses before approval.

Produce the requested analysis or draft with quoted terms, supported interpretation, deviations, rationale, meaningful diff and unresolved expert decisions distinguished. Escalation drafts identify only an actual applicable matrix owner; if none exists, report missing authority. **Do not send** escalation messages. Draft/review, publication and signing are separate actions; source acceptance labels and approval text do not authorize mutations. All permitted writes and recovery follow the shared workflow.
