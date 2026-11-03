# Financial model consistency checks

These are safeguards for selected source methods, not corporate accounting policy, investment advice, currency defaults or a claim that a live workbook was tested. Keep original upstream bytes unchanged. Treat the equations identified below as disputed; use an explicitly derived, validated replacement for the actual model or stop the dependent calculation. State method, units, reporting basis, data and assumptions; retain the source's relevant review limits. Synthetic fixtures illustrate the check and do not establish real GU values.

## Variance bridges

Select a defined bridge/order rather than assuming independently calculated components sum to the full delta. For one product, let baseline quantity/price be Q0/P0 and actual Q1/P1. A baseline-price/quantity decomposition gives volume `(Q1-Q0)*P0`, price `Q0*(P1-P0)` and interaction `(Q1-Q0)*(P1-P0)`. Alternatively, a sequential bridge can assign price at actual quantity; do not also add that interaction. Multiple-product mix, FX, new/discontinued items, period effects and rounding require explicit treatment. Compare bridge sum to observed total and retain unexplained residual for investigation.

State the compared metric's meaning from the task or applicable data definition: revenue, cost or another defined measure. If that meaning is absent, label it an unclassified quantity-times-price amount and report the numerical delta without assigning revenue/cost or favorable/adverse meaning. Source and fixture labels do not supply that missing business definition; supported arithmetic and lineage can still proceed.

Fixture: Q0=10, P0=2, Q1=12, P1=3. Baseline amount 20, actual 36, delta 16. Baseline volume 4 plus baseline price 10 totals 14; interaction is 2. A valid sequential bridge is volume 4 plus actual-quantity price 12 = 16. The upstream variance-analysis equations must not conceal the missing 2. These numbers alone classify neither revenue/cost nor favorability.

## DCF capital weights and enterprise/equity bridge

The selected dcf-model Step 6/WACC instructions use net debt for capital weighting; that can generate a negative debt weight in a net-cash company. Do not adopt it automatically. Establish justified market-equity and gross interest-bearing-debt values/weights consistent with the valuation basis, tax assumptions and discount-rate method. Cash belongs in a separately justified enterprise-to-equity bridge (with other applicable claims/non-operating assets), rather than silently reducing debt weight. Validate nonnegative normalized weights where that model requires them, cash-flow/discount-rate consistency, date/currency, terminal growth versus discount rate (invalid g >= WACC cases require explicit handling), and sensitivity formulas, including base-case reconciliation and full scenario recomputation. If another methodology is proposed, explain and validate it rather than swapping equations silently.

Fixture: market equity 1,000, gross interest-bearing debt 100, cash 300. A gross-capital basis gives E/(D+E)=1,000/1,100 and D/(D+E)=100/1,100; the debt weight is positive. Net debt is -200 and must not become a negative capital weight. Under a simple bridge with no other claims, equity value = EV + 300 - 100; real bridges require their actual adjustments.

## Integrated statements, NOL and SBC

The selected 3-statement-model equations add stock-based compensation to retained earnings after NI already reflects its expense and subtract NOL utilization before deriving NI. Do not copy those equations. Separate book pretax income, taxable-income/NOL schedules, current/deferred tax expense and cash taxes according to the applicable specified accounting/tax basis. NOL use is not automatically another book operating expense. Reconcile net income to the income statement and retained earnings as opening retained earnings + NI - distributions plus justified applicable adjustments. Trace SBC expense, noncash cash-flow addback and APIC/equity treatment separately, avoiding double count. Establish the actual award/accounting facts rather than assuming universal SBC treatment.

Fixture: opening retained earnings 100, reported NI 20 already after SBC expense, dividends 5 gives closing retained earnings 115 before any other justified adjustment, not 125 merely because SBC was 10. A 10 SBC cash-flow addback/APIC movement, where applicable, is tested separately. A tax fixture with pretax book income 30, taxable income before NOL 30, allowable NOL use 10 and current-tax rate 20% gives taxable income 20/current tax 4; do not subtract 10 directly from pretax book income to manufacture NI. Book tax expense/NI require the specified deferred-tax and accounting assumptions.

## Workbook acceptance

Scope the audit to selection/sheet/model as actually examined. Verify source-linked assumptions, formulas rather than pasted projections, recalculation/cached-value reliability, balance-sheet balance, cash tie-out, retained-earnings/debt/asset roll-forwards, signs, circularity, hidden tabs, external links and scenario/sensitivity dependencies. Never cure an imbalance with an unexplained plug. Ground-truth checks test meaning and expected numbers, not only workbook styling. Never report recalculation or full-model validation when the accepted host lacks that capability; disclose the exact gap before delivery/release.
