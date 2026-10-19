# Test Report

Results are **Passed**, **Failed** or **Not tested**. "Who checked" says whether
Claude ran the check here or you checked it in your own browser.

## Round 1: first version of `index.html` (2026-10-19)

Claude's checks ran in a headless Chromium browser (Playwright) in the cloud
container, with the file opened directly (`file://`), at two screen sizes:
phone 375×667 and laptop 1280×800. Both sizes gave the same results.

| # | Completion check (from project-brief.md) | Claude (headless Chromium) | You (your browser) | Notes |
|---|---|---|---|---|
| 1 | Opening `index.html` shows the heading "RTP Reading Club" at the top. | Passed | Passed | Heading text matched exactly and sat within the first screen at both sizes. |
| 2 | Three sections appear in order: About, Next Gathering, Next Book Read. | Passed | Passed | Section headings read in that exact order. |
| 3 | Next Gathering shows October 24, 2026 at 10:30 AM, the RTP Community Reading Room, and Chapters 10-15 of *This Inevitable Ruin* (Dungeon Crawler Carl Book 7). | Passed | Passed | All three details found in the Next Gathering section. |
| 4 | Clicking the main button moves the page down so Next Gathering is in view. | Passed | Passed | After clicking, the page scrolled down and the Next Gathering heading was fully on screen (phone: about 39px from the top). |
| 5 | The page clearly says it is fictional and has no sign-up form, payment, email link or login. | Passed | Passed | Fiction notice at the top and footer. Zero forms, input boxes, buttons, email/phone links, frames or scripts found. |

**Extra checks Claude ran:**
- No sideways scrolling on the phone size: Passed
- No browser errors: Passed
- Main button is large enough to tap (234×51 px): Passed

**Not checked by Claude:** real phones, Safari, Firefox, and how the smooth
scrolling looks and feels.

## Round 1: your browser check (2026-10-19)

You checked the live site deployed by Vercel from `main` and reported that
everything works as expected, so all five checks are marked **Passed** in the
"You (your browser)" column. Which browsers and devices you used wasn't recorded.
