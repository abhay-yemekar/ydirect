# Installation and first run

## Current availability

yDirect `1.3.3` is published and free on the official [Chrome Web Store listing](https://chromewebstore.google.com/detail/ydirect-snippet-manager-s/ehkahipeoahnbfbahlkedgdcjefejihg). It requires Google Chrome `116` or newer.

This public repository contains documentation and approved media only. It does not distribute source code, an unpacked build, ZIP, or CRX package.

## Install from the Chrome Web Store

1. Open the [official yDirect Chrome Web Store listing](https://chromewebstore.google.com/detail/ydirect-snippet-manager-s/ehkahipeoahnbfbahlkedgdcjefejihg).
2. Select **Add to Chrome**.
3. Review Chrome's permission summary and choose **Add extension**.
4. Open Chrome's Extensions menu and pin yDirect for convenient access.
5. Open a normal `http://` or `https://` page.
6. Click the yDirect toolbar icon or press `Alt+S`.

Only install yDirect from the official Store listing linked here or an official `ydirect.tech` page.

## Create or access an account

1. Continue with Google or register with email and a unique password of at least 12 characters.
2. Accept the Terms and acknowledge the Privacy Policy.
3. Complete email verification when requested.
4. Sign in and create a first folder.
5. Add a snippet with a clear label and reusable value.

A yDirect account is required. Do not reuse a password from another service.

## Open and copy

- `Alt+S`: open yDirect's native side panel.
- Toolbar icon: open or restore the side panel.
- Snippet copy button: copy the selected snippet.
- `Alt+C`: copy the most recently used snippet again.

Chrome lets users review or change extension shortcuts at `chrome://extensions/shortcuts`. A conflicting browser, extension, or operating-system shortcut may need reassignment.

## Native side panel and protected pages

yDirect uses Chrome's browser-owned native side panel. The toolbar, `Alt+S`, and the optional page shortcut open the same surface; the application is not embedded into the current website.

The optional draggable shortcut is available only on supported `http://` and `https://` pages. Chrome restricts page scripting on surfaces such as:

- `chrome://` settings and internal pages;
- the Chrome Web Store;
- some browser-protected or extension-owned pages.

The floating shortcut is absent there by design. Use the toolbar or `Alt+S` wherever Chrome permits an extension side panel.

## First backup

1. Create non-sensitive sample content.
2. Export a JSON backup and confirm the downloaded file exists.
3. If file-level protection is needed, create a passphrase-encrypted JSON export and store the passphrase separately.
4. Enable optional cloud backup only after reviewing its recovery limits.
5. Perform a test restore before relying on a backup workflow.

Cloud backup keeps the latest and one previous successful recovery point. It is not a full archive.

## Troubleshooting

### yDirect does not open

- Confirm the extension is enabled and up to date.
- Try the toolbar icon or `Alt+S`.
- Refresh a normal web page and try again.
- On a Chrome-protected page, remember that the floating shortcut is intentionally unavailable.

### A shortcut does not work

- Open `chrome://extensions/shortcuts` and confirm the shortcut is assigned.
- Resolve conflicts with another extension or operating-system action.
- Use the toolbar icon as a fallback.

### Sign-in or verification email is missing

- Check spam or junk and the exact email address entered.
- Wait briefly before requesting another message.
- Never share a verification or password-reset link with support.

### Export does not appear

- Check Chrome's download indicator and download folder.
- Confirm Chrome did not block the download.
- Retry from yDirect Settings and note the selected format.

### Cloud or shared content looks out of date

- Confirm the account is verified and online.
- Keep the visible panel open briefly so it can refresh.
- Close and reopen the panel if the connection changed.
- Preserve a local export before resolving a genuine workspace conflict.

## Get help

Visit the [yDirect Support Center](https://inksl-ay.firebaseapp.com/support.html) or email [support@ydirect.tech](mailto:support@ydirect.tech?subject=yDirect%20Support%20Request).

Include the yDirect version, Chrome version, operating system, affected surface, and safe reproduction steps. Hide personal and snippet information in screenshots. Never send passwords, codes, reset links, tokens, or sensitive content.
