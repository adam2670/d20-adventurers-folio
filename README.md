# D20 Adventurer's Folio — website

Marketing, support and privacy pages for the iOS app, served by GitHub Pages.

- `index.html` — marketing page (App Store **Marketing URL**)
- `support.html` — support page (App Store **Support URL**)
- `privacy.html` — privacy policy (App Store **Privacy Policy URL**)
- `style.css` — shared styles

Everything is self-contained: no fonts, scripts, images or trackers are fetched
from anywhere, so the pages load instantly and there is nothing to break.

The app itself lives in a separate private repository. This repo is public only
because App Store Connect requires publicly reachable URLs.

## ⚠️ THERE IS A SECOND COPY OF THESE PAGES, AND IT IS NOT THE ONE THAT SERVES

`Adventurers Folio/site/` in the app repo holds the same four files. **This repo
is the one GitHub Pages publishes** — `adam2670.github.io/d20-adventurers-folio`
— and the App Store's Marketing, Support and Privacy URLs all point here.

They were byte-identical until 2026-08-21, when an improvement to the video
embed was made in the app repo's copy and went live nowhere. Neither repo said
the other existed, which is how that happens.

**Edit here. Copy to the app repo's `site/` if you want them level.** And note
the asymmetry that makes this easy to get wrong: the app repo has a
`post-commit` hook that pushes every commit immediately, so a change there
*feels* published and is not. This repo has no such hook — publishing is a
deliberate `git push`, which is correct for a public page and is why nothing
here goes out by accident.
