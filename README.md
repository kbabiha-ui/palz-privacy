# Palz Household Organizer — Privacy Policy

The hosted privacy policy for **Palz Household Organizer**
(`com.richi.householdhub`) on Google Play.

Live at <https://kbabiha-ui.github.io/palz-privacy/>

## Why this repo exists

Google Play requires a publicly reachable privacy policy URL before any
release, and it must agree with the Data safety declaration in the Play
Console — a mismatch between the two is a routine rejection.

The app's own repository is private, and GitHub Pages does not serve private
repositories without a paid plan. Rather than make a commercial codebase public
to host one HTML file, the policy lives here on its own.

## Editing it

`index.html` is the whole site — no build step, no dependencies. The source of
truth is `docs/privacy-policy.html` in the app repository; change it there
first, copy it here, and update the "Last updated" date in both.

Keep it describing what the code actually does. The current text claims no
analytics and no ad SDKs because there are none, and describes account deletion
and household succession as they are actually implemented in migrations 0009
and 0006. If any of that changes in the app, this page has to change with it,
or the Data safety declaration stops being true.
