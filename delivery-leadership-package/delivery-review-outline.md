# Delivery Review: Evergreen Quote

## Slide 1: Delivery goal & did we hit it?

- Goal : Deliver a demonstrable "Evergreen Quote React app" Insurance quote experience for Auto, Home, and life insurance with typed data, resilient quote loading, and green CI, merged to main through a reviewed pull request. 
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
(https://github.com/asc1-student05/evergreen-quote-react-delivery/blob/main/delivery-leadership-package/risk-register.md)

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


