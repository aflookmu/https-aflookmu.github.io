# Sports Trivia Site: Spec

## Goal
A single-page sports trivia site, hosted on GitHub Pages at `aflookmu.github.io`.

## Scope
- **Sports:** football, baseball, basketball.
- **Time range:** 2000 and later only. No question, answer, or fact may refer to anything before January 1, 2000. (A question can name a record that stood for a long time, such as a championship drought, but only when the event being asked about happened in 2000 or later.)
- **Language:** American English.

## Constraints
- One file: `index.html`, with plain HTML and CSS inline.
- No JavaScript.
- No external requests of any kind: no web fonts, CDNs, images from other sites, analytics, tracking, cookies, or embeds.
- Uses the system font stack only.

## Look
- **One long scroll:** all three sports on a single page, one after another.
- **Plain and readable:** plain background, large body text, strong contrast, short line length.
- **Bold color:** each sport has its own bold accent color for its section header and question borders.
  - Football: green
  - Baseball: red
  - Basketball: orange
- Supports light and dark mode through `prefers-color-scheme`.
- Works at phone width with no sideways scrolling.

## Page structure
1. Header with the site title, a one-line intro, and jump links to each sport.
2. One section per sport, each with 7 questions.
3. Each question shows four choices. The answer and a one-sentence explanation are hidden in a `<details>` element the reader opens. This works without JavaScript.
4. A "Back to top" link after each section.
5. Footer noting that the site uses no tracking.

## Content rules
- Every fact is checked before it goes on the page.
- Each answer includes the year so the 2000+ rule is easy to verify.
- The correct choice is not always in the same position.

## Accessibility
- Semantic landmarks (`header`, `nav`, `main`, `section`, `footer`).
- One `h1`, an `h2` per sport, and questions in ordered lists.
- Visible focus outlines. Color is never the only signal.

## Out of scope for now
- Scoring, timers, or saved progress (these would need JavaScript).
- Committing and pushing. The owner will review first.
