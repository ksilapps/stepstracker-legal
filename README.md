# Steps: Daily Walk Tracker — legal & support

A small, dependency-free website for the iPhone app. GitHub Pages serves the HTML and shared CSS directly; no build step is required.

- `index.html`: privacy and support directory
- `privacy-policy.html`: permissions, local storage, iCloud app-state boundaries, purchases, notifications, deletion, and hosting
- `terms-of-use.html`: free/Pro access, one-time purchase and restore terms, sync, reminders, and measurement limitations
- `support.html`: common questions using native HTML disclosures
- `styles.css`: responsive layout, keyboard focus, reduced motion, and print styles
- `steps-icon.png`: supplied app artwork used in the header, home page, and browser icon

Keep the existing HTML filenames: the app links directly to them from Settings.

## Content maintenance

Content was checked against `../steps_tracker` on October 11, 2026, including Health and Motion access, finalized local history, Goal/Recovery plans, local notifications, Steps Pro, RevenueCat, the CloudKit schema, reset behavior, and Settings links. Update the privacy policy when data practices change, and revise the effective/update dates when appropriate.

The support contact is `ksil.apps@gmail.com`, as supplied by the developer.

Hosting disclosure references GitHub Pages documentation: https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages#data-collection

## Review

Serve this folder with any static HTTP server. Check all four pages at desktop and narrow mobile widths, keyboard navigation, policy section links, and support disclosures. No third-party fonts, scripts, analytics, or cookies are added by this site.

## Verified data boundaries

CloudKit sync includes selected settings, effective-dated goals/plans, badge IDs/unlock dates, and finalized day policy. It excludes activity measurements, completion results, height/weight, permission state, onboarding, and notification preferences. Reset Local Data does not delete the private cloud database or purchase records. Preserve these distinctions in future copy.

Code references: `../steps_tracker/src/cloud/schema.ts`, `src/cloud/localRepository.ts`, `src/storage/preferences.ts`, `src/purchases/revenueCat.ts`, `app/paywall.tsx`, `app/settings.tsx`, and `modules/steps-pedometer/ios/StepsNotificationsModule.swift`. App docs can lag implementation; verify against code.

Provider references checked October 11, 2026:

- RevenueCat purchase-data disclosures: https://www.revenuecat.com/docs/platform-resources/apple-platform-resources/apple-app-privacy
- RevenueCat privacy and end-user processing information: https://www.revenuecat.com/privacy
- Apple refund guidance: https://support.apple.com/en-us/118223

These pages describe implemented behavior. Store product setup, native/device purchase and sync validation, and App Store privacy disclosures remain separate release checks.
