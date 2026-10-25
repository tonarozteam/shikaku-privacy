# Shikaku Privacy Website

This repository hosts the public privacy-policy website for the Shikaku Android puzzle game published by Tunaroz.

## Public pages

- `index.html` — Privacy Policy (the canonical Google Play policy URL).
- `ABOUT.html` — About Shikaku and its publisher.
- `SUPPORT.html` — Contact and support information.
- `app-ads.txt` — Advertising seller declaration; it is not a privacy policy.
- `PRIVACY_REVIEW.md` — Source-inspection requirements and release checklist.
- `PRIVACY_POLICY_DRAFT.md` — Internal pre-publication draft; not a replacement for the live policy.
- `GOOGLE_PLAY_REVIEW.md` — Google Play review checklist.

## Public URLs

- Privacy Policy: https://tonarozteam.github.io/shikaku-privacy/
- About Shikaku: https://tonarozteam.github.io/shikaku-privacy/ABOUT.html
- Contact & Support: https://tonarozteam.github.io/shikaku-privacy/SUPPORT.html

## Important publication gate

The Unity project source tree and exact release build were not available during this repository update. The current `index.html` has therefore **not** been rewritten with unverified claims about SDKs, data flows, consent behavior, local-only storage, or children's audience. The new About and Support pages contain only basic publisher/game information and the existing contact email.

Before finalizing the privacy policy, inspect the release candidate and complete `PRIVACY_REVIEW.md`. Verify the live HTTPS URLs in a browser and reconcile the policy with the Google Play Data safety form.

Keep the in-game Privacy Policy link separate from the Google UMP privacy-options control. Do not change consent gating or build/signing/release configuration as part of website work.
