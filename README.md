# DAX Interactive website

The website for DAX Interactive, published with GitHub Pages at https://daxinteractive.com (custom domain set in `CNAME`; the GitHub address is maxhakin.github.io).

Plain HTML and one stylesheet (`style.css`); no build step.

## Two audiences

The site serves two separate audiences, and the two halves are kept apart on purpose:

- **Players (public):** the home page, the game pages and their privacy policies. Linked together, indexed by search engines, styled with `style.css`.
- **Clients (private portfolio):** everything under `portfolio/`. A pitch to potential clients, with its own styling. It is not linked from the public pages and is marked `noindex`, so people only reach it from a link shared with them directly. Keep it that way: don't link to it from the public pages.

## Contact emails

| Address | Use | Where it appears |
|---|---|---|
| `support@daxinteractive.com` | Player support and privacy questions | Both privacy policies (`quiltz/privacy/`, `stepquest/privacy/`) |
| `hello@daxinteractive.com` | Client project enquiries (links pre-fill the subject "Project enquiry") | Portfolio pages (`portfolio/`, `portfolio/quiltz/`) |

Don't mix them up: player-facing pages use `support@`, client-facing pages use `hello@`.

## Pages

Public:

- `index.html`: home (extra styles in `home.css`)
- `stepquest/index.html`: about StepQuest
- `stepquest/privacy/index.html`: StepQuest's privacy policy (its address is given to App Store Connect, so don't move it)
- `quiltz/index.html`: about Quiltz (screenshots in `quiltz/images/`)
- `quiltz/privacy/index.html`: Quiltz's privacy policy (its address goes in the game's Settings and App Store Connect, so don't move it). The source draft lives in the game's repo at `PocketPatterns/docs/privacy_policy.md`; keep the two in step.
- `legacy/index.html`: about Legacy

Client portfolio (unlinked, `noindex`):

- `portfolio/index.html`: client portfolio home (own style in `portfolio/portfolio.css`)
- `portfolio/quiltz/index.html`: Quiltz case study (Quiltz styles plus `portfolio/quiltz/case.css`, screenshots in `portfolio/quiltz/images/`)
