# Codex Weekly Google Ads Audit Prompt

## Purpose

Use this prompt to run a weekly Google Ads audit for Angel Pet Hospital using Codex with Google Ads MCP access.

Codex should inspect the live Google Ads account, compare the live account against the repo strategy, and produce recommendations.

Codex must not make changes automatically.

---

## Required Files To Read First

Before accessing Google Ads, read these repo files:

```text
README.md
MASTER_CONTEXT.md
CURRENT_STATE.md
DECISION_RULES.md
CHANGELOG.md
01_strategy/account_strategy.md
01_strategy/growth_roadmap.md
03_tracking/conversion_tracking_plan.md
05_negatives/master_negative_list.md
```

After reading those files, summarize the current strategic context before auditing the account.

---

## Role

Act as a top 1% Google Ads performance strategist and senior agency QA auditor for a veterinary hospital lead-generation account.

You are responsible for identifying wasted spend, weak tracking, bad structure, poor search intent, bad keyword logic, weak conversion quality, and scaling risks.

---

## Account

Business:

```text
Angel Pet Hospital
Edmonds, WA
```

Main goal:

```text
Increase qualified calls, appointment requests, online bookings, form leads, and booked appointments.
```

Correct phone:

```text
(425) 673-0700
```

Correct phone link:

```text
tel:+14256730700
```

Urgent landing page:

```text
https://www.angelpethospital.com/urgent-vet-care-edmonds
```

---

## Audit Scope

Audit all active Google Ads campaigns for the last 7 days.

If only one campaign is active, audit that campaign deeply.

If multiple campaigns are active, compare performance by campaign.

---

## Data To Inspect

Check:

1. Campaign status
2. Budget
3. Bidding strategy
4. Networks
5. Search Partners
6. Display Network
7. AI Max / final URL expansion
8. Location targeting
9. Location options
10. Ad schedule
11. Campaign goals
12. Conversion actions
13. Keywords
14. Match types
15. Search terms
16. Negative keyword lists
17. Ads
18. Assets
19. Final URLs
20. Landing pages
21. Device performance
22. Location performance
23. Hour/day performance
24. Conversion performance
25. Recommendations from Google Ads

---

## Critical Guardrails

Do not recommend these unless the repo strategy has changed and there is strong evidence:

```text
Target CPA
Maximize Conversions
Broad Match
Performance Max
Display Network
Search Partners
Budget increase
Aggressive keyword expansion
Auto-apply recommendations
```

---

## Search Term Classification

For every meaningful search term, classify it as:

```text
Keep
Watch
Add Negative
Competitor
Far Location
Move To General Vet Campaign
Move To Service Campaign
Move To Brand Campaign
Research Intent
```

Do not overreact to impressions only.

Prioritize action when a term has:

```text
Clicks
Spend
Repeated irrelevant impressions
Competitor intent
Far-location intent
Non-client intent
```

---

## Negative Keyword Review

Verify:

1. Global Vet Waste Negatives are applied where needed.
2. Competitor negatives are present.
3. Far-city negatives are present where justified.
4. Negatives are not blocking good urgent or service intent.
5. New negatives are based on actual search-term evidence.

---

## Conversion Tracking Review

Primary conversions should be real lead actions:

```text
Phone calls from ads
Website call clicks
Booking completion
Appointment request
Zoho form submission
Qualified offline lead import
```

These should not be primary:

```text
Page view
Scroll
Time on site
Generic engagement
Directions
Contact page visit
```

If tracking is incomplete, say so clearly.

Do not recommend Smart Bidding until tracking is clean.

---

## Output Format

Use this exact structure:

## A. Access Check

State what you could and could not access.

## B. Executive Verdict

State whether the account is:

```text
Safe to continue
Needs minor fixes
Needs urgent correction
Not ready to scale
Ready for controlled expansion
```

## C. What Is Set Up Correctly

List what is right.

## D. Critical Issues

Use this table:

| Severity | Issue | Evidence | Impact | Recommended Action |
|---|---|---|---|---|

## E. Campaign Performance Summary

Use this table:

| Campaign | Spend | Impressions | Clicks | CTR | Avg CPC | Conversions | CPA | Verdict |
|---|---:|---:|---:|---:|---:|---:|---:|---|

## F. Search Term Decisions

Use this table:

| Search Term | Campaign | Clicks | Cost | Verdict | Action |
|---|---|---:|---:|---|---|

## G. Keyword Decisions

Use this table:

| Keyword | Match Type | Cost | Clicks | Conversions | Verdict | Action |
|---|---|---:|---:|---:|---|---|

## H. Negative Keyword Recommendations

Group by theme:

```text
Competitor
Far Location
Shelter / Adoption
Jobs / Education
Free / Cheap
Grooming / Boarding
Research Intent
```

## I. Conversion Tracking Verdict

State whether tracking is ready for:

```text
Maximize Clicks
Maximize Conversions
Target CPA
Performance Max
```

## J. Landing Page / CRO Findings

Review message match, CTA clarity, mobile experience, phone consistency, and conversion friction.

## K. Do Not Change Yet

List what must not be changed.

## L. Next 7-Day Action Plan

Give prioritized next actions.

## M. Repo Files To Update

State which repo files should be updated based on findings:

```text
CURRENT_STATE.md
CHANGELOG.md
05_negatives/master_negative_list.md
06_reports/weekly_audits/
09_exports/processed_reports/
02_campaigns/[campaign]/optimization_notes.md
```

---

## Operating Rule

Do not make edits automatically.

If you find an urgent issue, label it:

```text
Recommended Immediate Fix
```

and wait for approval.
