# Release Record

## Release 1: first version of the RTP Reading Club page (2026-10-19)

**Live URL:** https://book-club-website-ai.vercel.app
_(This is the address in the repository's GitHub "Website" setting. Claude
couldn't open it from the cloud container, so it's taken as given.)_

**Commit on `main`:** `b0de089` (Record browser test results and update project state)
- The page itself (`index.html`) was last changed in `cb8db28`. `b0de089`
  only updated `test-report.md` and `project-state.md`.
- Vercel reported "Deployment has completed" for `b0de089` at 16:07 UTC:
  https://vercel.com/meek-learning/book-club-website-ai/8kNpEfiGL5YAZKzPTJTvP1uu5mbU

**What's in this release:** a single `index.html` (styles included) with a
"Fictional site" notice, the heading "RTP Reading Club", a "See the next
gathering" button, and the About, Next Gathering and Next Book Read sections.

### What you observed
- You opened the live Vercel site and reported that **everything works as
  expected**.
- On that basis, all five completion checks from `project-brief.md` are recorded
  as **Passed** in your column of `test-report.md`.
- You checked the deployment of `cb8db28`. `b0de089` didn't change the page.

### What Claude verified
- All five completion checks **Passed** in headless Chromium, with the file
  opened directly, at phone (375×667) and laptop (1280×800) sizes.
- No sideways scrolling on the phone size, no browser errors, and a button
  large enough to tap (234×51 px).
- GitHub shows Vercel's deployment of `b0de089` as successful.

### Limitations
- **Fictional content.** The club, reading room and gathering are made up. Only
  the books and author are real.
- **Fixed dates.** The Next Gathering (October 24, 2026) and Next Book Read are
  typed into the page. They won't update themselves, and the page will be out of
  date after October 24, 2026 unless someone edits it.
- **No time zone** is shown for 10:30 AM, and the reading room has no address.
- **Browsers and devices not recorded.** Your check didn't note which browsers
  or devices you used. Claude tested headless Chromium only, so Safari, Firefox
  and real phones aren't confirmed separately.
- **Live URL not opened by Claude.** The container's network couldn't reach
  the Vercel site, so Claude didn't confirm the live page directly.
- **Static page only.** By design, there's no sign-up, RSVP, payment, email,
  accounts or saved data.
