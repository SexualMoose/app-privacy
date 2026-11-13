# App privacy policies

The public privacy-policy pages that the Google Play listings of five Android apps link to.

## Overview / Purpose

Google Play requires every app to have a privacy policy at a public web address. The apps' own repositories
are private, so this repository holds only the policy pages and publishes them with GitHub Pages:

| App | Page |
| --- | --- |
| KeyCourier | https://sexualmoose.github.io/app-privacy/keycourier/ |
| PriceLens | https://sexualmoose.github.io/app-privacy/pricelens/ |
| OpenCube | https://sexualmoose.github.io/app-privacy/opencube/ |
| WallPlanner | https://sexualmoose.github.io/app-privacy/wallplanner/ |
| Projector+ | https://sexualmoose.github.io/app-privacy/projectorplus/ |

## Status

Working. Published 13 November 2026; all six addresses (the index and the five policies) answer.

## Technical Requirements

None to read the pages. To change them: git and a GitHub account with push access. GitHub Pages builds the
site with its own Jekyll; nothing is installed locally.

## Dependencies

- GitHub Pages (Jekyll, run by GitHub). No theme, plugin, script, font or stylesheet from anywhere else: the
  one layout in `_layouts/default.html` carries its styles inline.

## Setup Instructions

```
git clone https://github.com/SexualMoose/app-privacy
```

## Build & Run

There is no local build. A push to `main` makes GitHub Pages rebuild the site within about a minute
(Settings > Pages: deploy from branch `main`, folder `/`). The rebuild also runs when the commit message
contains `[skip ci]`.

## Usage

Each policy's source of truth is `PRIVACY.md` in that app's own repository, and the same text ships inside
the app. To change a policy:

1. Change `PRIVACY.md` in the app's repository (and its "Last updated" date) and ship the app.
2. Copy the text here as `<app>/index.md`, keeping the two-line front matter (`title:`) at the top.
3. Commit, push, and open the page to check it.

## Architecture

- `index.md`: the list of policies.
- `<app>/index.md`: one policy per app, in Markdown.
- `_layouts/default.html`: the only layout (plain HTML, inline styles, a link back to the list).
- `_config.yml`: site title and description; keeps the repository's own documents off the site.

## Integrations & Interconnects

- The five apps' repositories (private): each `PRIVACY.md` is copied here.
- Google Play: each store listing and each app's in-app privacy screen name the page's address.
- GitHub Issues on this repository: the public contact route named in every policy.

## Configuration & Secrets

None. The repository holds no keys, tokens or personal data, and needs none to publish.

## Testing

Open the six addresses after a push and check each returns the expected policy and date.

## Known Issues / TODO

None.

## Third-party & Licensing notes

No third-party content. The text is licensed under PolyForm Strict 1.0.0 (`LICENSE.md`).

## Security notes

Everything here is public by design. Keep it to policy text: no credentials, no personal names or e-mail
addresses, no device or network details. Commits use GitHub's no-reply author address.
