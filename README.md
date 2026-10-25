# Shikaku Privacy Website

This repository hosts the public privacy-policy site for the Shikaku Android puzzle game.

## Files

- `index.html` — current website page. Do not update its published privacy statements until they have been checked against the exact Unity release candidate.
- `app-ads.txt` — advertising seller declaration; this is not a privacy policy.
- `PRIVACY_POLICY_DRAFT.md` — internal, pre-publication draft. It is **not approved for publication**.
- `PRIVACY_REVIEW.md` — source-inspection requirements, known limitations, and release checklist.

## Publication gate

The Unity source tree was not available during the latest review, so the exact SDK inventory, data flows, save behavior, and Settings UI could not be verified. The current site has therefore not been changed. Before updating the live page, inspect the release candidate, complete the checklist in `PRIVACY_REVIEW.md`, verify the public HTTPS URL in a browser, and reconcile the final policy with the Google Play Data safety form.

Keep the in-game Privacy Policy link separate from the Google UMP privacy-options control. Do not change consent gating or build/signing/release configuration as part of this work.
