# Privacy and Chrome permissions

This page is a plain-language product explanation, not a replacement for the [Privacy Policy](https://inksl-ay.firebaseapp.com/privacy.html) or [Terms of Service](https://inksl-ay.firebaseapp.com/terms.html).

## Privacy model

yDirect is local-first for ordinary snippet work and uses cloud services only for account, optional backup, workspace/sharing, feedback, and related product operations.

The extension does not sell user data, use it for personalized advertising, collect browsing history, or request persistent permission to read every website.

The yDirect workspace runs in Chrome's native side panel and opens only after the user clicks yDirect, invokes `Alt+S`, or uses the optional page shortcut.

## Data categories used by product features

Depending on the features a user chooses, yDirect may handle:

| Category | Examples | Purpose |
| --- | --- | --- |
| Account identity | Email address, display name, sign-in provider, optional Google profile photo URL | Authentication, account display, verified sharing |
| Authentication information | Firebase user/session identifiers and sign-in tokens | Secure authenticated requests |
| User-provided content | Folder names, snippet labels/text, exports, backup content, contributions, feedback | Core snippet, recovery, sharing, and support functionality |
| Product state | Settings, copy counts, timestamps, roles, grants, backup status, extension version | Organize the library, enforce permissions, and operate features |
| Security/operational records | Limited error, rate-limit, queue, and delivery records | Reliability, abuse prevention, account operations, and support |

Do not store passwords, one-time codes, private keys, recovery codes, payment-card data, or other high-risk secrets as ordinary snippets.

## Chrome permissions

| Permission | Why yDirect needs it | What it does not mean |
| --- | --- | --- |
| `storage` | Stores folders, snippets, account-local cache, theme, backup schedule/status, and settings in Chrome | It does not grant access to unrelated files on the device |
| `downloads` | Saves a file after the user selects Export JSON, Encrypted JSON, or Export Excel | yDirect does not read, monitor, open, or modify existing downloads |
| `clipboardWrite` | Copies a selected snippet or the last-used snippet after the user invokes the action | It does not read clipboard history |
| `activeTab` | Temporarily grants access to the active tab after a yDirect toolbar click or shortcut | It is not permanent access to every website |
| `scripting` | Installs or health-checks only the optional draggable shortcut on the user-activated HTTP/HTTPS tab | The application itself uses the native side panel; there is no persistent all-sites content script |
| `sidePanel` | Opens the responsive yDirect workspace in Chrome's browser-owned side panel after a user action | It does not expose the snippet library to the active website |
| `offscreen` | Supports the user-initiated Google account chooser required by the Manifest V3 authentication flow | yDirect does not request Chrome's `identity` permission |
| `alarms` | Schedules optional automatic cloud backups at the frequency selected by the user | Automatic backup defaults to off |
| yDirect Functions origin | Sends authenticated account, workspace, sharing, feedback, and backup requests to the product backend | It is not general access to arbitrary internet hosts |

## Local, cloud, and shared data

### Local

Chrome local storage contains the working snippet library and relevant settings for the signed-in local profile.

### Optional cloud backup

An authenticated backup contains the content needed to restore the library. The service keeps the latest successful backup and one previous recovery point. Automatic backup is off by default.

### Workspaces

Cloud workspace data and grants make selected resources available to authorized verified accounts. Recipients do not automatically receive the owner's entire personal library.

## Import and export

- JSON is intended for a restorable yDirect backup.
- Passphrase-encrypted JSON provides file-level encryption controlled by the passphrase chosen by the user.
- Excel is intended for readable review and portability.
- Export begins only after the user selects the corresponding action.

Keep passphrases outside the exported file. Losing the passphrase can make an encrypted export unrecoverable.

## Remote code

The Chrome extension package executes code included in the reviewed package. It does not download executable JavaScript or WebAssembly from the backend. Network requests exchange data with the yDirect service.

## Account controls

Users can export content, clear browser-local data, leave shared access where available, and request account deletion from yDirect settings. Some security-sensitive actions may require a recent sign-in.

## Contacts

- Privacy or data request: [support@ydirect.tech](mailto:support@ydirect.tech?subject=yDirect%20Privacy%20Request)
- Product owner: [abhay.yemekar@ydirect.tech](mailto:abhay.yemekar@ydirect.tech)
- Security report: follow [SECURITY.md](../SECURITY.md)

Never email passwords, authentication links, one-time codes, private keys, or sensitive snippet content.
