# Changelog

This public changelog summarizes user-visible product milestones. It does not expose private implementation details or replace the release history in the private source repository.

## 1.3.3 — published September 8, 2026

Reliability, clarity, and Store-presentation update published through yDirect's permanent Chrome Web Store listing.

### Highlights

- Improved returning-user startup while revalidating cached account consent in the background.
- Fixed delayed Firebase authentication loading in the Manifest V3 service worker, including automatic-backup wake-up paths.
- Made workspace saves and retries conflict-safe while preserving genuine conflicts for reconciliation.
- Waited for sharing confirmation before closing and refreshed shared content in visible panels.
- Made Profile, About, Feedback, and Settings panels more compact.
- Clarified sign-in-method status, made the sign-in email read-only, corrected account/settings icons, and removed decorative bounce effects.
- Refined the Store title and summary around saving, searching, and copying reusable text.
- Published a new five-image Store gallery and refreshed public demo media.
- Added no new Chrome permissions.

## 1.3.2 — published August 2026

Compatibility and reliability update published to the existing Chrome Web Store listing.

### Highlights

- Replaced the website-embedded workspace with Chrome's native side panel.
- Unified toolbar, `Alt+S`, and the optional draggable page shortcut on the same browser-owned surface.
- Removed the site-specific iframe dependency that could be blocked by restrictive website policies.
- Added a Manifest V3-compatible Google account chooser without requesting Chrome's `identity` permission.
- Improved Google sign-in diagnostics and hosted-helper security controls.
- Improved verification, account, invitation, sharing, and support-email status handling.

## 1.3.1 — published August 12, 2026

Maintenance release published through the permanent Chrome Web Store listing.

### Highlights

- Made JSON, encrypted JSON, and Excel downloads more reliable through Chrome's native download flow.
- Preserved the on-demand active-tab access model for the workspace.
- Added feedback submission and support-mail delivery.
- Added workspace invitations and notifications for newly shared folders and snippets.
- Completed Store identity and OAuth binding for the permanent extension ID.
- Refined release documentation and permission-policy disclosures.

## 1.3.0 — first release candidate

### Highlights

- Introduced the yDirect smart snippet workspace for Chrome.
- Added folder and list views, search, sorting, one-click copy, and copy-last shortcut.
- Added local account-separated storage, optional masking, and light/dark themes.
- Added JSON, encrypted JSON, and Excel import/export.
- Added optional cloud backup with two recovery points.
- Added verified-account workspaces, scoped folder/snippet sharing, and member contributions.
- Added account, support, privacy, terms, uninstall, and changelog web pages.

## Status note

Chrome Web Store publication status in this repository is maintained manually. The [project README](README.md) records the current public version.
