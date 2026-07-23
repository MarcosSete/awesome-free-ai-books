# Contributing to Awesome Free AI Books

Thanks for wanting to contribute! This list only stays useful if every entry is accurate, legal, and actually free. Please read this before opening a PR or issue.

## What counts as a valid entry

A book qualifies if **all** of the following are true:

- [ ] **Officially free.** The author, publisher, or copyright holder has chosen to make it freely available — not a leaked copy, not a "preview" of a paid book, not a time-limited promotion.
- [ ] **Permanent, not a trial.** No countdown, no "free for launch week," no freemium teaser that cuts off after a few chapters.
- [ ] **Primary source.** The link goes to the author's personal/university page, the official book site, or the publisher's own open-access page — never a third-party file host.
- [ ] **Direct enough.** One or two clicks to reach the actual book (a simple, free sign-up form like Szeliski's *Computer Vision* is fine; a paywall or a "request access" form that may be denied is not).
- [ ] **On topic.** Deep Learning, Reinforcement Learning, Probabilistic/Bayesian ML, Classical ML/Statistics, NLP/LLMs, Math for ML, ML Systems, Computer Vision, Generative Models, Causal Inference, Graph Neural Networks, AI Safety/Alignment, or closely related theory.

### Explicitly not allowed

These will get a PR closed, no matter how good the book is:

- Scribd, PDFCoffee, Z-Library, Library Genesis / LibGen, Anna's Archive, Sci-Hub, or any other shadow-library / file-sharing mirror.
- Personal re-uploads to Google Drive, Dropbox, Mega, GitHub Releases, etc. — even if the uploader means well, this repository does not rehost or link to rehosted files.
- "Free" chapters that are really a marketing funnel for a paid book, course, or newsletter.
- Course slides or lecture notes being passed off as a full book (a strong standalone lecture-notes book, like Bertsekas's, is fine — a slide deck is not).
- Books whose free availability is ambiguous or unconfirmed. If you're not sure it's legitimate, open an issue to discuss first instead of a PR.

## How to add a book

1. **Fork** the repository and create a branch, e.g. `add-book-name`.
2. Add a single row to the correct table in `README.md`, keeping **alphabetical order by first author's last name** within that table.
3. Use this row format:

   ```markdown
   | Book Title | Author One, Author Two | Year | [site-name](https://full-url) |
   ```

   - `Year` — publication year, or the year of the most recent update if the book is a living draft. Use `—` if unknown or not applicable.
   - Link text should be the short domain name (e.g. `d2l.ai`), not "click here" or the full URL.
   - If the source requires a quick free sign-up, note that in plain text after the link, e.g. `(free sign-up required)`.

4. If no existing category fits, you may propose a new `##` section — explain why in the PR description.
5. **One book per pull request.** This keeps review fast and makes it easy to merge good additions even if another PR needs discussion.
6. In your PR description, briefly confirm the book meets the checklist above and link to where you verified it's officially free (e.g. the author's own site).

## Reporting a broken or incorrect link

Open an [issue](../../issues/new/choose) with:
- The book title
- The current link
- What's wrong (404, moved, now paywalled, wrong URL, etc.)
- A corrected link if you have one

Our automated link checker (see the badge in the README) also runs on a schedule and will flag dead links, but a human report is always faster.

## Style notes

- Keep table rows on a single line each — don't wrap cell content across lines.
- Match the emoji/heading style already used for section headers.
- Don't reorder or rewrite unrelated parts of the README in the same PR as your addition; keep diffs minimal and focused.
- Write commit messages and PR titles in English, e.g. `Add: "Book Title" to Deep Learning`.

## Code of Conduct

Be respectful and constructive. Disagreements about whether a source qualifies are normal — assume good faith, and when in doubt, open an issue to discuss before investing time in a PR. See [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) for the full guidelines.
