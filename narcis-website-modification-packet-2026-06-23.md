# Narcis Website Modification Packet — PetraLab RUO

Generated: 2026-06-23  
Owner: Narcis  
Review: Pafi  
Source hierarchy:

1. `/Users/pafi/.nexus/projects/petralab-ruo/implementation-todo-2026-06-22.md`
2. `/Users/pafi/Documents/RUO Peptides/output/live-site-audit-2026-06-22/peptralabs-live-audit-refined-modification-proposals-2026-06-22.md`
3. Pafi owner overrides: D2C remains live, ads are not running, high-revenue SKUs continue selling while copy/checkout risk is cleaned, B2B is inbound/supporting only.

## Execution Rule

Do not stop high-revenue D2C sales by default. The work is to remove public copy/tooling/checkout contradictions with RUO positioning and preserve revenue where the buyer flow can stay aligned with research-use intent.

## P0 — Do First

### 1. Affiliate Pages: Pause Or Rewrite

URLs:

- `https://www.peptralabs.com/affiliate`
- `https://www.peptralabs.ro/affiliate`

Modify:

- Remove recurring `20-35%` commission framing.
- Remove `5% override`.
- Remove sub-affiliate / team / downline recruitment.
- Remove influencer / creator recruitment framing.
- Remove passive-income framing.
- Remove weekly crypto payout promises.
- Remove public earnings calculator.
- Replace with `Referral programme paused pending compliance review` or private single-tier approved-partner wording.

Acceptance:

- Search finds no `override`, `sub-affiliate`, `recruit`, `passive income`, `20-35%`, `weekly USDC`, or `weekly USDT`.
- `.ro` version is not looser than `.com`.

### 2. Peptide Calculator And Reconstitution Flow: Remove Or Gate

URLs:

- `https://www.peptralabs.com/peptide-calculator`
- `.ro` equivalent
- `/glossary/reconstitution`
- `.ro` equivalent if present

Modify:

- Remove from navigation and public index.
- Either return `404`, `noindex`, login gate, or counsel-approved lab-only utility.
- If any calculator remains public, it must be generic unit conversion only.
- Remove U-100 syringe units, draw volume, target amount per draw, presets, reverse syringe mark calculation, and reconstitution instructions.

Acceptance:

- Public crawl cannot access syringe/draw/reconstitution workflow.
- No buyer-flow page links users toward dosing, injection, or reconstitution guidance.

### 3. High-Revenue / High-Risk SKU Copy Cleanup While Continuing Sales

SKUs/pages to handle first:

- Retatrutide
- GLP-1 adjacent pages
- BPC-157
- TB-500
- Tesamorelin
- Tirzepatide
- Semaglutida
- Melanotan 2
- Use-guidance/research-guide pages tied to the above

Known URL clusters:

- Retatrutide: `/products/retatrutide`, `/peptides/retatrutide`, `/research/retatrutide-research-guide`, `/retatrutide-europe`, `.ro/products/retatrutide`, `.ro/retatrutide-romania-pret`, `.ro/research/retatrutide-research-guide`
- BPC/TB: `/products/bpc-157`, `/peptides/bpc-157`, `/research/bpc-157-mechanisms`, `/products/tb-500`, `/peptides/tb-500`, `/research/tb-500-tissue-repair`, `/research/bpc-157-vs-tb-500`, plus `.ro` equivalents
- GLP-1 adjacent: `/products/tirzepatide`, `/buy-research-peptides-europe/tirzepatide`, `.ro/products/tirzepatide`, `.ro/semaglutida-cercetare-romania`

Modify:

- Remove body-effect and medical-use wording from product-near copy, meta, FAQ, schema, and cards.
- Remove or rewrite terms like weight loss, liver fat, diabetes, HbA1c, obesity, appetite, energy expenditure, healing, wound, repair, recovery, tendon, injury, treatment, clinical protocol.
- Keep neutral identity/specification/RUO wording.
- Keep sales live unless Pafi/counsel explicitly gates a SKU.

Acceptance:

- Pages contain no consumer benefit/dosing/use claims near commerce flow.
- Ordering language remains aligned with research-use intent.
- `.ro` is at least as strict as `.com`.

### 4. Checkout Intended-Use Acknowledgement

Modify checkout before or during payment:

- Buyer type.
- Research purpose.
- Acknowledgement: no personal use, no clinical use, no injection, no treatment, no resale-with-claims.
- Source tag.
- Manual review/rejection flags for invalid intent.

Acceptance:

- Order record stores acknowledgement fields.
- Checkout flags or rejects personal-use, dosing/injection, treatment, and resale-with-claims intent.
- Evidence is visible in dashboard/Supabase order data.

### 5. High-Risk CTAs And Promo Strips

Modify:

- Replace `ORDER NOW`, `COMANDĂ ACUM`, `Buy`, launch discount, free-shipping promo near high-risk SKU or research pages.
- Use restrained research-supply wording such as `Request supply`, `Request batch info`, or approved equivalent.

Acceptance:

- High-risk SKU pages and research pages do not show aggressive consumer-commerce CTAs.
- Product cards do not push high-risk SKUs with discount/free-shipping language.

## P1 — Do Next

### 6. AI/Search/Schema Parity

Surfaces:

- Visible page copy
- Meta titles/descriptions
- FAQ schema
- Product JSON-LD
- `llms.txt`
- `llms-full.txt`

Modify:

- Rebuild from the same approved content model after page copy cleanup.
- Block stronger claims in schema/AI files than visible copy.
- Remove clinical/body-effect/commerce claim fields from high-risk product schema.

Acceptance:

- Banned-claim scan passes on visible HTML and generated AI/SEO/schema files together.

### 7. COA Absence-State Consistency

Modify:

- Preserve existing `No COA report currently listed` improvements.
- Make COA state structured by SKU/batch.
- Mirror state in `.com`, `.ro`, product schema, support macros, lab-report archive, and LLM files.

Allowed states:

- Verified report
- Supplier COA
- Independent COA
- No public COA
- Failed
- Not applicable

Acceptance:

- Every SKU/batch has exactly one explicit COA state.
- `.ro` and `.com` do not disagree.

### 8. Romanian Parity

Modify:

- Translate compliance policy, affiliate pause, buyer-intent acknowledgement, and high-risk SKU rewrites into Romanian.
- Do not leave `.ro/affiliate` in English.
- Remove Romanian clinical/metabolic wording from high-risk pages.

Acceptance:

- Same scan rules pass on `.ro` as on `.com`.
- `.ro` is not a softer sales/compliance channel.

### 9. Accessories / BAC Water Separation

Modify:

- Keep accessories separate from peptide administration/injection workflow.
- Avoid syringe/reconstitution adjacency.
- Copy should be storage/logistics only unless proof and policy gate allow more.

Acceptance:

- Accessories pages do not link to calculator, dosing, injection, or peptide-use instructions.

## Final Verification For Narcis

After changes:

1. Send Pafi exact URLs changed.
2. Send before/after screenshots for affiliate, calculator, one GLP-1 page, one BPC/TB page, checkout acknowledgement, and `.ro` affiliate/high-risk examples.
3. Export or screenshot the banned-claim scan terms.
4. Confirm dashboard/Supabase has checkout acknowledgement fields if checkout work is deployed.
5. Mark any not-done item as `blocked` with reason, not silently skipped.
