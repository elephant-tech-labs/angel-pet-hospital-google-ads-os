# Conversion Tracking Plan

## Purpose

This file defines the conversion tracking strategy for Angel Pet Hospital Google Ads.

The goal is to track real lead actions, not vanity actions.

Google Ads should optimize toward qualified calls, appointment requests, booking actions, and form submissions.

---

## Current Tracking Status

Tracking is not yet mature enough for Smart Bidding.

Until tracking is clean and verified, campaign bidding should remain:

```text
Maximize Clicks
```

Do not use yet:

```text
Target CPA
Maximize Conversions
Performance Max optimization
Broad Match with Smart Bidding
```

---

## Primary Conversion Actions

These are real lead actions and should be used as primary conversions when properly configured.

| Conversion | Primary? | Notes |
|---|---|---|
| Phone calls from ads | Yes | Ideally count calls above a qualified duration threshold |
| Website call clicks | Yes | Track clicks on `tel:+14256730700` |
| Booking completion | Yes | Best if actual completion is trackable |
| Appointment request | Yes | If the booking flow only supports request submission |
| Zoho form submission | Yes | Should fire only after successful form submission |
| Qualified offline lead import | Later | Ideal future state after CRM/clinic feedback loop |

---

## Secondary Conversion Actions

These may be useful for analysis but should not guide bidding.

| Conversion | Primary? | Reason |
|---|---|---|
| Directions click | No | Local intent, but not a confirmed lead |
| Page view | No | Not a lead |
| Scroll | No | Not a lead |
| Time on site | No | Not a lead |
| Engagement | No | Too weak |
| Contact page visit | No | Not a lead unless form/call happens |
| Booking button click | Maybe secondary | Better to track booking completion if possible |

---

## Required Tracking Events

### 1. Phone Calls From Ads

Purpose:

Track calls directly from Google Ads call assets.

Recommended conversion name:

```text
Phone Call From Ads - Qualified
```

Recommended settings:

| Setting | Recommendation |
|---|---|
| Category | Phone call lead |
| Count | One |
| Call length | 60 seconds minimum if possible |
| Action optimization | Primary |
| Value | Optional at first |
| Attribution | Data-driven if available |

---

### 2. Website Call Clicks

Purpose:

Track people who click the phone number or Call Now button on the landing page.

Landing page:

```text
https://www.angelpethospital.com/urgent-vet-care-edmonds
```

Correct phone link:

```text
tel:+14256730700
```

Recommended conversion name:

```text
Website Call Click - Urgent Page
```

Trigger:

```text
Click URL contains tel:+14256730700
```

Recommended settings:

| Setting | Recommendation |
|---|---|
| Category | Contact or Phone call lead |
| Count | One |
| Action optimization | Primary |
| Value | Optional at first |

---

### 3. Booking Click

Purpose:

Track clicks on the Book Appointment button.

This is useful if booking completion cannot be tracked yet.

Recommended conversion name:

```text
Booking Click - Urgent Page
```

Trigger:

```text
Click URL contains booking URL
```

Recommended status:

```text
Secondary initially
```

Use as Primary only temporarily if booking completion cannot be tracked and no other website lead tracking exists.

---

### 4. Booking Completion

Purpose:

Track actual appointment request or booking completion.

Recommended conversion name:

```text
Booking Completion - Urgent Vet
```

Preferred trigger:

```text
Thank-you page view after successful booking
```

or

```text
Booking platform submit confirmation event
```

Recommended settings:

| Setting | Recommendation |
|---|---|
| Category | Book appointment |
| Count | One |
| Action optimization | Primary |
| Value | Optional initially |

---

### 5. Zoho Form Submit

Purpose:

Track successful Request Call Back form submissions.

Recommended conversion name:

```text
Zoho Form Submit - Urgent Vet
```

Best setup:

Redirect the Zoho form to a thank-you page after successful submission:

```text
/urgent-vet-care-thank-you
```

Trigger:

```text
Page URL contains /urgent-vet-care-thank-you
```

Recommended settings:

| Setting | Recommendation |
|---|---|
| Category | Submit lead form |
| Count | One |
| Action optimization | Primary |
| Value | Optional initially |

Important:

Do not track the form button click as a final lead if the form has not actually been submitted.

---

### 6. Directions Click

Purpose:

Track local intent, but do not optimize bidding toward it.

Recommended conversion name:

```text
Directions Click - Urgent Page
```

Directions URL:

```text
https://www.google.com/maps/dir/?api=1&destination=47.7845464,-122.3446758
```

Trigger:

```text
Click URL contains google.com/maps
```

Recommended status:

```text
Secondary only
```

---

## Google Tag Manager Recommendation

Use Google Tag Manager to manage tracking.

Recommended GTM events:

| Event | Trigger |
|---|---|
| Website call click | Click URL contains `tel:+14256730700` |
| Booking click | Click URL contains booking URL |
| Zoho form submit | Thank-you page view |
| Directions click | Click URL contains `google.com/maps` |

---

## GTM Installation Requirement

GTM should load globally across the Next.js website.

Pages that must include GTM:

- Homepage
- Urgent landing page
- Future general vet landing page
- Future dental page
- Future surgery page
- Future wellness/vaccines page
- Thank-you pages

---

## Next.js Implementation Notes

All phone links should use:

```text
tel:+14256730700
```

All Call Now buttons should point to the same phone link.

All Book Appointment buttons should use one clearly defined booking URL constant.

All Get Directions buttons should use:

```text
https://www.google.com/maps/dir/?api=1&destination=47.7845464,-122.3446758
```

The urgent form should redirect to:

```text
/urgent-vet-care-thank-you
```

after successful submission.

---

## Primary vs Secondary Conversion Rule

Primary conversions should include only real lead actions:

```text
Phone calls
Website call clicks
Booking completion
Appointment request
Zoho form submit
```

Secondary conversions may include:

```text
Directions
Booking click
Page view
Engagement
Scroll
Time on site
```

---

## Smart Bidding Readiness Checklist

Do not use Target CPA or Maximize Conversions until all are true:

- Phone call conversions are working.
- Website call-click conversions are working.
- Form/booking conversions are working.
- Weak actions are not primary.
- Conversion data is stable.
- Search terms are clean.
- Clinic confirms lead quality.
- There is enough conversion volume to support Smart Bidding.

---

## Future Offline Conversion Plan

Eventually, the ideal system should import offline lead quality back into Google Ads.

Possible offline statuses:

- Qualified call
- Appointment requested
- Appointment booked
- New patient booked
- Completed visit
- Revenue generated

This should be explored after the basic tracking system is stable.

---

## Current Priority

Immediate tracking priorities:

1. Install GTM / Google tag.
2. Track website call clicks.
3. Track booking clicks or booking completion.
4. Track Zoho form submissions.
5. Keep directions secondary.
6. Keep Maximize Clicks until tracking is clean.
