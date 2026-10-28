# Leave Planner & Approval Tracker

A single-page prototype for a small team to submit leave requests, review them against a monthly team calendar, and track approval status.

## Screens

- **Request leave:** applicant name, application date, start and end dates, with working-day duration calculated automatically (weekends and listed public holidays excluded).
- **Review:** monthly calendar showing approved, pending and selected leave, with an over-limit flag for days when too many people are away. The team lead can approve, reject, or reopen a past decision.
- **Status:** requesters pick their name to see each request as Pending, Approved or Not approved.

## Prototype limits

- No login.
- Data is saved in the viewer's browser (`localStorage`), so it is not shared between people or devices.
- The public holiday list (Singapore) is partial and is defined in the `HOL` object in `index.html`.
- The over-limit threshold defaults to more than 2 people away and can be changed on the Review screen.

## Deploy on Vercel

This is a static site with no build step.

1. Import this repository in Vercel.
2. Framework preset: **Other**. Leave the build command and output directory empty.
3. Deploy. `vercel.json` only adds clean URLs and basic security headers.

To preview locally, open `index.html` in a browser.
