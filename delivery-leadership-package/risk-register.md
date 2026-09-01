# Risk Register


| # | Risk | Owner | Likelihood (L/M/H) | Impact (L/M/H) | Mitigation | Trigger to escalate |
|---|---|---|---|---|---|---|
| R1 | TypeScript errors prevent successful build or deployment. | Jyoti | M | H | Run `npm run type-check` after every major change and before committing code. | Type-check still fails after 30 minutes of troubleshooting. |
| R2 | React components are not assembled correctly, causing application features to break. | Jyoti | M | H | Test functionality after wiring each component into App.tsx. | Quote form or recent quotes section is not working by end of Day 2. |
| R3 | Incorrect premium rates are configured, resulting in inaccurate quote estimates. | Jyoti | M | M | Verify sponsor-approved rates before updating `BASE_RATES`. | Rate values cannot be confirmed before Day 3. |
| R4 | GitHub Actions CI pipeline fails and blocks merge activities. | Jyoti | M | H | Review CI results after every push and fix failures immediately. | CI remains red for more than one work session. |
| R5 | Unexpected injects or scope changes reduce available time for priority work. | Jyoti | H | M | Re-prioritize backlog and focus on required deliverables first. | Inject requires significant work that threatens completion of core tasks. |
| R6 | Delivery leadership documents are incomplete before presentation day. | Jyoti | M | M | Complete artifacts daily instead of waiting until Day 5. | Any required artifact is missing at end of Day 4. |
| R7 | Late scope change (ZIP-code field request) impacts the team's ability to complete committed delivery goals on schedule. | Jyoti | H | H | Keep focus on the agreed delivery scope and defer non-critical features to a future release. Re-prioritize backlog items as needed. | Additional feature work causes Day 3 or Day 4 deliverables to fall behind schedule. |
| R8 | Moderate-severity dependency audit finding raises stakeholder concerns or creates uncertainty about release readiness. | Jyoti | M | M | Track the platform team's planned upgrade and monitor for changes in severity. | New information indicates customer-facing impact or the sponsor requests a release hold. |

## How I'll use this register

I will review this risk register at the start and end of each day to identify issues early and update mitigation plans. The register will be stored in the delivery leadership package and shared with the instructor and teammates for visibility. Any risk that reaches its escalation trigger will be discussed during the next status update or check-in.
