# Shikaku Privacy Website

This repository hosts the public privacy-policy website for the Shikaku Android puzzle game published by Tunaroz.

## Public page

- `index.html` — the Privacy Policy and canonical external policy URL for Google Play.
- `app-ads.txt` — advertising seller declaration; it is not a privacy policy.
- `PRIVACY_REVIEW.md` — source-inspection requirements and release checklist.
- `PRIVACY_POLICY_DRAFT.md` — internal pre-publication draft; not a replacement for the live policy.
- `GOOGLE_PLAY_REVIEW.md` — Google Play review checklist.

## Public URL

- Privacy Policy: https://tonarozteam.github.io/shikaku-privacy/

## In-game UI requirement

The **About Us** and **Contact & Support** screens must be implemented inside the Unity game, not as external webpages. The **Privacy Policy** is the only item in this section that should open an external URL.

Recommended in-game section:
- **About Us** — show a short description of Shikaku and publisher Tunaroz in an in-app screen.
- **Contact & Support** — show `tunarozteam@gmail.com` in an in-app screen, with a button to compose an email using a `mailto:` link. The screen itself must remain in-game; opening an email app is an explicit user action.
- **Privacy Policy** — open the public HTTPS URL above.
- **Privacy Choices** — if required/supported, use the existing Google UMP privacy-options API. Keep this distinct from the policy link.

## Important publication gate

The Unity project source tree and exact release build were not available during this repository update. The live policy therefore must still be reconciled with the actual SDK inventory, data flows, consent behavior, local storage, target audience, and Google Play Data safety declarations. Do not claim full compliance until this verification is complete.

Do not change consent gating or build/signing/release configuration as part of website work.
