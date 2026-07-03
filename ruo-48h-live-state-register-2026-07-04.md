# RUO 48h Live-State Register

Generated: 2026-07-04 00:05 EEST  
Owner: Pafi  
Scope: 48-hour operating state snapshot. This is a status register, not a freeze.
Public copy: https://cryptopafi.github.io/nexusos-reports/ruo-48h-live-state-register-2026-07-04.md

## Executive State

| Area | State | Owner | Next action | Evidence / linked task |
|---|---|---|---|---|
| D2C peptide sales | Live, controlled | Pafi | Continue only inside current RUO/compliance-safe flow; no expansion until compliance gates clear. | Dashboard owner override; `P0-001` Website Compliance |
| Paid ads | Not running | Pafi | Keep paused until website/compliance and SKU disposition are cleared. | Dashboard owner override |
| Website compliance | Waiting / blocked on lawyer opinion | Vic | Prepare correction map and evidence only; no new site modifications until lawyer gives boundaries. | `P0-001`, `P0-0-004` |
| High-revenue / high-risk SKUs | Continue selling only under current lawyer-approved RUO copy model | Pafi + Vic compliance gate | Remove/avoid treatment, dosing, injection, healing, fat-loss, before/after, protocol, and medical-benefit claims from public surfaces. | `P0-001`, `P0-007` |
| Dragos collaborator sales | Not active as collaborator channel | Dragos / Pafi | Keep Dragos work inside operating contract, referral mapping, evidence, and order/handoff controls. | `P1-006` done; `P1-019` open |
| Supabase/dashboard | Active operating layer | Narcis | Continue as operating source for SKU, stock, orders, payments, approvals, COA/SDS, and evidence links. | `P0-0-006` done |
| Supabase writes by Codex/Pafi agents | Blocked unless explicitly Pafi-authorized | Pafi / Codex / Narcis | Any write must use Pafi authorization, audit markers, and same-transaction `set local app.actor='Pafi'`. | `P0-0-006`, RUO Supabase guardrail |
| Airtable | Frozen / read-only legacy source | Pafi + Narcis | Use only for historical evidence and reconciliation; no new operational writes. | `P0-010` done |
| Accessories | Waiting for proof/QC and separate business plan | Pafi | Build the standalone Accessories Business plan covering compliance, products/SKUs, purchasing, proof/QC, workflows, marketing/sales, logistics, and budget/P&L. | `P0-008`, `P2-004` |
| AOD9604 website strength | Done | Narcis | No action unless regression appears. | `P0-011` done |
| AOD9604 labels | Open / yellow | Narcis | Re-order/reprint 5 mg labels with new supplier and prevent 10 mg labels from being used on 5 mg stock. | `P0-012` |
| SO-04 restock | Ordered / in transit / not received | Narcis | Enforce delivery receipt gate: batch number and COA required before stock acceptance, customer dispatch, or sale-ready status. | `P0-014` |
| Ibiza 69-vial transfer | In transit / not sellable | Narcis | Confirm physical receipt and recount; until then treat as not sellable. | `P0-013` |
| Sultan client orders | Prepared / done | Pafi | Dispatch only after Ibiza stock is refilled with Bucharest in-transit transfer and proper handoff evidence exists. | `P0-017` done |
| Sultan owner entry | Plan done, external decision pending | Pafi | If Sultan approves, onboarding starts; if not, do not start. | `P0-016` done |
| Next Pafi-only restock | Open / needs COA-corrected economics | Pafi | Supersede the old USD 868 recommendation until COA cost, FX, and margin economics are correctly applied. | `P0-018` |
| Pricing and margin truth | Open / yellow | Pafi | Complete canonical SKU pricing/margin table in dashboard/admin with supplier cost, landed cost, public price, margin, discount/promoter/CAC cap, reorder status, counsel flag, and active copy status. | `P0-006` |
| SKU disposition | Open / yellow | Pafi | Classify every SKU by continue, cleanup, COA needed, margin review, reorder focus, counsel review, or inbound-B2B support. | `P0-007` |
| Wholesale / dropshipping lane | Open | Pafi | Define controlled service lane, eligible products, pricing tiers, payment terms, fulfillment responsibility, evidence/COA handling, and compliance-safe copy. | `P1-012` |
| Affiliate/referral engine | Planned, not active | Narcis | Build only after rules/compliance and economics are approved. | `P1-015` |
| Customer referral tree | Open / yellow | Dragos primary, Narcis support | Map every customer/order to root account Pafi, Narcis, Vic, Dragos, or Sultan; do not guess unknowns. | `P1-019` |
| Hermes Telegram group agent | Open | Narcis | Integrate Hermes into the shared Telegram group for stock-management and peptide/supplement protocol workflows. | `P1-011` |
| RUO Slack workspace + Hermes | Open / yellow | Vic | Create workspace; attach Hermes only read-only/draft-first with Supabase/PepInternal least-privilege access. | `P1-018` |
| Daily export/checksum backup | Done | Narcis | Keep as proof-control layer for dashboard-critical tables. | `P1-010` done |

## 48h Control Readout

Green / live:
- D2C is live, but controlled.
- Supabase/dashboard is the active operating layer.
- Airtable is frozen as read-only legacy evidence.
- AOD9604 website strength correction is done.
- Sultan order prep and Sultan owner-entry plan are done at internal-planning level.
- Daily export/checksum backup is done.

Yellow / active risk or incomplete:
- Pricing/margin truth is still not complete in a canonical table.
- SKU disposition is still open.
- Accessories business is not ready; plan/proof/QC gates remain.
- SO-04 is in transit and cannot enter stock without batch number and COA.
- Ibiza 69-vial transfer is not sellable until receipt/recount.
- Retatrutide premium restock and next Pafi-only restock need corrected COA economics.
- Referral tree and affiliate/referral engine are not active/completed.

Red / blocked:
- Website compliance execution is blocked until lawyer boundaries arrive.
- Dragos cash/reconciliation remains blocked on Dragos-provided records.

## Immediate Next 48h Actions

1. Pafi: keep `P0-018` on hold until the restock planner is corrected for COA cost per SKU.
2. Pafi: progress `P0-006` and `P0-007` together, because pricing/margin and SKU disposition must share the same SKU truth.
3. Pafi: use `P0-008` as the single container for all accessories decisions.
4. Vic: wait for lawyer response before any website execution; prepare counsel/customs packet inputs.
5. Narcis: keep SO-04 receipt/admin gate strict: no batch number + COA means no stock acceptance.
6. Dragos: provide cash and transaction reconciliation records; no collaborator sales activation until controls are complete.

## Dashboard Result

`P0-0-001` can be marked done because this register now exists and links each live-state item to state, owner, next action, and evidence/task reference. It does not close the underlying open tasks listed above.
