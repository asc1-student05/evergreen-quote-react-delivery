# Evergreen Quote: Vision Brief

> Copy this file into `delivery-leadership-package/vision-brief.md` in your repo and fill it in. Target length: 1 page (~300 words). Write for a Liberty Mutual VP who has 90 seconds.

## Product
**Name:** Evergreen Insurance Quote (Phase 2 React rebuild)
**Delivery week:** 2
**Delivery Lead:** Jyoti Kumari
**Engineering team (represented by):** https://github.com/asc1-student05/evergreen-quote-react-delivery/tree/main/delivery-leadership-package
**GitHub Project board:** _link_

## Who is the customer?
The customer is a first-time insurance shopper, often a new renter, first-time homeowner, or young adult purchasing insurance for the first time. They have been told they need coverage and want a quick estimate before investing time in a lengthy application process. They are typically browsing on a mobile device and comparing multiple providers. Today, their alternative is navigating insurance websites that require extensive personal information, account creation, or email capture before showing any pricing, causing many users to abandon the process and look elsewhere.

## What pain does Evergreen Quote remove?
Evergreen Quote removes the frustration of waiting to see a price. Customers want a fast, commitment-free estimate to understand what insurance might cost before deciding whether to engage further. Phase 1 required users to complete fields and click a calculate button to see a quote. Phase 2 improves the experience by providing a live premium estimate that updates instantly as users enter information. The result is a simpler, more responsive experience that reduces friction, provides immediate feedback, and helps shoppers get the information they need before they leave for a competitor.

## What does "good" look like at end of the week?
- Customers see their estimated monthly premium update instantly as they modify coverage type, age, or coverage amount.
- Recent quotes load successfully from the JSON data feed and clearly display loading, error, and success states.
- Saving a quote immediately places it at the top of the Recent Quotes list.
- `npm run type-check` and `npm run build` complete successfully with no errors.
- The solution is merged into `main` through a reviewed pull request with a green CI pipeline run.

- 
- 
- 

## What are we explicitly NOT doing this week?
- Building a real insurance pricing or actuarial rating engine.
- Creating customer accounts, authentication, or quote persistence.
- Adding email capture, marketing workflows, or customer outreach features.
- Implementing payment processing, policy purchase, or checkout functionality.
- Building a backend service, deployment pipeline, routing, or automated test suite.

- 
- 
- 

## How will we know if it worked?
- 100% of supported coverage types (Auto, Home, Life) produce valid premium estimates that update in real time.
- CI passes successfully with both TypeScript compilation and production build completion.
- A saved quote appears at the top of the Recent Quotes list immediately after selection, with no page refresh required.

- 
- 
