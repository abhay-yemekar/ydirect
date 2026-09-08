# Frequently asked questions

## What is yDirect?

yDirect is a Chrome snippet manager for saving, organizing, searching, copying, exporting, backing up, and selectively sharing reusable text from Chrome's native side panel.

## Is yDirect available now?

Yes. Version `1.3.3` was published on September 8, 2026 through the [official Chrome Web Store listing](https://chromewebstore.google.com/detail/ydirect-snippet-manager-s/ehkahipeoahnbfbahlkedgdcjefejihg).

## Is yDirect free?

Yes. The current `1.3.x` line has no subscriptions, payments, advertising, or paid features.

## What Chrome version is required?

The current package requires Google Chrome `116` or newer.

## Is a yDirect account required?

Yes. Continue with Google or create an email/password account. A verified account is required for protected cloud and workspace operations.

## Is yDirect open source?

No. The extension and backend source are private and proprietary. This public repository contains product documentation and approved showcase media so people can evaluate the product without publishing its implementation.

## Why have a public repository without source code?

It provides a durable place for product documentation, architecture, privacy and permission explanations, roadmap, changelog, issues, media assets, ownership, and portfolio review while protecting implementation and operations.

## Does yDirect read every webpage?

No. The workspace runs in Chrome's native side panel and is not embedded into the website. yDirect does not request a persistent all-sites content script. Temporary `activeTab` and `scripting` access is used only after a user gesture to install or health-check the optional floating shortcut on supported pages.

## Why use Chrome's native side panel?

The side panel is browser-owned and remains separate from a website's DOM, CSS, iframe rules, Trusted Types, and Content Security Policy. It keeps the current page visible while providing a consistent extension surface.

## Does yDirect collect browsing history or page content?

No. Browsing-history and visited-page-content collection are not part of the product.

## Where are snippets stored?

Each account has an account-separated working copy in Chrome local storage. Workspace features also use yDirect's cloud service; optional cloud backup is a separate recovery feature.

## Is masking the same as encryption?

No. Visual masking reduces casual on-screen visibility. It does not encrypt stored content.

## Can I use yDirect as a password or API-key manager?

No. Keep passwords, real API keys, private keys, recovery codes, payment-card data, and other highly sensitive information in a dedicated password or secrets manager. The developer screenshot uses placeholders only.

## What backup formats are available?

yDirect supports JSON, passphrase-encrypted JSON, and Excel import/export. Optional cloud backup keeps the latest successful backup and one previous recovery point.

## Can I share only one folder or snippet?

Yes. The workspace model supports scoped folder and snippet access for verified yDirect accounts. A recipient does not automatically receive the owner's entire personal library.

## What are the workspace roles?

- **Super Admin:** owns and controls the workspace.
- **Core Member:** can organize workspace content and add Members within release limits.
- **Member:** sees explicitly shared resources and may manage only their own contributions inside directly shared folders.

See the [Feature guide](FEATURES.md) for the full role table and sharing behavior.

## How does yDirect handle workspace conflicts?

Workspace saves track edited workspaces independently. Retries recognize already-applied changes; genuine competing revisions remain visible for reconciliation so newer local work is not silently overwritten.

## Does yDirect automatically paste text?

No. The core workflow copies the selected snippet to the clipboard. The user controls where and when to paste it.

## Does yDirect download remote code?

No. Executable extension code is included in the reviewed Store package. Backend requests exchange data, not executable JavaScript or WebAssembly.

## How can I report a bug or request a feature?

Use [GitHub Issues](https://github.com/abhay-yemekar/ydirect/issues) for non-sensitive reports. Follow [SECURITY.md](../SECURITY.md) for vulnerabilities.

## Who owns yDirect?

yDirect is created, owned, and maintained by **Abhay Yemekar**. Contact [abhay.yemekar@ydirect.tech](mailto:abhay.yemekar@ydirect.tech) for owner, partnership, portfolio, or press inquiries. Use [support@ydirect.tech](mailto:support@ydirect.tech) for product support.
