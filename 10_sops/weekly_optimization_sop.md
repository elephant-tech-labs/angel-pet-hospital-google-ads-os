# Weekly Google Ads Optimization SOP

## Purpose

This SOP defines how Angel Pet Hospital Google Ads should be reviewed and optimized weekly.

The goal is to improve qualified leads, reduce wasted spend, improve conversion tracking, and scale only when quality is proven.

---

## Weekly Workflow

1. Export or inspect last 7 days of Google Ads data.
2. Run Codex weekly audit prompt.
3. Review Codex audit with strategy director.
4. Approve, delay, or reject recommendations.
5. Implement approved changes manually in Google Ads.
6. Run Codex post-change QA.
7. Update repo files.
8. Prepare client-facing summary if needed.

---

## Required Weekly Data

Review:

- Campaign performance
- Search terms
- Search keywords
- Negative keywords
- Ads
- Assets
- Locations
- Devices
- Hour/day performance
- Conversion actions
- Landing page performance
- Call data if available
- Booking/form data if available

---

## Weekly Performance Metrics

Track:

| Metric | Why It Matters |
|---|---|
| Spend | Budget control |
| Impressions | Demand volume |
| Clicks | Traffic volume |
| CTR | Ad relevance |
| Avg CPC | Cost pressure |
| Conversions | Lead volume |
| Cost per conversion | Efficiency |
| Calls | Primary lead action |
| Call duration | Lead quality |
| Form submits | Secondary lead action |
| Booking requests | High-intent lead action |
| Search term quality | Traffic quality |
| Wasted spend | Control |
| Location performance | Geo quality |
| Device performance | Mobile/call behavior |

---

## Weekly Search Term Review

Classify each meaningful search term as:

```text
Keep
Watch
Add Negative
Competitor
Far Location
Move To General Vet
Move To Service Campaign
Research Intent
```

Prioritize search terms with:

- clicks
- spend
- repeated poor intent
- competitor intent
- far-location intent
- non-client intent

Do not overreact to impressions only.

---

## Weekly Keyword Review

For each keyword, check:

- impressions
- clicks
- cost
- conversions
- search-term quality
- CPC
- intent match

Decision categories:

```text
Keep
Watch
Pause
Tighten match type
Move to another campaign
Add negative
```

Do not pause a keyword from tiny data unless it is clearly generating bad search terms.

---

## Weekly Negative Keyword Review

Update:

```text
05_negatives/master_negative_list.md
```

Only add negatives that protect budget without blocking good intent.

Every major negative addition should be recorded in:

```text
CHANGELOG.md
```

---

## Weekly Landing Page Review

Check:

- message match
- phone number consistency
- mobile CTA visibility
- form friction
- booking link
- directions link
- load speed
- broken buttons
- trust proof
- call-first hierarchy

If users click but do not call/book/form-submit, investigate landing page friction.

---

## Weekly Conversion Tracking Review

Check whether primary conversions are real leads:

Allowed primary:

```text
Phone calls from ads
Website call clicks
Booking completion
Appointment request
Zoho form submission
Qualified offline lead import
```

Should not be primary:

```text
Page view
Scroll
Time on site
Engagement
Directions
Contact page view
```

---

## Weekly Scaling Decision

Do not scale unless:

- search terms are clean
- lead quality is confirmed
- tracking is working
- CPC is stable
- no major competitor or far-location waste
- clinic can handle additional lead volume

Scale slowly:

```text
10% to 20% budget increase at a time
```

Do not double budgets based on one good week.

---

## Weekly Bidding Decision

Stay on Maximize Clicks until tracking is clean.

Only consider Maximize Conversions when:

- real lead conversions are tracked
- weak actions are not primary
- there is enough lead volume
- search terms are clean
- clinic confirms lead quality

Only consider Target CPA after stable conversion volume.

---

## Weekly Output

Each week produce:

1. Internal audit
2. Change recommendations
3. Approved action list
4. Post-change QA
5. Client-facing update if needed

---

## Weekly Report Storage

Save weekly audits in:

```text
06_reports/weekly_audits/
```

Save processed summaries in:

```text
09_exports/processed_reports/
```

Save client reports in:

```text
06_reports/client_reports/
```

Update:

```text
CURRENT_STATE.md
CHANGELOG.md
```

when changes are made.
