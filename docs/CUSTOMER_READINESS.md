# Customer-readiness and publication gate

Recorded: 2026-10-31 (Asia/Dubai)
Status: **NOT VERIFIED READY TO PUBLISH**. This is a gap-and-acceptance record, not proof of deployment, a sale, or a passed test.

## Exact product outcome
Deliver an authorized, source-attributed crawl of a customer-provided domain.

## Surgical acceptance checks (not yet passed)
1. [ ] Run the documented Python engine and GET /health successfully.
2. [ ] POST /crawl against an authorized test host with depth 1; retain input, output, timestamp and trace.
3. [ ] Confirm normalized URL inventory, deduplication, depth and same-domain limits.
4. [ ] Compare hosted UI result with canonical engine output; document any separate adapter or deployment.

## Verified limitations / missing evidence
- Hosted interface is described but not independently revalidated in this change.
- No verified paying customer, contract, measured savings, invoice or receipt.
- No live PayPal or Ziina checkout linked to this repository.

## Immediate next executable action
Reproduce one bounded crawl and attach input/output evidence before promoting the publish gate.

## Customer evidence rule
Only identify a customer if a customer-specific contract, purchase/order, invoice and settled-payment receipt, or documented accepted delivery identifies the project. A source repository, GitHub issue, demo, live URL or CRM lead by itself does **not** prove a paying customer. Customer name, source reference, date, product mapping, amount and currency must be verified before adding revenue claims. No customer or payment transaction is asserted by this record.

## Payments: PayPal and Ziina
- Provider integration: **NOT CONNECTED / NOT VERIFIED** for this repository.
- Never commit API credentials, account details or webhook secrets.
- Before enabling a live checkout, confirm account ownership, platform approval, appropriate product/service, merchant terms, currency/tax handling, redirect URLs, authenticated callback/webhook verification, idempotency, refund and failure flow, and a provider-recorded transaction linked to this product.
- Do not substitute a manually supplied payment link for a verified merchant integration or claim a settlement from a checkout screen.

## Publication rule
No “live,” “customer-ready,” “selling,” or “payments enabled” label unless the corresponding independent evidence is attached with a timestamp, environment, test result, and accountable reviewer. Reversible preparation is allowed; production changes remain subject to actual external authorization/security boundaries.

Executing agent for this documentation change: GPT-6.
