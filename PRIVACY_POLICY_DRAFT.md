# Shikaku Privacy Policy — Pre-publication Draft

**Status: NOT APPROVED FOR PUBLICATION.** This draft is intentionally conservative because the Unity source tree and final SDK inventory were not available during this review. Do not replace the live policy or submit this draft to Google Play until every item in `PRIVACY_REVIEW.md` is verified against the release candidate.

**App:** Shikaku, an Android puzzle game  
**Publisher name currently shown on the existing site:** Tunaroz  
**Effective date:** Set on approval; do not treat this draft date as the effective date.  
**Privacy contact currently shown on the existing site:** tunarozteam@gmail.com — confirm this mailbox is monitored before publication.

## 1. Scope and publisher

This policy describes information handling for the Shikaku mobile game published under the name Tunaroz. The final published version must identify the correct publisher and provide a working privacy contact.

## 2. Information processed by the game and its service providers

The game uses Unity and has an AdMob/Google User Messaging Platform (UMP) integration documented in the project's prior release notes. The precise SDK versions and complete set of enabled services must be verified against the release candidate before publication.

### Gameplay and device-local data

The game maintains gameplay progress and game settings. The final policy must name the exact categories stored locally after checking the save model and persistence code. Do not claim that all progress is exclusively local until cloud backup, platform services, diagnostics, and all network calls have been checked.

### Advertising

The game integrates Google AdMob. Depending on the final SDK configuration, a user's region, device settings, and consent/privacy choices, Google and its advertising partners may process information such as IP address, advertising/device identifiers, app and device information, ad delivery and interaction events, and fraud-prevention signals. Confirm the actual SDK version, mediation adapters, ad formats, and request configuration before publishing this description.

Google resources:
- [Google Privacy Policy](https://policies.google.com/privacy)
- [How Google uses information from apps that use its services](https://support.google.com/admob/answer/6128543)

### Consent and privacy choices

The game has a Google UMP consent flow and a privacy-options control according to the prior implementation record. UMP may present consent or privacy choices where required by the configured message and the user's region. The privacy-options control is separate from this policy and does not replace access to the policy itself. Confirm the live UMP message configuration and behavior before publication.

### Analytics, crash reporting, and other SDKs

**Do not publish this section as a definitive statement until the Unity packages, plugins, Android manifest, and source code have been inspected.** Identify each analytics, crash-reporting, attribution, mediation, platform, or other SDK that is included and enabled. If none are present, state that only after verifying the full project and build dependency graph.

## 3. Purposes of processing

Depending on the verified services included in the released version, information may be processed to operate and save the game, provide advertising and consent choices, measure ad delivery, prevent invalid activity, diagnose errors, maintain security, and respond to support requests. Remove any purpose that is not supported by the actual release build, and add any verified purpose omitted here.

## 4. Sharing and service providers

Google AdMob/UMP is a known service integration. List any other recipients only after verifying the release build and network/service integrations. Service providers may process information under their own privacy terms. Do not claim that information is never shared, sold, or disclosed until the actual SDK terms, configuration, and applicable legal definitions have been reviewed.

## 5. Storage and retention

The game has local gameplay persistence, but the exact stored fields and platform backup behavior must be verified. State which data remains on the device and how it can be removed only after checking save files, PlayerPrefs, caches, backups, and any remote services.

Do not promise a fixed retention period for third-party data unless the relevant provider documentation and configuration substantiate it. Refer users to the applicable provider policies for provider-controlled retention where appropriate.

## 6. Children's privacy and audience

Before publication, confirm the intended audience, age rating, Google Play target audience declaration, and whether child-directed treatment or Families requirements apply. Describe the actual ad and consent configuration for that audience. Do not use a generic statement that the game is not intended for children unless it matches the app's declared audience and distribution.

## 7. Consent and user choices

Users can use the consent/privacy choices surfaced by the configured UMP flow where available. The final policy should explain any additional controls that are actually available in the game or Android settings. Do not promise a universal opt-out or a specific control unless it is present and tested.

## 8. Privacy requests and contact

For privacy questions or requests, contact the publisher using the verified contact details published with this policy.

**Publisher contact to confirm before publication:** tunarozteam@gmail.com (currently displayed on the existing policy page). Confirm that it is monitored and suitable for privacy requests. Do not add a postal address unless the publisher supplies and approves one.

## 9. Security and international processing

Third-party services may process information under their own terms and may process it in countries outside the user's country. The final policy should describe applicable safeguards only where verified. Avoid absolute security guarantees.

## 10. Changes

When the policy changes materially, publish the revised version at the same stable HTTPS URL and update the effective date. Keep the policy consistent with the released app, SDK configuration, and Google Play Data safety declarations.

---

## Publication gate

This is a working draft, not legal advice and not a verified final policy. Before publication:

1. Complete every item in `PRIVACY_REVIEW.md`.
2. Replace this draft with final, source-verified wording and remove internal review notes.
3. Verify the public HTTPS URL loads without authentication and is reachable from a browser.
4. Add the same URL as a distinct action in the in-game Settings UI, preserving the UMP privacy-options action.
5. Reconcile the policy with Google Play's Data safety form and advertising/consent configuration.
