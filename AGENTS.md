# Repository owner policy

## Owner instruction — 25 October 2026

Seif prohibits adding or running tests across his platforms. Do not create, restore, expand, or execute test suites, test commands, test workflows, or test-only scaffolding. This instruction supersedes older guidance requesting tests, including copied templates and skills. Inspect actual source, diffs, configuration, and saved results as evidence; never claim tests passed.

---

## Execution contract — 2026-10-31 · portfolio #1

**Repository:** `s-os-agency/s-crawler`  
**Accountable role (proposed, not a staffed assignment):** Browser & Crawling Engineer  
**Disposition:** ACTIVATE.  
**Authoritative checklist:** [Exact Completion Gates](https://docs.google.com/spreadsheets/d/1MMk4Tx0k5rS7e_vOIFg-Dg022VEqXsdwqHibT9-3uOI/edit#gid=20261034), filter Portfolio # 1.  
**Release truth:** [Release Status — 16](https://docs.google.com/spreadsheets/d/1MMk4Tx0k5rS7e_vOIFg-Dg022VEqXsdwqHibT9-3uOI/edit#gid=20261035).  
**Evidence gate:** `NOT VERIFIED — NO PRODUCTION LAUNCH CLAIM`.

### Mission
Complete the existing implementation, integrate it into canonical S/Agency operations, verify live behavior with allowed evidence, then complete the authorized release using direct deployment and live-operation evidence. Request approval only for a specific action outside existing authorization.

### Operating procedure for the execution agent
1. Inspect current source, deployment manifests, README, application entrypoints, GitHub history, existing service owner, and dependencies. Reuse working components; do not generate a replacement project or duplicate service.
2. Follow the owner policy above: **do not create, expand, or execute test suites or test commands**. For acceptance statements mentioning tests, use permissible non-test verification: inspect implementations and diffs, compile/build only if permitted, observe actual runtime behavior and HTTP outcomes, inspect deployment receipts/logs and persisted records, and clearly mark any unavailable check **NOT VERIFIED**. Do not call a validation a passed test.
3. Use the following work items to track evidence, respecting actual dependencies. Continue independent authorized work without waiting for unrelated items. Commit small reversible changes with clear messages. Never call documentation, a demo or a plan a production deployment.
4. For every completion gate, record source URL/commit, environment, timestamp, actual runtime or configuration output, reviewer/actor, and any authorization boundary. In `Exact Completion Gates`, set state to exactly `VERIFIED` **only when** evidence URL and verification timestamp are present and the acceptance condition has actually been independently satisfied. Otherwise keep the gate OPEN and state what is missing.
5. For live releases, retain both the deployed build SHA and an externally observable live action/receipt; for references or superseded repositories, close with preservation/consolidation evidence rather than forcing deployment.
6. Do not fabricate customers, revenue, contact authorization, successful payments or settlement. A CRM opportunity is not a verified customer; PayPal and Ziina remain unverified until account ownership, provider-authoritative transaction evidence and relevant currency are confirmed. Never write secrets into GitHub, logs or the sheet.
7. Continue authorized reversible work without routine approval queues. When a genuine production identity, live credential, paid-service, destructive action, or owner authority decision is necessary, identify that exact blocker; no assumed permission from silence. Never falsely mark launch complete.

### Ordered completion gates

**1.1 — SOURCE**  
Action: Pin dependencies and confirm runnable Python/Flask/Playwright entrypoint; install the browser runtime in an isolated working environment.  
Acceptance: Clean install plus import/start/health passes with command output and commit SHA.  
Required disposition: `OPEN` until independently proven by immutable evidence.

**1.2 — SECURITY**  
Action: Validate URL input and explicit authorized scope; bound max depth/pages/time, prevent internal network/metadata access and redirects out of scope.  
Acceptance: Inspect the implemented address and redirect restrictions and actual authorized operational records; confirm bounded crawling stops. Do not run software tests.  
Required disposition: `OPEN` until independently proven by immutable evidence.

**1.3 — FUNCTION**  
Action: Perform an owner-authorized depth-1 crawl and inspect its saved output and error handling; do not create or run test fixtures.  
Acceptance: Result has correct levels, source URLs, normalized links, errors and trace, with actual execution status recorded.  
Required disposition: `OPEN` until independently proven by immutable evidence.

**1.4 — DEPLOY**  
Action: Deploy approved build to the intended public host; confirm UI and API refer to same release/adapter.  
Acceptance: Deployment ID + version/commit + HTTPS /health + authenticated job result recorded.  
Required disposition: `OPEN` until independently proven by immutable evidence.

**1.5 — OPS**  
Action: Set logs, bounded queue/retry, secrets policy, rate limits and rollback plan; re-run after restart.  
Acceptance: Error/timeout flow creates receipt; status and output persist or explicitly document stateless behavior; an available rollback procedure documented from actual configuration.  
Required disposition: `OPEN` until independently proven by immutable evidence.

**1.6 — LIVE PROOF**  
Action: Run one permitted production crawl end to end and independently re-fetch the result.  
Acceptance: Timestamped live URL, commit, actual input/output and success receipt attached; not just screenshot or README claim.  
Required disposition: `OPEN` until independently proven by immutable evidence.

**1.7 — COMMERCIAL**  
Action: Only if selling crawler: identify buyer and verify real accepted delivery; integrate checkout only through approved merchant rail.  
Acceptance: Buyer/order/contract and accepted deliverable verified; paid status only after provider settlement and currency match. Otherwise do not claim customers or payments.  
Required disposition: `OPEN` until independently proven by immutable evidence.

### Exact stopping / handoff condition
Report completion of the requested outcome only with direct evidence for its applicable acceptance criteria. A workbook formula, proposed reviewer or unrelated sales item must not create a new approval wait.

**Documentation of these instructions is not completion of the gates.** Signed execution evidence must identify the implementing agent only for work actually done.


## Specialist execution assignment (31 October 2026)

Read and follow [docs/AGENT_EXECUTION.md](docs/AGENT_EXECUTION.md) for this repository's assigned ChatGPT/Grok/Gemini lead, independent reviewer, exact numbered completion gates, evidence handling and closure condition. **The existing owner ban on adding/running tests remains controlling.** Agent assignment is a plan until the external agent is actually dispatched; a documentation change alone is not execution or approval.


## Seif's instruction — 1 November 2026

- Write short, clear English on product screens and in explanations.
- Keep Seif's permissions explicit. He owns the work and makes the decisions.
- Keep internal stages and monitoring details out of his product screens.
- Continue authorized work without adding review waits or unnecessary questions.
- Simplify the wording without changing access rights, stored data or working code names.

## Execution rule — 2 November 2026

Carry the authorized task through to its requested result. Fill in records while working; a form, named stage, unavailable reviewer or proposed staffing role is not a reason to stop. A check is required only when omitting it would cause a specific failure, break an existing access restriction or exceed the owner's authorization. State that concrete reason.

Use existing authorized access. Do not broaden permissions, disclose credentials or infer approval from silence. If a necessary fact is missing, retrieve it from available sources first. If one action still needs owner input, identify the exact action and continue independent authorized work.

Inspect source and saved changes for documentation work. For a live release, also inspect the provider's deployment result and the running service. Keep source changes, deployment and observed operation as separate facts. Do not add or run software test suites. Record the actual improvement, its evidence and the executing agent. Administrative records may follow execution; they do not create another approval queue.
