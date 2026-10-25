# Shikaku — Google Play Privacy Review Checklist

**Repository:** `tonarozteam/shikaku-privacy`  
**Publisher stated on the current policy:** Tunaroz  
**Policy URL:** https://tonarozteam.github.io/shikaku-privacy/  
**Support:** tunarozteam@gmail.com

This document is a working checklist, not a legal opinion or a claim that the app has passed Google Play review. The Unity project and the exact release build must be audited before final declarations are made.

## Public page in this repository

- Privacy Policy: `index.html`
- Public URL: https://tonarozteam.github.io/shikaku-privacy/

**About Us** and **Contact & Support** must be in-app Unity screens, not external website pages. Only the Privacy Policy item should open the external policy URL. The Contact & Support screen may offer an explicit button to open the user's email application via `mailto:tunarozteam@gmail.com`.

## Required app and SDK audit

Before finalizing the policy or Data safety declaration, inspect the exact project and release configuration. Confirm each service is installed, initialized, enabled, and used; do not infer data collection solely from a dependency being present.

- [ ] List all Unity packages, Android libraries, plugins, and SDK versions.
- [ ] Inspect Android manifest permissions and merged manifest.
- [ ] Confirm Google Mobile Ads / AdMob SDK configuration and each ad format used.
- [ ] Confirm UMP consent information update, consent form flow, consent gating, and privacy-options requirements.
- [ ] Verify which advertising identifiers and device/network signals may be processed by the configured SDK.
- [ ] Confirm whether Firebase Analytics, Crashlytics, Unity Analytics/diagnostics, attribution, or any other telemetry service is actually used.
- [ ] Identify any backend, account, cloud sync, external API, or other data transmission.
- [ ] Document local-only save data and how clearing app data or uninstalling affects it.
- [ ] Verify the app's target audience, age rating, and applicable Families requirements.
- [ ] Confirm contact details and publisher identity are accurate.
- [ ] Compare the final policy with the exact production build and Google Play Console Data safety answers.

## Google Play Console checks

- [ ] Set the Privacy Policy URL to the public policy URL above.
- [ ] Ensure the policy is accessible without login, is not a PDF-only document, and is not blocked by region or robots configuration.
- [ ] Make the policy accessible from inside the app.
- [ ] Complete the Data safety form for the app and every relevant third-party SDK.
- [ ] Ensure declared data collection, sharing, purposes, and security practices match verified behavior.
- [ ] Verify target audience, Families declarations, and ad configuration where applicable.
- [ ] If users can create accounts in any version, review Google Play account-deletion requirements. Do not declare account deletion as applicable or available without verifying the account feature.
- [ ] Recheck all public links after deployment.

## Important implementation note

The public Privacy Policy describes expected behavior at a general level. Statements about optional analytics, diagnostics, third-party processing, consent, and retention must be tightened or removed after the audit. This checklist itself does not establish that any particular SDK is present or that the app is compliant.

## Official references

- Google Play User Data policy: https://support.google.com/googleplay/android-developer/answer/10144311
- Google Play Data safety section: https://support.google.com/googleplay/android-developer/answer/10787469
- Google Play Families policy requirements: https://support.google.com/googleplay/android-developer/answer/9893335
- Google privacy policy: https://policies.google.com/privacy
- Google Mobile Ads and app data disclosure guidance: https://support.google.com/admob/answer/6128543
- Unity Privacy Policy: https://unity.com/legal/privacy-policy
