# Steps: Walking Tracker — legal & support

A small, dependency-free website for the iPhone app. GitHub Pages serves the HTML and shared CSS directly; no build step is required.

- `index.html`: privacy and support directory
- `privacy-policy.html`: permissions, local storage, deletion, and website hosting
- `terms-of-use.html`: app usage and measurement limitations
- `support.html`: common questions using native HTML disclosures
- `styles.css`: responsive layout, keyboard focus, reduced motion, and print styles
- `steps-icon.png`: supplied app artwork used in the header, home page, and browser icon

Keep the existing HTML filenames: the app links directly to them from Settings.

## Content maintenance

Content was checked against `../steps_tracker` on October 5, 2026, including app permissions, Health access, local storage, reset behavior, and Settings links. Update the privacy policy when data practices change, and revise the effective/update dates when appropriate.

The support contact is `ksil.apps@gmail.com`, as supplied by the developer.

Hosting disclosure references GitHub Pages documentation: https://docs.github.com/en/pages/getting-started-with-github-pages/what-is-github-pages#data-collection

## Review

Serve this folder with any static HTTP server. Check all four pages at desktop and narrow mobile widths, keyboard navigation, policy section links, and support disclosures. No third-party fonts, scripts, analytics, or cookies are added by this site.
