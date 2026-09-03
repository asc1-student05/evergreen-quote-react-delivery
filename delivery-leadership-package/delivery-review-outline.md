# Delivery Review: Evergreen Quote

## Slide 1: Delivery goal & did we hit it?

- Goal : Deliver a demonstrable "Evergreen Quote React app" Insurance quote experience for Auto, Home, and life insurance with typed data, resilient quote loading, shared state, and green CI, merged to main through a reviewed pull request. 
- Hit? ☑ Yes  ☐ Partially  ☐ No
- Why: The application was successfully assembled, data loading was implemented, context and hooks were integrated, CI was enabled, and all required leadership deliverables were completed.

## Slide 2: What shipped

- Evergreen Quote React application running successfully.
- QuoteForm, PremiumDisplay, and RecentQuotes components integrated.
- TypeScript validation completed and issues resolved.
- Data loading implemented using quotes.json.
- Hook and Context architecture integrated.
- Save This Quote functionality working.
- GitHub Actions CI workflow enabled.
- Risk Register, Decision Memo, Status Updates, and Go/No-Go assessment completed.
- Link to merged PR: [(https://github.com/asc1-student05/evergreen-quote-react-delivery/pull/12)]
- Link to green CI run: [[Add after final CI run](https://github.com/asc1-student05/evergreen-quote-react-delivery/actions/runs/33672309764)]

## Slide 3: Two key decisions

#### Decision 1: Defer ZIP-Code Field Request

Why it mattered:
- Protected the committed delivery scope.
- Reduced risk to timeline and testing efforts.
- Allowed focus on delivering the agreed business outcome.

#### Decision 2: Continue With the Planned Release

Why it mattered:
- The dependency audit identified a moderate security issue in a development tool, not customer-facing software.
- The platform team already had a fix planned for the following week.
- Holding the release would have delayed delivery without a confirmed customer impact.
- Allowed the team to stay on schedule while continuing to track the risk.

## Slide 4: Risks & injects

- Top risk we tracked: 
| R1 | TypeScript errors prevent successful build or deployment. | Jyoti | M | H | Run `npm run type-check` after every major change and before committing code. | Type-check still fails after 30 minutes of troubleshooting. |
| R2 | React components are not assembled correctly, causing application features to break. | Jyoti | M | H | Test functionality after wiring each component into App.tsx. | Quote form or recent quotes section is not working by end of Day 2. |
| R3 | Incorrect premium rates are configured, resulting in inaccurate quote estimates. | Jyoti | M | M | Verify sponsor-approved rates before updating `BASE_RATES`. | Rate values cannot be confirmed before Day 3. |
| R4 | GitHub Actions CI pipeline fails and blocks merge activities. | Jyoti | M | H | Review CI results after every push and fix failures immediately. | CI remains red for more than one work session. |
| R5 | Unexpected injects or scope changes reduce available time for priority work. | Jyoti | H | M | Re-prioritize backlog and focus on required deliverables first. | Inject requires significant work that threatens completion of core tasks. |
| R6 | Delivery leadership documents are incomplete before presentation day. | Jyoti | M | M | Complete artifacts daily instead of waiting until Day 5. | Any required artifact is missing at end of Day 4. |
| R7 | Late scope change (ZIP-code field request) impacts the team's ability to complete committed delivery goals on schedule. | Jyoti | H | H | Keep focus on the agreed delivery scope and defer non-critical features to a future release. Re-prioritize backlog items as needed. | Additional feature work causes Day 3 or Day 4 deliverables to fall behind schedule. |

#### Inject #1 (Tuesday)

- Marketing requested a ZIP-code field.
- Platform team reported a dependency audit finding. The dependency audit identified a moderate security issue in a development tool, not customer-facing software.
- Decision: Defer ZIP-code enhancement and continue planned delivery.

#### Inject #2 (Wednesday)

- Customer reported an unusually high quote amount.
- CI on main became red after a hotfix.
- Reviewed failure and escalated investigation.
- Made a GO WITH CONDITIONS recommendation.
GO WITH CONDITIONS.

My delivery/lead branch is currently passing type-check and build validation, but main is red following a recent hotfix. The primary factor driving this decision is the unresolved CI failure on main, which indicates that the integration environment is not currently stable. I will proceed only after the owner of the hotfix confirms the root cause and main returns to a green state. If investigation shows the issue is unrelated to my branch and main is restored to green, I would move forward with the merge.

#### Inject #3 (Wednesday)

- Customer pricing concern remained under investigation.
- Main branch still required resolution before merge readiness.
- Coordinated ownership, communication, and risk management.

## Slide 5: What I'd do differently next round

- Review CI health immediately after every merge.
- Track dependency audit findings earlier.
- Increase stakeholder communication around scope changes.
- Expand testing scenarios before release readiness reviews.
- 
### Slide 6: Executive Summary

#### Delivery Outcome

Successfully delivered the Evergreen Quote React application.

#### Key Accomplishments

- Assembled and integrated all required React components.
- Fixed TypeScript issues and maintained type safety.
- Implemented data loading using quotes.json.
- Integrated Hooks and Context architecture.
- Enabled GitHub Actions CI workflow.
- Completed all required delivery leadership artifacts.

#### Key Decisions

- Deferred the ZIP-code enhancement to protect committed scope.
- Proceeded with the planned release while monitoring the dependency audit finding.
- Used a GO WITH CONDITIONS approach when main branch CI became unstable.

#### Lessons Learned

- Protecting scope is critical to meeting delivery commitments.
- CI health should be monitored continuously.
- Early stakeholder communication reduces delivery risk.
- Strong delivery leadership requires prioritization, coordination, and decision-making.

#### Final Result

The project achieved its primary objective: delivering a typed, data-loading Evergreen Quote application with documented decisions, managed risks, CI validation, and a clear release recommendation.


