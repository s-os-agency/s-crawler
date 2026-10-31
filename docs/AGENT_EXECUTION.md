# s-crawler — Agent execution instructions

**Portfolio:** 1/16 (source row 1); **Lead agent:** Grok; **specialty:** Browser exploration, crawl boundaries, runtime traces; **independent reviewer:** ChatGPT (Architecture and security review).
**Repository:** https://github.com/s-os-agency/s-crawler
**Authoritative gates:** https://docs.google.com/spreadsheets/d/1MMk4Tx0k5rS7e_vOIFg-Dg022VEqXsdwqHibT9-3uOI/edit#gid=20261034
**Release dashboard:** https://docs.google.com/spreadsheets/d/1MMk4Tx0k5rS7e_vOIFg-Dg022VEqXsdwqHibT9-3uOI/edit#gid=20261035
**Disposition:** ACTIVATE; **accountable proposed engineering role:** Browser & Crawling Engineer.

## Mandatory operating rules
- Existing root AGENTS.md owner instruction controls: do not add, restore or run software test suites, test-only workflows or scaffolding. Existing spreadsheet references to tests are superseded: obtain real source/build/configuration and operational readback evidence within the owner policy. Never claim tests were run or passed.
- Inspect canonical README, source, existing diffs and deployments before changes. Make the smallest reversible implementation change required. Do not merely write plans or invent launch statuses.
- The named lead is a proposed execution assignment, **not proof of an active external agent session**, OpenRouter invocation, or authority to use another agent's account. A reviewer is an independent second-pass assignment, not an approval already provided.
- Use only scoped provider access actually available. No blind deployment, destructive migrations, new permissions, purchases or exposure of credentials. Preserve backups and rollback.
- Attach evidence URL, UTC date, version/commit, deployed environment and observed result to the corresponding Exact Completion Gates row. Mark VERIFIED only for evidence-backed completion. Leave other gates OPEN; no fabricated real customer, revenue, PayPal or Ziina status.
- Production launch requires a provider-backed deployment receipt and actual live runtime observation, not a green document or UI screenshot.

## Exact execution order

### Gate 1.1 — SOURCE
**Action:** Pin dependencies and confirm runnable Python/Flask/Playwright entrypoint; install browser runtime in isolated test environment.
**Acceptance outcome:** Clean install plus import/start/health passes with command output and commit SHA.
**Evidence required:** actual source/commit, environment, timestamp, direct output/receipt, and reviewer; record in sheet. **Initial state: OPEN.**

### Gate 1.2 — SECURITY
**Action:** Validate URL input and explicit authorized scope; bound max depth/pages/time, prevent internal network/metadata access and redirects out of scope.
**Acceptance outcome:** Tests reject localhost/private/link-local/metadata targets and cross-scope redirects; bounded crawl demonstrably stops.
**Evidence required:** actual source/commit, environment, timestamp, direct output/receipt, and reviewer; record in sheet. **Initial state: OPEN.**

### Gate 1.3 — FUNCTION
**Action:** Execute authorized depth-1 crawl with duplicate URL, broken link, and network timeout fixtures.
**Acceptance outcome:** Result has correct levels, source URLs, normalized links, errors and trace; test run exit code zero.
**Evidence required:** actual source/commit, environment, timestamp, direct output/receipt, and reviewer; record in sheet. **Initial state: OPEN.**

### Gate 1.4 — DEPLOY
**Action:** Deploy approved build to the intended public host; confirm UI and API refer to same release/adapter.
**Acceptance outcome:** Deployment ID + version/commit + HTTPS /health + authenticated job result recorded.
**Evidence required:** actual source/commit, environment, timestamp, direct output/receipt, and reviewer; record in sheet. **Initial state: OPEN.**

### Gate 1.5 — OPS
**Action:** Set logs, bounded queue/retry, secrets policy, rate limits and rollback plan; re-run after restart.
**Acceptance outcome:** Error/timeout flow creates receipt; status and output persist or explicitly document stateless behavior; rollback tested.
**Evidence required:** actual source/commit, environment, timestamp, direct output/receipt, and reviewer; record in sheet. **Initial state: OPEN.**

### Gate 1.6 — LIVE PROOF
**Action:** Run one permitted production crawl end to end and independently re-fetch the result.
**Acceptance outcome:** Timestamped live URL, commit, test input/output and success receipt attached; not just screenshot or README claim.
**Evidence required:** actual source/commit, environment, timestamp, direct output/receipt, and reviewer; record in sheet. **Initial state: OPEN.**

### Gate 1.7 — COMMERCIAL
**Action:** Only if selling crawler: identify buyer and verify real accepted delivery; integrate checkout only through approved merchant rail.
**Acceptance outcome:** Buyer/order/contract and accepted deliverable verified; paid status only after provider settlement and currency match. Otherwise do not claim customers or payments.
**Evidence required:** actual source/commit, environment, timestamp, direct output/receipt, and reviewer; record in sheet. **Initial state: OPEN.**

## Completion handoff
Update each gate's verification state in Google Sheets and attach proof. Distinguish implementation from launch, customer acceptance from inquiries and settled payments from checkout creation. The lead produces the change receipt; the reviewer checks evidence independently. Do not announce completion until all required applicable gates pass. Report any unavoidable external authorization boundary specifically.

**Agent document author:** GPT-6 (instructions only; not a launch attestation).
