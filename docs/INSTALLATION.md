# Installation and first run

## Current availability

yDirect `1.3.1` is available from the official [Chrome Web Store listing](https://chromewebstore.google.com/detail/ydirect-%E2%80%94-smart-snippet-m/ehkahipeoahnbfbahlkedgdcjefejihg). Version `1.3.2` is release-ready for that same listing and will become available only after Store submission, review, and publishing.

The public repository does not contain source code or an installable extension package.

## Install from the Chrome Web Store

To install the published version:

1. Open the [official yDirect Chrome Web Store listing](https://chromewebstore.google.com/detail/ydirect-%E2%80%94-smart-snippet-m/ehkahipeoahnbfbahlkedgdcjefejihg).
2. Select **Add to Chrome**.
3. Review Chrome's permission summary and choose **Add extension**.
4. Open Chrome's Extensions menu and pin yDirect for convenient access.
5. Open a normal `http://` or `https://` page.
6. Click the yDirect toolbar icon or press `Alt+S`.

Only install yDirect from the official listing linked by this repository or an official `ydirect.tech` page.

## Create or access an account

1. Register with an email address and a unique password of at least 12 characters, or choose Google sign-in.
2. Accept the Terms and acknowledge the Privacy Policy.
3. Complete email verification when requested.
4. Sign in and create a first folder.
5. Add a snippet with a clear label and reusable value.

Do not reuse a password from another service.

## Open and copy

- `Alt+S`: open yDirect from a supported page.
- Toolbar icon: open or restore the native side panel.
- Snippet copy button: copy the selected snippet.
- `Alt+C`: copy the most recently used snippet.

Chrome may allow users to change extension shortcuts at `chrome://extensions/shortcuts`.

## Native side panel and restricted pages

Version `1.3.2` uses Chrome's native side panel for the yDirect workspace. The toolbar, `Alt+S`, and the optional page shortcut open the same browser-owned surface. The application is not embedded into the current website.

The optional floating shortcut is available only on supported `http://` and `https://` pages. Chrome restricts page scripting on surfaces such as:

- `chrome://` settings and internal pages;
- the Chrome Web Store;
- some browser-protected or extension-owned pages.

On those pages the floating shortcut is absent by design. Use the toolbar or `Alt+S` wherever Chrome permits an extension side panel.

## First backup

1. Create non-sensitive sample content.
2. Export a JSON backup and confirm the downloaded file exists.
3. If file-level protection is needed, create a passphrase-encrypted JSON export and store the passphrase separately.
4. Enable optional cloud backup only after reviewing its recovery limits.
5. Perform a test restore before relying on any backup workflow.

Cloud backup keeps the latest and one previous successful recovery point. It is not a full archive.

## Troubleshooting

### yDirect does not open

- Confirm the page uses `http://` or `https://`.
- Try the toolbar icon or `Alt+S` instead of a remembered extension URL.
- Refresh the page and open yDirect again.
- On a Chrome-protected page, remember that the floating shortcut is intentionally unavailable.
- Check that the extension is enabled and up to date.

### Shortcut does not work

- Open `chrome://extensions/shortcuts` and confirm the shortcut is assigned.
- Resolve any shortcut conflict with another extension or operating-system action.
- Use the toolbar icon as a fallback.

### Sign-in or verification email is missing

- Check spam/junk folders and the exact email address entered.
- Wait briefly before requesting another message.
- Never share a verification link with support.

### Export does not appear

- Check Chrome's download indicator and download folder.
- Confirm Chrome did not block the download.
- Retry from yDirect settings and record the format selected.

## Get help

Visit the [yDirect Support Center](https://inksl-ay.firebaseapp.com/support.html) or email [support@ydirect.tech](mailto:support@ydirect.tech?subject=yDirect%20Support%20Request).

Include the yDirect version, Chrome version, operating system, affected surface (popup, native side panel, toolbar, floating shortcut, or hosted account page), and steps to reproduce. Hide personal and snippet information in screenshots. Never send passwords, codes, reset links, or sensitive content.
