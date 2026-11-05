# Palz Household Organizer — Privacy Policy and Terms

The hosted privacy policy and terms of service for **Palz Household Organizer**
(`com.richi.householdhub`) on Google Play.

- Privacy policy — <https://kbabiha-ui.github.io/palz-privacy/>
- Terms of service — <https://kbabiha-ui.github.io/palz-privacy/terms-of-service.html>

## Why this repo exists

Google Play requires a publicly reachable privacy policy URL before any
release, and it must agree with the Data safety declaration in the Play
Console — a mismatch between the two is a routine rejection.

A terms of service URL is required alongside the trader status declaration,
which a personal developer account selling subscriptions has to make.

The app's own repository is private, and GitHub Pages does not serve private
repositories without a paid plan. Rather than make a commercial codebase public
to host one HTML file, the policy lives here on its own.

## Editing it

`index.html` and `terms-of-service.html` are the whole site — no build step,
no dependencies. The source of truth for both is `docs/` in the app repository
(`privacy-policy.html` and `terms-of-service.html`); change them there first,
copy them here, and update the "Last updated" date in both copies.

Keep it describing what the code actually does. The current text claims no
analytics and no ad SDKs because there are none, and describes account deletion
and household succession as they are actually implemented in migrations 0009
and 0006. If any of that changes in the app, this page has to change with it,
or the Data safety declaration stops being true.

The policy says photos, videos and audio **are** collected. That is not an
oversight: `getDocumentAsync` in `src/hooks/useDocuments.ts` is called with no
`type` option, so the picker accepts any file and the app stores whatever the
user hands it. Do not narrow that claim here without adding a `type` filter to
the picker first.
