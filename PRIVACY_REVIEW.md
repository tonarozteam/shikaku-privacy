# Shikaku Privacy Review — Release Blocker #1

## Current repository findings

- Existing site repository: `tonarozteam/shikaku-privacy`
- Existing policy page source: `index.html` (currently contains a broad policy and a pre-existing contact email)
- Advertising declaration: `app-ads.txt`
- Repository documentation: `README.md`
- GitHub Pages is enabled in repository metadata.
- Candidate public URL: `https://tonarozteam.github.io/shikaku-privacy/`
- URL status: **not verified as publicly reachable in this review**; the web fetch tool could not access it. Do not claim publication or Google Play compliance from repository settings alone.

## Scope limitation

The Unity project source tree was not available through the current conversation's project files or the connected GitHub repositories. Prior project notes describe AdMob + UMP gating, an in-game UMP privacy-options control, interstitial ads after qualifying level completions, and rewarded ads granting 1 hint or 100 coins only after the reward callback. Those notes are useful leads but do not establish the current source/build behavior. No source-code or UI change can safely be made without the current Unity project.

## Existing policy statements that require verification

The existing `index.html` currently makes broad statements about local gameplay progress, possible advertising/diagnostic data, Unity and other service providers, support correspondence retention, children's privacy, and data rights. Several statements are generic and should not be treated as verified facts until matched to the release candidate.

## Required source inspection

- [ ] `Packages/manifest.json` and lock file: all packages, SDKs, mediation adapters, analytics and crash reporting.
- [ ] `Assets/Plugins/Android`, AARs, `Assets/ExternalDependencyManager`, Gradle templates if present, and generated dependency declarations: transitive Android SDKs.
- [ ] `Assets/GoogleMobileAds` and AdMob settings: SDK version, app ID, ad unit IDs, mediation, ad formats.
- [ ] UMP/consent implementation: consent-information update, form presentation, `CanRequestAds()` gating, privacy-options entry point, debug geography/test devices, configured messages.
- [ ] Android manifest and Unity Player settings: permissions, advertising ID permission, backup flags, target audience-related configuration.
- [ ] Search source for network requests, analytics, telemetry, crash reporting, attribution, identifiers, and third-party endpoints.
- [ ] Save implementation: PlayerPrefs, files, save fields, backup/cloud behavior, deletion behavior.
- [ ] Settings UI: identify the existing UMP privacy-options action and add a separate policy link using established UI conventions.
- [ ] Tests: add a focused test or validation that the policy URL is non-empty HTTPS and the policy action remains distinct from the UMP privacy-options action. Add UI behavior coverage if the current test setup supports it.

## Publisher confirmations needed

- [ ] Confirm publisher/legal entity name to display (existing site says “Tunaroz”).
- [ ] Confirm `tunarozteam@gmail.com` is monitored and approved for privacy requests.
- [ ] Supply an address only if required for the publisher's legal obligations and if it should be publicly disclosed; none should be invented.
- [ ] Confirm intended audience and whether children are a target audience.
- [ ] Confirm supported distribution regions and the legal entity/jurisdiction relevant to privacy requests.
- [ ] Confirm final Google Play Data safety answers against verified SDK behavior.

## Minimal implementation plan

1. Keep the existing website and update `index.html` only after source verification; use the existing GitHub Pages URL if its public reachability is verified.
2. Keep `app-ads.txt` separate from the privacy policy.
3. Add a distinct “Privacy Policy” action in the existing Unity Settings UI that opens the verified HTTPS URL. Preserve the current UMP privacy-options control and all consent gating.
4. Add a focused test/documentation update; do not change unrelated gameplay, ads, signing, package identity, or release configuration.
5. Verify the live policy URL and reconcile it with Google Play Data safety before claiming compliance.

## Actions deliberately not performed

- No APK/AAB build.
- No Gradle invocation.
- No Android signing, package identity, or release configuration changes.
- No update to the currently published `index.html`, because the Unity SDK inventory and actual data flows could not be verified.
