# Installation and first run

## Current availability

yDirect `1.3.1` was submitted to the Chrome Web Store on August 11, 2026. Review is pending and automatic publishing is disabled, so the owner will complete a final check before the public listing goes live.

The public repository does not contain source code or an installable extension package.

## Install from the Chrome Web Store

After the listing is published:

1. Open the official yDirect Chrome Web Store listing linked from the project README.
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
- Toolbar icon: open or restore the attached workspace.
- Snippet copy button: copy the selected snippet.
- `Alt+C`: copy the most recently used snippet.

Chrome may allow users to change extension shortcuts at `chrome://extensions/shortcuts`.

## Supported and restricted pages

The attached right-edge workspace works on normal `http://` and `https://` pages where Chrome permits extension injection.

Chrome restricts extension injection on pages such as:

- `chrome://` settings and internal pages;
- the Chrome Web Store;
- some browser-protected or extension-owned pages.

On a restricted page, yDirect may open its standalone extension page instead of attaching to the current tab.

## First backup

1. Create non-sensitive sample content.
2. Export a JSON backup and confirm the downloaded file exists.
3. If file-level protection is needed, create a passphrase-encrypted JSON export and store the passphrase separately.
4. Enable optional cloud backup only after reviewing its recovery limits.
5. Perform a test restore before relying on any backup workflow.

Cloud backup keeps the latest and one previous successful recovery point. It is not a full archive.

## Troubleshooting

### yDirect does not attach to the current page

- Confirm the page uses `http://` or `https://`.
- Try the toolbar icon instead of a remembered extension URL.
- Refresh the page and open yDirect again.
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

Include the yDirect version, Chrome version, operating system, affected surface (popup or attached workspace), and steps to reproduce. Hide personal and snippet information in screenshots. Never send passwords, codes, reset links, or sensitive content.
