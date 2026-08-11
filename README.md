# Food Tracker — Legal documents

Public legal documents for the [Food Tracker](https://github.com/Shred0/FoodTracker) app, served via GitHub Pages.

- [Privacy Policy](https://legal.shreddedonion.com/privacy-policy.html) (English)

Served by GitHub Pages from this repo through the custom domain in `CNAME`
(`legal.shreddedonion.com`). **Always publish the app pointing at the custom domain, never at
`shred0.github.io`**: the URL is compiled into every released build, so an installation that is
never updated keeps requesting the address it shipped with. We control the DNS of the custom
domain and can move the hosting anywhere; a `*.github.io` hostname cannot be redirected by us at
all, and a freed GitHub username can be taken over by someone else.

The app links to these pages from its About page and first-run legal notice
(`LegalConstants.PrivacyPolicyUrl` in the app repo). When a document changes materially,
bump `LegalConstants.LegalNoticeVersion` in the app so users are asked to acknowledge it again.

The policy must also stay consistent with the **Data safety** form in the Play Console: a
mismatch between the two is a common rejection reason, so update both together.

## History

| Notice version | Date | Change |
|---|---|---|
| 1 | 15 Jul 2026 | First version: local-only storage, AdMob, Open Food Facts, Frankfurter. |
| 2 | 11 Aug 2026 | Added every route by which data can now leave the device — AI photo scanning with your own API key, backups (picked folder / Google Drive appDataFolder / iCloud), sharing plans and progress reports with a nutritionist, and Health Connect / Apple Health. Corrected the previous claim that data was never transmitted to any server, which had ceased to be true. Stated explicitly that health data never reaches the advertising SDK, and that the app contains no analytics, telemetry or crash reporting. |
