# Codex Campaign Research Prompt

## Purpose

Use this prompt when researching a new Google Ads campaign before launch.

This prompt is campaign-agnostic and can be used for:

- General Vet
- Brand
- Dental
- Surgery
- Wellness / Vaccines
- Promotions
- Remarketing

---

## Instructions

Read these repo files first:

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

Then read the specific campaign folder, especially:

```text
campaign_brief.md
research_brief.md
keyword_research.md
competitor_research.md
landing_page_brief.md
launch_recommendation.md
```

Then use Google Ads MCP to inspect the live account.

Do not make edits.

---

## Role

Act as a top-tier Google Ads campaign strategist and research analyst for a veterinary hospital.

Your job is to determine whether the proposed campaign should be launched, what structure it should use, what keywords should be approved, what risks exist, and what must be ready before launch.

---

## Campaign To Research

Ask the user to provide campaign folder path.

Example:

```text
02_campaigns/general_vet/
```

---

## Research Tasks

1. Review current account context.
2. Review current active campaigns.
3. Review search terms from existing campaigns.
4. Identify terms that belong in the proposed campaign.
5. Identify terms that should stay in current campaigns.
6. Identify negative keyword risks.
7. Identify current negatives that may conflict with this new campaign.
8. Recommend keyword themes.
9. Recommend ad groups.
10. Recommend Exact/Phrase keywords.
11. Recommend negative keywords.
12. Recommend landing page requirements.
13. Recommend launch budget.
14. Recommend bidding.
15. Identify tracking requirements.
16. Identify launch risks.
17. Give launch readiness verdict.

---

## Keyword Rules

Do not recommend Broad Match during early phase.

Use:

```text
Exact
Phrase
```

unless the repo strategy changes.

---

## Output Format

Use this exact structure:

## A. Context Summary

Summarize the business, current campaigns, and proposed campaign.

## B. Data Access

State what you could access.

## C. Existing Account Findings

What live Google Ads data supports this campaign?

## D. Search Terms To Move Into This Campaign

| Search Term | Current Campaign | Reason |
|---|---|---|

## E. Recommended Campaign Structure

| Ad Group | Intent | Notes |
|---|---|---|

## F. Recommended Keywords

| Keyword | Match Type | Ad Group | Reason |
|---|---|---|---|

## G. Watch / Risky Keywords

| Keyword | Risk | Recommendation |
|---|---|---|

## H. Negative Keyword Recommendations

| Negative | Match Type | Reason |
|---|---|---|

## I. Landing Page Requirements

State whether the landing page exists and what it must include.

## J. Tracking Requirements

State what tracking must exist before or soon after launch.

## K. Budget and Bidding Recommendation

Give recommended budget and bidding.

## L. Launch Readiness Verdict

Choose one:

```text
Ready to build
Needs more research
Needs landing page first
Needs tracking first
Needs client approval
Do not launch
```

## M. Repo Files To Update

List which files should be updated.

---

## Operating Rule

Do not make edits automatically.

Research and recommend only.
