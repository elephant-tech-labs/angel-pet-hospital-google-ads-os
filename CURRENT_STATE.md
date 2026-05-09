# Current Google Ads State

Last updated: 2026-05-09

## Executive Current State

The Google Ads account is currently in a drift-recovery state.

The approved system was designed to run only controlled Search campaigns with:
- Search-only traffic
- Display Network off
- Search Partners off
- AI Max / Final URL Expansion off
- Exact and Phrase match only
- Maximize Clicks until tracking is mature
- Dedicated landing pages
- Global Vet Waste Negatives applied
- Campaigns launched only after repo approval and QA

Recent audits found the account drifted away from this approved system.

Major drift found:
- Legacy campaigns were re-enabled.
- All 4 campaigns were enabled.
- Campaigns were using Maximize Conversions with target CPA.
- Display/content network was on.
- General Vet was enabled before final repo QA approval.
- Campaign #1 spent heavily despite being previously marked unsafe.
- Website traffic-Search-1 was enabled again despite being unsafe.
- Urgent campaign settings drifted from the approved Maximize Clicks / Search-only setup.

Current operating priority:
Restore the account to a safe, controlled state before scaling.

---

## Approved Safe Operating State

Only campaigns that are:
- documented in the repo
- built from approved campaign files
- using approved settings
- QA-passed
- manually approved

should be allowed to run.

No campaign should run with:
- Display/content network on
- Search Partners on
- AI Max / Final URL Expansion on
- Broad Match
- Maximize Conversions
- Target CPA
- homepage/default landing page
- business.google.com landing page
- missing negative keyword controls

---

## Campaign Status

### Search - Urgent Vet Care - Edmonds

Strategic role: Approved urgent / emergency-adjacent Search campaign.

Current recommended status: Enabled only after settings are corrected.

Approved setup:

Status: Enabled  
Budget: $50/day for next 24h recovery period  
Bidding: Maximize Clicks  
Max CPC ceiling: $8  
Network: Google Search only  
Search Partners: Off  
Display Network: Off  
AI Max / Final URL Expansion: Off  
Landing page: https://www.angelpethospital.com/urgent-vet-care-edmonds  
Phone: (425) 673-0700  
Match types: Exact and Phrase only  
Broad match: Not allowed  
Negative list: Global Vet Waste Negatives applied  

Required urgent fix:
- Confirm bidding is Maximize Clicks, not Maximize Conversions / tCPA.
- Confirm Display/content network is off.
- Confirm Search Partners are off.
- Confirm AI Max / Final URL Expansion is off.
- Confirm urgent landing page is used.
- Confirm phone asset is `(425) 673-0700`.

Recent urgent search-term note:
- `emergency vet arlington wa` appeared as a far-location urgent query.
- Add exact negative: `[emergency vet arlington wa]`
- Do not add broad `"arlington"` unless repeated clicked waste appears.

Current verdict:
Urgent can run only after the above controls are confirmed.

---

### Search - General Vet - Edmonds

Strategic role: New general veterinary care / new-patient campaign.

Current recommended status: Paused until pre-launch QA passes.

Planned setup:

Status: Paused until QA  
Budget: $30/day after approval  
Bidding: Maximize Clicks  
Network: Google Search only  
Search Partners: Off  
Display Network: Off  
AI Max / Final URL Expansion: Off  
Landing page: https://www.angelpethospital.com/veterinarian-edmonds  
Match types: Exact and Phrase only  
Broad match: Not allowed  
Negative list: Global Vet Waste Negatives applied  
Campaign-specific urgent negatives required  

Approved ad groups:
- Vet / Veterinarian Near Me
- Animal Hospital / Veterinary Clinic
- Dog & Cat Vet
- Local City Vet

Recent issue:
General Vet was enabled before final repo QA and ran with wrong settings:
- $50/day instead of planned $30/day
- Maximize Conversions / tCPA
- Display/content network on

Required fix:
- Pause General Vet.
- Correct budget to $30/day.
- Set bidding to Maximize Clicks.
- Turn Display/content network off.
- Turn Search Partners off.
- Turn AI Max off.
- Confirm all 4 ad groups are complete.
- Confirm final URL is `/veterinarian-edmonds`.
- Apply Global Vet Waste Negatives.
- Add campaign-specific urgent negatives.
- Add competitor negatives before launch.

New negative from General Vet drift:
- `"helping hands vet"`
- `"helping hands vet lynnwood"`

Current verdict:
General Vet is strategically approved, but not approved to run until QA passes.

---

### Campaign #1

Strategic role: Legacy unsafe campaign.

Current recommended status: Paused.

Reason:
Campaign #1 was previously identified as structurally unsafe and not part of the approved long-term strategy. Earlier audit evidence showed Campaign #1 had major structural risks including Display/content enabled, Maximize Conversions/tCPA, weak landing URL behavior, no proper negative controls, and low-quality search terms such as shelter, competitor, and far-location searches. :contentReference[oaicite:0]{index=0}

Recent issue:
Campaign #1 was re-enabled and spent heavily again.

Recent drift found:
- Status: Enabled
- Budget: $200/day
- Spend: $266.96 in roughly 24h
- Bidding: Maximize Conversions / tCPA
- Display/content network: On
- Final URL: business.google.com
- Repo approved: No

Required action:
- Pause Campaign #1 immediately.
- Do not optimize or scale Campaign #1.
- Use Campaign #1 data only as dirty legacy research.
- If the client insists it remains live, it must be treated as a restricted temporary safety-net campaign and must be rebuilt with strict controls before running.

Current verdict:
Pause immediately.

---

### Website traffic-Search-1

Strategic role: Legacy unsafe campaign.

Current recommended status: Paused.

Recent drift found:
- Status: Enabled
- Budget: $100/day
- Bidding: Maximize Conversions / tCPA
- Display/content network: On
- AI Max: On
- Final URL: Homepage
- Search term found: `animal shelter`
- Repo approved: No

Required action:
- Pause immediately.
- Do not relaunch unless rebuilt from scratch under approved rules.

Current verdict:
Pause immediately.

---

## Current Open Issues

### Critical

1. Legacy campaigns were re-enabled.
2. All campaigns drifted to Maximize Conversions / tCPA.
3. Display/content network was enabled.
4. General Vet ran before QA approval.
5. Campaign #1 spent heavily while structurally unsafe.
6. Website traffic-Search-1 ran again despite unsafe setup.
7. Client/manual changes are bypassing the repo-approved operating system.

### High

1. Conversion tracking is not mature enough for Smart Bidding.
2. Website call-click tracking still needs setup.
3. Booking tracking still needs setup.
4. Zoho form tracking still needs setup.
5. Lead quality is not yet verified from clinic outcomes.
6. Campaigns need daily QA until stable.

### Medium

1. Urgent campaign schedule should be cleaned to 9:00 AM - 7:00 PM if still showing odd minute offsets.
2. Business name asset issue may remain unresolved.
3. Asset copy should be visually spot-checked in Google Ads UI.
4. Need consistent repo updates after manual changes.

---

## Required Immediate Fixes

Do these before scaling or trusting performance data:

1. Pause Campaign #1.
2. Pause Website traffic-Search-1.
3. Pause Search - General Vet - Edmonds until QA passes.
4. Fix Urgent to Maximize Clicks.
5. Turn Display/content network off on every Search campaign.
6. Turn Search Partners off.
7. Turn AI Max / Final URL Expansion off.
8. Confirm Urgent final URL:
   `https://www.angelpethospital.com/urgent-vet-care-edmonds`
9. Confirm General Vet final URL:
   `https://www.angelpethospital.com/veterinarian-edmonds`
10. Apply Global Vet Waste Negatives where appropriate.
11. Add exact urgent negative:
   `[emergency vet arlington wa]`
12. Add General Vet competitor negatives:
   `"helping hands vet"`
   `"helping hands vet lynnwood"`
13. Run Codex pre-launch QA before enabling General Vet.
14. Run daily full-account QA until account drift is controlled.

---

## Current Budget Recommendation

For next 24h recovery period:

| Campaign | Recommended Budget | Status |
|---|---:|---|
| Search - Urgent Vet Care - Edmonds | $50/day | Enabled only after fixes |
| Search - General Vet - Edmonds | $0 live spend | Paused until QA |
| Campaign #1 | $0 | Paused |
| Website traffic-Search-1 | $0 | Paused |

Do not increase budget until:
- urgent settings are corrected
- General Vet passes QA
- search terms are clean
- tracking is verified
- client/manual drift is controlled

---

## Current Operating Rule

No campaign should be enabled unless:

1. It exists in the repo.
2. Campaign brief is complete.
3. Keywords are documented.
4. Ads are documented.
5. Negatives are documented.
6. Landing page is live and correct.
7. Tracking plan is acceptable for current bidding.
8. Campaign is built paused first.
9. Codex QA passes.
10. Human approval is given.
11. Change is logged in `CHANGELOG.md`.

---

## Do Not Do

Do not:
- re-enable Campaign #1
- re-enable Website traffic-Search-1
- enable General Vet before QA
- use Maximize Conversions
- use Target CPA
- enable Display
- enable Search Partners
- enable AI Max
- add Broad Match
- increase budget
- send paid traffic to homepage
- send paid traffic to business.google.com
- trust conversions until tracking is cleaned
- treat calls as qualified leads without clinic confirmation

---

## Next Required QA

Run Codex full-account QA after manual fixes.

QA must check:
- campaign statuses
- budgets
- bidding strategies
- networks
- Display/content setting
- Search Partners
- AI Max
- final URLs
- ad groups
- keywords and match types
- negative keyword lists
- call asset phone number
- assets
- search terms
- spend
- conversions
- whether any non-approved campaign is enabled

---

## Repo Files To Update After Fixes

Update:
- `CURRENT_STATE.md`
- `CHANGELOG.md`
- `06_reports/daily_qa/2026-05-09_daily_qa.md`
- `09_exports/processed_reports/2026-05-09_processed_summary.md`
- `02_campaigns/general_vet/launch_recommendation.md`
- `02_campaigns/general_vet/negatives.md`
- `05_negatives/master_negative_list.md`

---

## Summary Verdict

The account is currently in drift-recovery mode.

The safe path is:
1. Stop legacy campaign leakage.
2. Restore Urgent to approved Search-only Maximize Clicks setup.
3. Pause General Vet until QA passes.
4. Relaunch General Vet only after settings, negatives, assets, and landing page pass QA.
5. Keep daily QA until the system is stable.
