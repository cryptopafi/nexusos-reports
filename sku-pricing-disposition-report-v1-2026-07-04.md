# RUO SKU Pricing And Disposition Tables v1

Generated: 2026-07-04 00:20 EEST

## Owner Decisions Applied
- D1: Controlled Continue default
- D2: High-risk SKUs sell only as yellow/counsel-review when otherwise eligible
- D3: Green only with public/verified COA
- D4: Strict margin gate
- D5: Restock only if COA-economic
- D6: RUO-safe public copy only
- D7: Existing stock without verified COA is hold
- D8: Verified COA means independent/public, batch-linked where possible
- D9: 60% minimum margin after COA + discount/commission/CAC reserve
- D10: Build v1 now from available data with gaps marked

## Summary
- rows: 31
- green: 0
- yellow: 12
- red: 11
- grey: 8
- verified_coa: 12
- hold_until_verified_coa: 11
- reorder_focus_or_blocked: 3

Interpretation: this is a control table, not a sales recommendation. Per Pafi, existing stock without verified independent/public COA is hold/red. High-risk SKUs with verified COA can remain controlled/yellow under counsel review. Green requires verified COA, strict 60% margin, and RUO-safe copy.

## Files
- Pricing/margin CSV: `sku-pricing-margin-table-v1-2026-07-04.csv`
- Disposition CSV: `sku-disposition-table-v1-2026-07-04.csv`
- Machine summary: `sku-pricing-disposition-summary-2026-07-04.json`

## Red / Hold Rows
| SKU | Disposition | COA | Margin | Issues |
|---|---|---|---|---|
| 5AMINO1MQ-50MG | hold_until_verified_coa | coa_review_hold_quantity_only | yellow_below_60_fix_by_reprice_or_reserve_cap | verified_public_coa_missing_or_incomplete; strict_margin_not_green; public copy waits Vic/lawyer pass; SS_HEURISTIC |
| AOD9604-5MG | hold_until_verified_coa | hold_no_verified_public_coa | yellow_below_60_fix_by_reprice_or_reserve_cap | verified_public_coa_missing_or_incomplete; strict_margin_not_green; counsel_review; AOD 5mg/10mg historical drift + label task open; public copy waits Vic/lawyer pass; PERSONAL_USE_SKEW; NO_RECENT_CUSTOMER_DEMAND; SS_HEURISTIC |
| BAC-10ML | hold_until_verified_coa | hold_no_verified_public_coa | yellow_below_60_fix_by_reprice_or_reserve_cap | verified_public_coa_missing_or_incomplete; strict_margin_not_green; counsel_review; public copy waits Vic/lawyer pass; SS_HEURISTIC |
| CJC1295-5MG | hold_until_verified_coa | hold_no_verified_public_coa | yellow_below_60_fix_by_reprice_or_reserve_cap | verified_public_coa_missing_or_incomplete; strict_margin_not_green; counsel_review; public copy waits Vic/lawyer pass; PERSONAL_USE_SKEW; NO_RECENT_CUSTOMER_DEMAND; SS_HEURISTIC |
| GLUTATHIONE-1500MG | hold_until_verified_coa | hold_no_verified_public_coa | yellow_below_60_fix_by_reprice_or_reserve_cap | verified_public_coa_missing_or_incomplete; strict_margin_not_green; public copy waits Vic/lawyer pass; PERSONAL_USE_SKEW; SS_HEURISTIC |
| NAD+-500MG | hold_until_verified_coa | hold_no_verified_public_coa | yellow_below_60_fix_by_reprice_or_reserve_cap | verified_public_coa_missing_or_incomplete; strict_margin_not_green; public copy waits Vic/lawyer pass; SS_HEURISTIC |
| PT141-10MG | hold_until_verified_coa | hold_no_verified_public_coa | yellow_below_60_fix_by_reprice_or_reserve_cap | verified_public_coa_missing_or_incomplete; strict_margin_not_green; counsel_review; public copy waits Vic/lawyer pass; PERSONAL_USE_SKEW; NO_RECENT_CUSTOMER_DEMAND; SS_HEURISTIC |
| SELANK-10MG | hold_until_verified_coa | hold_no_verified_public_coa | yellow_below_60_fix_by_reprice_or_reserve_cap | verified_public_coa_missing_or_incomplete; strict_margin_not_green; public copy waits Vic/lawyer pass; NO_RECENT_CUSTOMER_DEMAND; SS_HEURISTIC |
| SEMAX-10MG | hold_until_verified_coa | hold_no_verified_public_coa | yellow_below_60_fix_by_reprice_or_reserve_cap | verified_public_coa_missing_or_incomplete; strict_margin_not_green; public copy waits Vic/lawyer pass; NO_RECENT_CUSTOMER_DEMAND; SS_HEURISTIC |
| THYMOSINALPHA1-10MG | hold_until_verified_coa | hold_no_verified_public_coa | yellow_below_60_fix_by_reprice_or_reserve_cap | verified_public_coa_missing_or_incomplete; strict_margin_not_green; public copy waits Vic/lawyer pass; PERSONAL_USE_SKEW; NO_RECENT_CUSTOMER_DEMAND; SS_HEURISTIC |
| VIP-10MG | hold_until_verified_coa | hold_no_verified_public_coa | yellow_below_60_fix_by_reprice_or_reserve_cap | verified_public_coa_missing_or_incomplete; strict_margin_not_green; public copy waits Vic/lawyer pass; PERSONAL_USE_SKEW; NO_RECENT_CUSTOMER_DEMAND; SS_HEURISTIC |

## Yellow / Controlled Review Rows
| SKU | Disposition | COA | Margin | Restock | Issues |
|---|---|---|---|---|---|
| BPC157-5MG | continue_controlled_margin_review | verified_public_batch_linked | yellow_below_60_fix_by_reprice_or_reserve_cap | no_restock_now | strict_margin_not_green; counsel_review; public copy waits Vic/lawyer pass; SS_HEURISTIC |
| EPITHALON-10MG | continue_controlled_margin_review | verified_public_batch_linked | yellow_below_60_fix_by_reprice_or_reserve_cap | no_restock_now | strict_margin_not_green; public copy waits Vic/lawyer pass; SS_HEURISTIC |
| GHKCU-50MG | continue_controlled_margin_review | verified_public_batch_linked | yellow_below_60_fix_by_reprice_or_reserve_cap | no_restock_now | strict_margin_not_green; public copy waits Vic/lawyer pass; SS_HEURISTIC |
| IPAMORELIN-5MG | continue_controlled_margin_review | verified_public_batch_linked | yellow_below_60_fix_by_reprice_or_reserve_cap | no_restock_now | strict_margin_not_green; counsel_review; public copy waits Vic/lawyer pass; SS_HEURISTIC |
| KISSPEPTIN10-5MG | continue_controlled_margin_review | verified_public_batch_linked | yellow_below_60_fix_by_reprice_or_reserve_cap | no_restock_now | strict_margin_not_green; public copy waits Vic/lawyer pass; PERSONAL_USE_SKEW; SS_HEURISTIC |
| KPV-10MG | continue_controlled_margin_review | verified_public_batch_linked | yellow_below_60_fix_by_reprice_or_reserve_cap | no_restock_now | strict_margin_not_green; public copy waits Vic/lawyer pass; SS_HEURISTIC |
| MELANOTAN2-10MG | continue_controlled_margin_review | verified_public_batch_linked | yellow_below_60_fix_by_reprice_or_reserve_cap | no_restock_now | strict_margin_not_green; counsel_review; public copy waits Vic/lawyer pass; PERSONAL_USE_SKEW; SS_HEURISTIC |
| MOTSC-10MG | continue_controlled_margin_review | verified_public_batch_linked | yellow_below_60_fix_by_reprice_or_reserve_cap | reorder_focus_coa_economic | strict_margin_not_green; counsel_review; public copy waits Vic/lawyer pass; PERSONAL_USE_SKEW; SS_HEURISTIC |
| RETATRUTIDE-10MG | continue_controlled_margin_review | verified_public_batch_linked | yellow_below_60_fix_by_reprice_or_reserve_cap | transfer_first_no_purchase | strict_margin_not_green; counsel_review; public copy waits Vic/lawyer pass; SS_HEURISTIC |
| RETATRUTIDE-30MG | parked_no_stock_until_coa_margin_decision | verified_public_batch_linked | unknown | parked_no_stock_no_restock | strict_margin_not_green; counsel_review; public copy waits Vic/lawyer pass; FORECAST_IS_LOWER_BOUND; SS_HEURISTIC; PERSONAL_USE_SKEW; PARKED_OUT_OF_STOCK |
| TB500-5MG | continue_controlled_margin_review | verified_public_batch_linked | yellow_below_60_fix_by_reprice_or_reserve_cap | no_restock_now | strict_margin_not_green; counsel_review; public copy waits Vic/lawyer pass; SS_HEURISTIC |
| TESAMORELIN-10MG | continue_controlled_margin_review | verified_public_batch_linked | yellow_below_60_fix_by_reprice_or_reserve_cap | reorder_focus_coa_economic | strict_margin_not_green; counsel_review; public copy waits Vic/lawyer pass; SS_HEURISTIC |

## Grey / Parked Rows
| SKU | Disposition | Reason |
|---|---|---|
| CEREBROLYSIN-60MG | parked_no_stock_until_coa_margin_decision | verified_public_coa_missing_or_incomplete; strict_margin_not_green; public copy waits Vic/lawyer pass; FORECAST_IS_LOWER_BOUND; SS_HEURISTIC; PERSONAL_USE_SKEW; PARKED_OUT_OF_STOCK |
| CJC1295DAC-5MG | parked_no_stock_until_coa_margin_decision | verified_public_coa_missing_or_incomplete; strict_margin_not_green; counsel_review; public copy waits Vic/lawyer pass; FORECAST_IS_LOWER_BOUND; SS_HEURISTIC; PERSONAL_USE_SKEW; PARKED_OUT_OF_STOCK |
| DSIP-10MG | parked_no_stock_until_coa_margin_decision | verified_public_coa_missing_or_incomplete; strict_margin_not_green; public copy waits Vic/lawyer pass; FORECAST_IS_LOWER_BOUND; SS_HEURISTIC; PARKED_OUT_OF_STOCK |
| FOXO4-10MG | parked_no_stock_until_coa_margin_decision | verified_public_coa_missing_or_incomplete; strict_margin_not_green; public copy waits Vic/lawyer pass; FORECAST_IS_LOWER_BOUND; SS_HEURISTIC; PERSONAL_USE_SKEW; PARKED_OUT_OF_STOCK |
| IGF1LR3-1MG | parked_no_stock_until_coa_margin_decision | verified_public_coa_missing_or_incomplete; strict_margin_not_green; counsel_review; public copy waits Vic/lawyer pass; FORECAST_IS_LOWER_BOUND; SS_HEURISTIC; PERSONAL_USE_SKEW; PARKED_OUT_OF_STOCK |
| SLUPP332-5MG | parked_no_stock_until_coa_margin_decision | verified_public_coa_missing_or_incomplete; strict_margin_not_green; public copy waits Vic/lawyer pass; FORECAST_IS_LOWER_BOUND; SS_HEURISTIC; PERSONAL_USE_SKEW; PARKED_OUT_OF_STOCK |
| SS31-10MG | parked_no_stock_until_coa_margin_decision | verified_public_coa_missing_or_incomplete; strict_margin_not_green; public copy waits Vic/lawyer pass; FORECAST_IS_LOWER_BOUND; SS_HEURISTIC; PERSONAL_USE_SKEW; PARKED_OUT_OF_STOCK |
| TIRZEPATIDE-10MG | parked_no_stock_until_coa_margin_decision | verified_public_coa_missing_or_incomplete; strict_margin_not_green; counsel_review; public copy waits Vic/lawyer pass; FORECAST_IS_LOWER_BOUND; SS_HEURISTIC; PERSONAL_USE_SKEW; PARKED_OUT_OF_STOCK |

## Important Notes
- `P0-006` table uses strict margin after VAT, economic COA allocation, and 30% public-price reserve for discount/commission/CAC.
- `P0-007` disposition table applies the COA hold rule before commercial judgement.
- BAC Water is treated as quality-proof blocked until appropriate sterile/BAC-water documentation exists; Janoshik peptide COA is not the right evidence type for BAC.
- AOD9604 remains blocked by no verified public COA plus 5mg/10mg historical drift and open label task.
- Website copy remains yellow globally until Vic/lawyer pass confirms RUO-safe public copy.
