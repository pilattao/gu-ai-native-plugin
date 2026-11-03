---
name: finance
description: Use when handling Green Unicorn management reports, plan-versus-actual analysis, project economics, financial models or calculation review.
---
# Finance

Work in the current agent and conversation. Apply [GU policy](../../references/gu-policy.md) and [the shared workflow](../../references/workflow.md); reuse their current confirmed version without repeating bootstrap on direction switches.

Use [adapt-knowledge-work](../adapt-knowledge-work/SKILL.md) for relevant finance/data/reporting methods. Add [adapt-anthropic-financial-services](../adapt-anthropic-financial-services/SKILL.md) only when a specialized model or spreadsheet audit fits. Read selected original methods rather than relying on the direction summary.

Establish reporting entity, business period/calendar, actual versus forecast basis, units, transaction/calculation/presentation currencies, FX basis, taxes within given inputs and metric definitions. Check formulas, signs, totals, reconciliations, zero denominators, dry/wet mass, hardcodes, hidden sheets and sensitivity where relevant. Do not fill missing assumptions with source examples.

Preserve exact inputs and calculation precision; display decimal places do not specify a rounding mode. If rounding depends on an unspecified mode, including a half-way case, leave the final display unresolved or show explicitly conditional comparisons. Do not choose a mode and assert its result as final, even with an assumption caveat. Apply permitted preview preferences separately.

For an FX calculation or fixed/pegged-rate assumption, include an FX reconciliation: original amount/currency, rate/basis/date, fees or commissions, bank spread, exchange differences and net settlement. Mark missing components as unknown; a peg or fixed rate does not make those components zero.

For a mixed marketing/finance task, reconcile spend, revenue, customer/lead and attribution definitions before combining results; preserve one shared context and evidence trail. Deliver source-backed figures, assumptions, explained variances and unresolved gaps in the user's language. Preserve spreadsheet formulas/sheets/styles or disclose losses before approval; release only to the requested stage.
