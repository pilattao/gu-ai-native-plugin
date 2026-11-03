---
name: adapt-knowledge-work
description: Use when a Green Unicorn task needs financial statements, reconciliation, variance analysis, data validation, charts or marketing performance reporting.
---
# Knowledge-work adapter

Apply [GU policy](../../references/gu-policy.md) and [the shared workflow](../../references/workflow.md) independently, including on a direct invocation. Load them if absent or their installed version changed; reuse confirmed context. Use the current agent. This is the shared finance/data/marketing base; specialist adapters supplement the selected method rather than replacing common evidence and validation.

## Select exact original methods

Read only applicable pinned originals and included dependencies; [source provenance](../../upstream/sources.json) binds exact revisions/hashes and licenses. Source commands are methodological references, not new executable entrypoints.

| Need | Selected original |
|---|---|
| Period statements, comparisons, adjustments | [financial-statements](../../upstream/knowledge-work/finance/skills/financial-statements/SKILL.md) |
| GL/subledger/bank/intercompany comparison | [reconciliation](../../upstream/knowledge-work/finance/skills/reconciliation/SKILL.md) |
| Plan/actual drivers and variance narrative | [variance-analysis](../../upstream/knowledge-work/finance/skills/variance-analysis/SKILL.md) |
| Query/data/result quality and completeness | [validate-data](../../upstream/knowledge-work/data/skills/validate-data/SKILL.md) |
| Task-appropriate, accessible charts | [data-visualization](../../upstream/knowledge-work/data/skills/data-visualization/SKILL.md) |
| Campaign/channel/period metrics and recommendations | [performance-report](../../upstream/knowledge-work/marketing/skills/performance-report/SKILL.md) |

## Map context and tools

Map `~~erp`, `~~data warehouse`, `~~marketing analytics`, `~~product analytics`, database/query and collaboration placeholders to task-provided data and the actual accessible Drive/Docs/Sheets capabilities discovered through public Core. `CONNECTORS.md` is vocabulary, not connection permission. Do not connect another service, run SQL against an undiscovered database, install chart/parser software or invoke a provider. If only a workbook/CSV extract is available, scope validation to it; do not claim warehouse-wide checks. Apply chart examples only through the accepted installed host capability.

Establish entity, periods, units, currencies/FX, accounting/reporting basis, materiality and comparison definitions from applicable policy/task input. Source USD, GAAP/IFRS references, numerical thresholds, attribution defaults and benchmark ranges are examples or context-sensitive methodology; none becomes GU policy or current authoritative accounting guidance automatically. Preserve qualified financial review before reporting/filing or reconciliation sign-off.

## Domain validation and result

Use the selected method's quality checks and meaningful caveats. Check full covered ranges, duplicates, missing data, join cardinality/filters where relevant, outliers, zero denominators, signs, FX, chart labels/axes and source dates. Reconcile totals to source and distinguish explanation from causal hypothesis. Treat reasonableness bounds contextually: legitimate returns/credits can make revenue negative, and growth percentages can exceed 100%; investigate rather than force an example range. Define conversion/customer, spend/revenue, attribution window/model and ROI/ROAS before mixing finance and marketing. A source's revenue/cost ratio labelled “ROI” is not silently interchangeable with net-return ROI.

The variance-analysis price/volume/mix equations are not universally additive. Choose and state a decomposition, preserve interaction/mix/residual explicitly and reconcile the complete observed delta. See [financial consistency checks](../../references/financial-model-checks.md). Never force an unexplained residual to zero or copy disputed equations blindly.

Deliver the requested statement/reconciliation/report/chart with sources, definitions, coverage, assumptions, checks and unresolved items. Label forecasts and causal claims appropriately; sample-size/benchmark advice does not prove certainty. Missing data or tools blocks the dependent method, with the precise gap disclosed; continue supported analysis. All artifacts, unknowns, writes and memory use remain under the shared workflow.
