# Processed Google Ads Summary - 2026-05-06

## Account

Angel Pet Hospital  
Google Ads customer: 1957941070  
Timezone: America/Los_Angeles

---

## Executive Summary

The Google Ads account required immediate correction on 2026-05-06.

Campaign #1 was temporarily re-enabled because of concern that the new urgent campaign might not receive enough clicks. After Codex QA, Campaign #1 was found to be structurally unsafe and was recommended to be paused again.

The urgent campaign was mostly aligned with the approved strategy, but live bidding still showed Maximize Conversions with tCPA instead of the approved Maximize Clicks strategy. This was a setup mismatch and required correction.

The main decision from the QA:

```text
Pause Campaign #1 again.
Restore urgent campaign bidding to Maximize Clicks.
Run urgent campaign only for the next 24 hours after post-change QA passes.
```

Codex found that Campaign #1 spent $86.80 in one account day, generated 27 clicks and 4 tracked calls, but produced poor search-term quality including shelter, competitor, far-location, and weak general-vet searches. These calls should not be treated as confirmed qualified leads without clinic verification. :contentReference[oaicite:0]{index=0}

---

## Campaign Performance Summary

| Campaign | Status During QA | Spend | Impressions | Clicks | CTR | Avg CPC | Conversions | Conversion Type | Verdict |
|---|---|---:|---:|---:|---:|---:|---:|---|---|
| Campaign #1 | Enabled | $86.80 | 833 | 27 | 3.24% | $3.21 | 4 | Calls from ads | Pause |
| Search - Urgent Vet Care - Edmonds | Enabled | $26.74 | 180 | 7 | 3.89% | $3.82 | 1 | Calls from ads | Continue after bid fix |
| Search - Urgent Vet Care - Edmonds, May 5 context | Enabled | $13.76 | 71 | 3 | 4.23% | $4.59 | 0 | None | Early learning |
| Website traffic-Search-1 | Paused | $0 | 0 | 0 | 0% | $0 | 0 | None | Keep paused |

---

## Settings Findings

| Campaign | Finding | Impact | Decision |
|---|---|---|---|
| Campaign #1 | Maximize Conversions with tCPA $17.00 | Unsafe because tracking is not mature and campaign structure is poor | Pause |
| Campaign #1 | Display/content network was on | Risk of low-quality traffic | Pause |
| Campaign #1 | No Global Vet Waste Negatives found | Allows shelter, competitor, far-location, and irrelevant searches | Pause |
| Campaign #1 | Final URL pointed to `business.google.com` | Weak landing page control and poor conversion path | Pause |
| Urgent campaign | Maximize Conversions/tCPA $17.40 live during QA | Mismatch with repo-approved Maximize Clicks setup | Restore Maximize Clicks |
| Urgent campaign | Search Partners off, Display off, AI Max off | Correct | Keep |
| Urgent campaign | Final URL was urgent landing page | Correct | Keep |
| Urgent campaign | Global Vet Waste Negatives applied | Correct | Keep |

Codex confirmed Campaign #1 was structurally unsafe because Display/content was on, the Global Vet Waste Negatives list was not applied, bidding used Maximize Conversions with tCPA, the final URL pointed to `business.google.com`, and search terms included competitor, shelter, far-location, and weak general-vet traffic. :contentReference[oaicite:1]{index=1}

---

## Search Quality Summary

### Campaign #1

Campaign #1 search-term quality was poor and not acceptable for a controlled live campaign.

Examples of problematic terms:

```text
shelton animal shelter
ridgetop animal hospital
all creatures arlington
alpine vet monroe
animal shelter marysville wa
vet queen anne
vets oak harbor
```

These terms show multiple waste patterns:

- shelter intent
- competitor intent
- far-location intent
- weak general-vet intent
- service mismatch

Campaign #1 should not be kept active just because it generated clicks or tracked calls.

---

### Urgent Campaign

Urgent campaign search terms were cleaner.

Examples:

```text
pet emergency near me
emergency vet
vet near me
veterinary clinic near me
affordable emergency vet near me
```

Interpretation:

| Term | Interpretation | Action |
|---|---|---|
| pet emergency near me | Good urgent intent | Keep |
| emergency vet | Good urgent intent | Keep |
| vet near me | General vet intent, but one conversion occurred | Watch and use for General Vet planning |
| veterinary clinic near me | General vet intent | Move learning to General Vet campaign |
| affordable emergency vet near me | Price-sensitive urgent query | Watch / consider urgent negative |

Blue Pearl did not reappear after negatives were added, so it is not a current urgent issue unless it appears again. :contentReference[oaicite:2]{index=2}

---

## Conversion Quality Notes

Campaign #1 generated 4 tracked calls from ads.

However, because Campaign #1 produced poor search-term quality, those calls should not be considered confirmed qualified leads until the clinic verifies the calls.

Urgent campaign generated 1 tracked call from ads.

This should also be treated as a tracked call, not a confirmed qualified lead, until call quality is confirmed.

Current tracking status:

```text
Smart Bidding is not safe yet.
```

Reason:

- call quality is not verified
- tracking is not mature
- website call-click tracking still needs improvement
- booking/form tracking is still incomplete
- weak conversion signals must not guide bidding

---

## Decisions Made

### Campaign #1

Decision:

```text
Pause again
```

Reason:

```text
Campaign #1 is structurally unsafe and not part of the approved long-term strategy.
```

Specific reasons:

- Display/content network was on
- No Global Vet Waste Negatives were applied
- Bidding used Maximize Conversions with tCPA
- Final URL was `business.google.com`
- Search terms included shelter, competitor, far-location, and weak general-vet queries
- It spent $86.80 in one account day
- It generated tracked calls, but quality is not verified

---

### Urgent Campaign

Decision:

```text
Continue after bidding fix
```

Reason:

```text
The urgent campaign has the correct Search-only structure, correct final URL, correct phone number, and correct negative keyword list. The main issue was bidding mismatch.
```

Required correction:

```text
Restore bidding to Maximize Clicks.
```

---

## Actions Completed

| Priority | Action | Campaign | Status |
|---|---|---|---|
| P0 | Pause Campaign #1 again | Campaign #1 | Completed manually |
| P0 | Restore bidding to Maximize Clicks | Search - Urgent Vet Care - Edmonds | Completed manually |
| P1 | Preserve Campaign #1 learnings for General Vet planning | General Vet docs | In progress |
| P1 | Update repo docs | Repo | In progress |

---

## Pending Actions

| Priority | Action | Reason |
|---|---|---|
| P1 | Run Codex post-change QA | Verify Campaign #1 is paused and urgent campaign is safe |
| P1 | Confirm urgent campaign bidding is now Maximize Clicks | Ensure live Google Ads matches repo strategy |
| P1 | Confirm urgent call quality with clinic | Determine if the 1 tracked call was a qualified lead |
| P1 | Consider adding `affordable` as urgent campaign negative | Price-sensitive urgent search appeared |
| P2 | Continue General Vet campaign planning | Use useful learning but do not reuse Campaign #1 |
| P2 | Build `/veterinarian-edmonds` landing page before launching General Vet | Avoid homepage/default landing page weakness |

---

## Useful Learnings For Future General Vet Campaign

Campaign #1 should not be reused, but it provided useful planning signals.

Useful themes:

```text
bothell pet hospital
animal hospital variants
general vet near me intent
brand query: angel pet hospital
local competitor terms
```

These should inform future campaign planning, but only through a clean rebuilt structure.

General Vet campaign should be built as:

```text
Search - General Vet - Edmonds
```

With:

- Search only
- Exact and Phrase match only
- dedicated `/veterinarian-edmonds` landing page
- Global Vet Waste Negatives
- campaign-specific urgent negatives
- campaign-specific competitor/far-location controls
- Maximize Clicks at launch
- no Display
- no Search Partners
- no Broad Match
- no Target CPA

---

## What Not To Do

Do not:

- re-enable Campaign #1
- keep Campaign #1 active because it generated calls
- increase budget today
- use Target CPA
- use Maximize Conversions
- enable Display
- enable Search Partners
- use Broad Match
- launch General Vet before the landing page is ready
- treat tracked calls as confirmed qualified leads without clinic verification

---

## Final Verdict

The account is safer after the manual fixes, but it still requires post-change QA.

The correct operating decision is:

```text
Run only Search - Urgent Vet Care - Edmonds for the next 24 hours after post-change QA passes.
```

Campaign #1 should remain paused and should be used only as historical research evidence.
