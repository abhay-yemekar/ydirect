# Changelog

This public changelog summarizes user-visible product milestones. It does not expose private implementation details or replace the release history in the private source repository.

## 1.3.2 — release-ready August 21, 2026

Compatibility and reliability update prepared for the existing Chrome Web Store listing. Version `1.3.1` remains the published version until `1.3.2` completes Store submission, review, and publishing.

### Highlights

- Replaced the website-embedded workspace with Chrome's native side panel.
- Unified toolbar, `Alt+S`, and the optional draggable page shortcut on the same browser-owned surface.
- Removed the site-specific iframe dependency that could be blocked by restrictive website policies.
- Added a Manifest V3-compatible Google account chooser without requesting Chrome's `identity` permission.
- Improved Google sign-in diagnostics and hosted-helper security controls.
- Improved the accuracy and reliability of verification, account, invitation, sharing, and support email status.

## 1.3.1 — published August 12, 2026

Maintenance release published through the permanent Chrome Web Store listing.

### Highlights

- Made JSON, encrypted JSON, and Excel downloads more reliable through Chrome's native download flow.
- Preserved the on-demand active-tab access model for the attached workspace.
- Added feedback submission and support-mail delivery.
- Added workspace invitations and notifications for newly shared folders and snippets.
- Completed final Store identity and OAuth binding for the permanent extension ID.
- Refined release documentation and policy disclosures for the download permission.
- Revalidated automated data, workspace, UI, lifecycle, permission, and policy checks.

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

The Chrome Web Store publication status shown in this repository is updated manually. Refer to the project README for the current public status.
