# EdTech User Journey and Conversion Funnel Analysis

This repository is an anonymized Business Analyst portfolio case study on user journey friction, conversion drop-offs, competitor benchmarking, and tracking gaps in an online education funnel.

## Public Portfolio Note

This project is based on publicly accessible website walkthroughs and browser-side testing. Company names, URLs, screenshots, tracking identifiers, and other identifying details have been generalized. The analysis does not use internal company data.

## Project Overview

This project evaluates the browsing-to-purchase journey for an online education platform by comparing a `Target Platform` against a `Benchmark Platform` from the perspective of a parent evaluating math programs for a child.

## Business Problem

Parents need clear course information, pricing, placement requirements, trial options, and refund policies before committing to an education program. When key decision information is hidden, scattered, or introduced too late, users may drop off before registration, evaluation, or purchase.

## Data

- Public website walkthroughs from a simulated parent perspective
- Competitor user journey comparison between a target platform and a benchmark platform
- Funnel-stage friction assessment across browsing, sign-up, evaluation, trial, and purchase
- Browser-side GA4 request inspection using Chrome DevTools
- Observed front-end events and tracking gaps

## Approach

- Mapped the end-to-end user journey from search entry to course purchase
- Compared friction across major funnel stages for both platforms
- Identified three high-impact drop-off points in the target platform journey
- Prioritized recommendations by expected impact, implementation effort, and speed to effect
- Reviewed browser-side tracking coverage to assess whether the funnel could be measured reliably

## Key Insights

- Key decision information, especially pricing and course overview details, was less visible on core program pages
- Evaluation prompts appeared early and frequently, creating pressure before users had enough information to decide
- A low-cost trial option existed but was difficult to discover at the moment users needed risk reduction
- Refund and drop policies were not surfaced clearly at key purchase-decision points
- Tracking coverage appeared insufficient for full mid-funnel diagnosis, especially around course selection, checkout intent, and form-level behavior

## Recommendations

- Make the low-cost trial entry point visible on course pages, evaluation prompts, and navigation
- Surface refund and drop policies directly on course pages and purchase-adjacent screens
- Show pricing or price ranges before sign-in to reduce unnecessary registration friction
- Reduce repeated evaluation prompts during browsing and shift placement messaging closer to high-intent moments
- Add journey-specific GA4 events for course views, selections, enrollment intent, trial clicks, checkout steps, and form behavior

## Success Metrics

If these recommendations were implemented, I would track whether the changes improve both conversion behavior and measurement quality:

- Course detail to sign-up rate
- Course detail to trial CTA click rate
- Evaluation CTA click-through rate
- Evaluation start to completion rate
- Sign-up start to form submit rate
- Checkout start rate
- Purchase or enrollment conversion rate
- Refund/drop policy view rate near purchase intent
- Event coverage completeness across the funnel

## Implementation Priority

| Priority | Recommendation | Why It Comes First |
| --- | --- | --- |
| P0 | Increase low-cost trial and refund/drop policy visibility | High expected impact with low implementation effort because the assets already exist |
| P1 | Improve pricing and course overview visibility | Reduces early browsing friction and helps users compare options before sign-in |
| P2 | Reduce evaluation prompt pressure and revise placement messaging | High impact, but likely requires more product, UX, and stakeholder alignment |

## Start Here

- `PROJECT_SUMMARY.md`: detailed anonymized case study
- `docs/measurement_plan.md`: recommended event tracking plan for funnel measurement
- `docs/dashboard_plan.md`: dashboard plan for monitoring funnel performance

## Repository Contents

- `README.md`: portfolio landing page
- `PROJECT_SUMMARY.md`: full case-study narrative with funnel findings and recommendations
- `docs/measurement_plan.md`: proposed GA4-style tracking plan
- `docs/dashboard_plan.md`: proposed dashboard structure and KPI views

## Skills Demonstrated

- user journey analysis
- conversion funnel analysis
- web analytics and GA4 tracking review
- competitor benchmarking
- UX friction diagnosis
- recommendation prioritization
- data communication
- dashboard and KPI planning
