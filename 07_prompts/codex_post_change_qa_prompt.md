# Codex Post-Change QA Prompt

## Purpose

Use this prompt after making changes in Google Ads.

The goal is to verify that the live account matches the approved strategy and that no accidental settings, URL, phone, budget, bidding, or tracking mistakes were introduced.

Codex must inspect the live Google Ads account through MCP and report findings.

Do not make edits automatically.

---

## Required Files To Read First

Read:

```text
README.md
MASTER_CONTEXT.md
CURRENT_STATE.md
DECISION_RULES.md
CHANGELOG.md
01_strategy/account_strategy.md
```

Then inspect the live account.

---

## Role

Act as a senior Google Ads QA auditor.

Your job is to catch mistakes before they waste budget.

---

## Campaigns To Check

Check all active campaigns.

If the change was made to a specific campaign, check that campaign first.

Current primary campaign:

```text
Search - Urgent Vet Care - Edmonds
```

---

## QA Checklist

Verify:

1. Campaign status
2. Daily budget
3. Bidding strategy
4. Search Partners status
5. Display Network status
6. AI Max / final URL expansion
7. Location targeting
8. Location options
9. Ad schedule
10. Campaign goals
11. Conversion actions
12. Keywords
13. Match types
14. Negative keyword list application
15. Ads
16. Final URLs
17. Display paths
18. Call asset phone number
19. Sitelinks
20. Callouts
21. Structured snippets
22. Location assets
23. Disapprovals
24. Limited status warnings
25. Tracking warnings

---

## Approved Urgent Campaign Settings

For the urgent campaign, expected setup is:

```text
Campaign type: Search
Budget: $70/day
Bidding: Maximize Clicks
Search Partners: Off
Display Network: Off
AI Max / Final URL Expansion: Off
Match types: Exact and Phrase only
Broad Match: Not allowed
Landing page: https://www.angelpethospital.com/urgent-vet-care-edmonds
Phone: (425) 673-0700
Phone link: tel:+14256730700
Negative list: Global Vet Waste Negatives applied
```

---

## Red Flag Settings

Flag immediately if any of these are found:

```text
Target CPA turned on
Maximize Conversions turned on before tracking is clean
Display Network on
Search Partners on
Broad Match keywords active
AI Max / final URL expansion on
Homepage used as final URL for urgent campaign
Wrong phone number
No negative keyword list applied
Page view or engagement used as primary conversion
Budget higher than approved
```

---

## Output Format

Use this exact format:

## A. QA Verdict

State one:

```text
Passed
Passed with minor issues
Failed - urgent correction needed
```

## B. Settings Correct

List what is correct.

## C. Issues Found

Use this table:

| Severity | Issue | Expected | Actual | Impact | Recommended Action |
|---|---|---|---|---|---|

## D. Campaign-Specific QA

Use this table:

| Campaign | Budget | Bidding | Networks | Final URL | Negatives | Phone | Verdict |
|---|---:|---|---|---|---|---|---|

## E. Conversion QA

State whether conversion goals are safe for current bidding.

## F. Asset QA

State whether ads, callouts, snippets, sitelinks, and call assets are correct.

## G. Do Not Change

List items that should remain unchanged.

## H. Required Human Actions

List only actions that need manual implementation.

## I. Repo Files To Update

State which repo files need updates.

---

## Operating Rule

Do not make edits automatically.

Report only.
