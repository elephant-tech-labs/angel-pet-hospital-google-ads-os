# Master Negative Keyword System

## Purpose

This file is the source of truth for negative keyword strategy across Angel Pet Hospital Google Ads campaigns.

Negative keywords are used to prevent wasted spend from searches that are unlikely to become qualified clinic leads.

The goal is not to block traffic aggressively. The goal is to block traffic that clearly shows:

- non-client intent
- competitor intent
- job seeker intent
- research intent
- shelter/adoption intent
- free/cheap/low-cost intent
- grooming/boarding/retail intent
- far-location intent

---

## Core Rule

Never add negatives blindly.

Add negative keywords when the search term shows clear evidence of waste, poor lead quality, or irrelevant intent.

Prioritize adding negatives when a term has:

- clicks
- cost
- repeated impressions
- competitor intent
- non-client intent
- far-location intent
- low-quality lead behavior

---

## Global Vet Waste Negatives

These should generally be applied across Google Ads campaigns unless a specific campaign has a reason to allow them.

### Shelter / Adoption / Rescue

```text
adoption
adopt
shelter
rescue
foster
fostering
animal control
humane society
spca
volunteer
```

### Free / Cheap / Low Cost

```text
free
cheap
low cost
low-cost
affordable
discount
```

Use care with `affordable` and `discount`. These may be allowed in future promotional campaigns, but they should generally be blocked from urgent-care campaigns.

### Jobs / Careers / Education

```text
jobs
job
career
careers
salary
school
course
training
how to become
internship
vet school
veterinary jobs
veterinary assistant salary
```

### Grooming / Boarding / Retail

```text
grooming
boarding
pet store
supplies
food
dog grooming
pet grooming
pet boarding
pet supplies
dog food
cat food
```

### Wildlife / Zoo / Non-Clinic Intent

```text
wildlife
zoo
animal control
```

---

## Competitor Negatives

Use competitor negatives unless there is an approved competitor conquesting strategy.

For the current urgent-care campaign, competitor terms should be blocked because the campaign budget is limited and should focus on direct urgent-intent searches.

```text
blue pearl
bluepearl
blue pearl kirkland
blue pearl renton
blue pearl olympia
blue pearl seattle
banfield
vca
veg
veterinary emergency group
```

---

## Far-City Negatives

Urgent vet care is distance-sensitive. Far-location searches usually do not convert well unless the clinic is a true emergency destination and users are willing to travel.

Use far-city negatives carefully and based on actual search-term data.

Current far-city negatives / watchlist:

```text
spokane
spokane valley
olympia
renton
kirkland
poulsbo
issaquah
lake stevens
```

Watch before blocking unless spend occurs:

```text
everett
seattle
stanwood
bellevue
redmond
```

---

## Phrase Negative Examples

Use phrase match negatives for multi-word bad-intent queries.

```text
"animal shelter"
"pet adoption"
"dog adoption"
"cat adoption"
"free vet"
"low cost vet"
"cheap vet"
"vet jobs"
"veterinary jobs"
"vet school"
"how to become a vet"
"pet grooming"
"dog grooming"
"pet boarding"
```

---

## Exact Negative Examples

Use exact negatives when one specific query is bad but related broader searches may still be useful.

Examples:

```text
[blue pearl kirkland]
[blue pearl renton]
[blue pearl olympia]
[blue pearl seattle]
```

---

## Do Not Block Core Vet Intent

Do not add these as negatives unless specifically approved:

```text
urgent
emergency
vet
veterinarian
animal hospital
pet hospital
sick pet
open now
same day
appointment
near me
edmonds
lynnwood
shoreline
mountlake terrace
woodway
brier
```

---

## Campaign-Specific Negative Logic

### Urgent Vet Campaign

Block:
- shelter/adoption/rescue/foster
- free/cheap/low-cost
- jobs/school/training
- grooming/boarding
- competitor terms
- far-location terms when they click or repeatedly appear

Watch:
- general vet terms
- broad animal hospital terms
- emergency terms if clinic cannot handle emergency-adjacent calls

Do not block:
- urgent vet
- emergency vet
- sick pet
- open now
- same-day vet
- animal hospital open now

### General Vet Campaign

Block:
- shelter/adoption/rescue/foster
- jobs/school/training
- grooming/boarding
- free/cheap/low-cost unless promotional strategy allows it

May allow:
- vet near me
- animal hospital near me
- dog vet near me
- cat vet near me
- veterinarian near me

### Brand Campaign

Usually block:
- competitor names
- job seeker terms
- free/cheap/low-cost if not part of strategy

Allow:
- Angel Pet Hospital
- Angel Pet Hospital Edmonds
- Angel Pet Hospital phone
- Angel Pet Hospital hours

### Dental Campaign

Block unrelated services if they spend:
- surgery
- emergency
- grooming
- boarding
- adoption
- jobs

Allow:
- pet dental cleaning
- dog teeth cleaning
- cat dental care
- veterinary dental cleaning

### Surgery Campaign

Block unrelated services if they spend:
- grooming
- boarding
- adoption
- jobs
- dental if it causes mismatch

Allow:
- pet surgery
- dog surgery
- cat surgery
- veterinary surgery

---

## Search-Term Review Decision Table

Use this format when reviewing search terms:

| Search Term | Verdict | Action |
|---|---|---|
| emergency vet | Keep | No action |
| blue pearl kirkland | Competitor | Add negative |
| veterinary clinic near me | Watch / General | Move to General campaign later |
| animal shelter near me | Waste | Add negative |
| dog grooming near me | Waste | Add negative |
| emergency vet lake stevens | Far-location | Watch or negative if clicked |

---

## Negative Keyword Change Log

Every important negative keyword addition should also be recorded in:

```text
CHANGELOG.md
```

Example:

| Date | Negative Added | Reason | Campaign/List |
|---|---|---|---|
| 2026-05-05 | blue pearl | Competitor click appeared | Global Vet Waste Negatives |
| 2026-05-05 | spokane | Far-location intent appeared | Global Vet Waste Negatives |

---

## Current Strategy

The negative keyword system should protect budget without choking useful urgent demand.

The goal is to reduce wasted spend while preserving qualified local searches that can become calls, appointments, and clinic visits.
