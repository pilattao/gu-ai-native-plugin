---
name: adapt-anthropic-financial-services
description: Use when a Green Unicorn finance task requires an integrated three-statement model, discounted cash-flow valuation or spreadsheet/model audit.
---
# Financial-services adapter

Apply [GU policy](../../references/gu-policy.md) and [the shared workflow](../../references/workflow.md) independently, even when called directly. Read them if absent or changed; reuse current confirmed context and identity. Continue in the current agent. Use [the knowledge-work base](../adapt-knowledge-work/SKILL.md) when the task also requires statements, reconciliation, reporting or data validation; this adapter adds specialized modeling methods.

## Select exact original methods

[Source provenance](../../upstream/sources.json) binds pinned originals and licenses. Read the applicable source and included dependencies:

| Need | Original |
|---|---|
| Populate/link an existing integrated framework | [3-statement-model](../../upstream/financial-services/plugins/vertical-plugins/financial-analysis/skills/3-statement-model/SKILL.md) |
| Forecast cash flows, valuation and sensitivity | [dcf-model](../../upstream/financial-services/plugins/vertical-plugins/financial-analysis/skills/dcf-model/SKILL.md) |
| Scoped formula/sheet/full-model integrity review | [audit-xls](../../upstream/financial-services/plugins/vertical-plugins/financial-analysis/skills/audit-xls/SKILL.md) |

## Map inputs and execution assumptions

Use task-provided or authorized accessible statements, forecasts, assumptions and market inputs through public Core. Bloomberg, FactSet, SEC/research retrieval and other source-tool examples do not authorize connections or undeclared network reads. Mark date, source and verification of valuation inputs. Missing evidence is not an invitation to invent market data, taxes or rates.

Map upstream staged confirmations to the requested task: when the user requests a complete draft and supplies the material assumptions, perform the method's intermediate checks and finish the available draft without pausing for repeated approval of inputs or derived numbers. Reuse confirmed inputs; disclose any material missing data or conflict and stop only its dependent calculation. Follow an explicitly requested step-by-step mode. Source checkpoints do not create extra human approval barriers; actual mutations, publication, reporting/filing and professional sign-off retain their applicable authorization and review requirements.

Map Office JS/openpyxl/recalc.py examples to the accepted installed host spreadsheet capability and real sandbox; do not install/run a second parser, provider, script dependency or upstream harness automatically. Preserve formula-driven projections, linked assumptions, source comments, scenario logic and recalculation requirements. If formulas cannot be recalculated/verified or workbook features cannot be preserved, report that exact blocked capability; writing formulas alone is not verified calculation.

## Mandatory equation review

Apply [financial model consistency checks](../../references/financial-model-checks.md) before using source equations. The dcf-model net-debt WACC weights and the 3-statement retained-earnings/SBC/NOL equations are disputed. Use justified market-equity/gross-debt weights and a separate cash bridge where applicable; separate book NI from taxable income and SBC/APIC/noncash movements. Proceed only with explicitly corrected, validated calculations; no silent copying or edits to originals.

Establish entity, business date/period, units, accounting basis, currency/FX, transaction versus presentation amounts and assumptions. Run source-appropriate balance/cash/roll-forward, units/signs, circularity, external-link, scenario and sensitivity checks. Test expected numbers and meaning independently; no source example or default horizon becomes GU policy. Preserve applicable professional review before financial reporting, filing or sign-off.

For an audit, report findings with sheet/cell/range and severity first; do not change the workbook without a corresponding fix request. Deliver the requested model/audit with source lineage, assumptions, corrected-method rationale, actual audit coverage, checks and unresolved limitations. Observation, forecast and valuation estimate remain distinct. A draft model is not financial approval or a release; write/recovery/final readback follow the shared workflow.
