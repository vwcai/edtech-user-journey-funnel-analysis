# Measurement Plan

This document outlines an anonymized tracking plan for measuring the user journey described in the case study.

This is a proposed business tracking plan, not an implemented analytics setup.

## Measurement Goal

The goal is to make the browsing-to-enrollment funnel measurable so a product or analytics team can identify where users drop off and which interventions reduce friction.

## Recommended Funnel Events

| Event | Purpose | Suggested Parameters |
| --- | --- | --- |
| `view_program_list` | User views a list of available programs or courses | `grade_level`, `program_type`, `entry_source` |
| `select_program` | User selects a program from a list or card | `grade_level`, `program_type`, `position`, `price_visible` |
| `view_program_detail` | User views a course detail page | `grade_level`, `program_type`, `price_visible`, `placement_required` |
| `pricing_view` | User views pricing or a price range | `program_type`, `price_type`, `price_visible_before_signin` |
| `evaluation_cta_click` | User clicks an evaluation or placement CTA | `page_type`, `program_type`, `cta_text`, `cta_position` |
| `trial_cta_click` | User clicks a trial or low-risk entry CTA | `page_type`, `program_type`, `cta_position` |
| `sign_up_start` | User begins registration | `entry_point`, `program_type`, `is_required_to_continue` |
| `form_start` | User begins a form | `form_id`, `form_name`, `page_type` |
| `form_submit` | User submits a form | `form_id`, `form_name`, `submission_status` |
| `begin_checkout` | User reaches checkout or enrollment confirmation | `program_type`, `price`, `placement_status` |
| `purchase` | User completes purchase or enrollment | `program_type`, `price`, `trial_flag` |
| `policy_view` | User views refund, drop, or cancellation policy | `policy_type`, `page_type`, `program_type` |

## Key Funnel Questions

- How many users view course details before registering?
- Which course pages drive the highest evaluation or trial clicks?
- How often do users encounter pricing before sign-in?
- Do users who view refund or drop policies convert at a different rate?
- Where do users abandon between course browsing, evaluation, trial, and purchase?
- Does surfacing the trial option earlier reduce evaluation-stage drop-off?

## Core Metrics

- Course detail view rate
- Sign-up start rate
- Evaluation CTA click rate
- Trial CTA click rate
- Pricing visibility rate
- Form start to form submit rate
- Checkout start rate
- Purchase or enrollment conversion rate
- Drop-off by funnel stage

## Recommended Segments

- New vs returning users
- Organic vs paid vs referral entry source
- Grade level
- Program type
- Users exposed to trial CTA vs not exposed
- Users exposed to policy information vs not exposed
- Users who completed evaluation vs users who abandoned before evaluation

## Setup Notes

- Define one primary reporting destination before expanding event coverage
- Use consistent event and parameter naming across pages
- Avoid relying only on page views and scroll events for funnel analysis
- Test events before using them for reporting
- Document the business meaning of each tracked event so reporting remains interpretable
