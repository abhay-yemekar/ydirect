# Frequently asked questions

## What is yDirect?

yDirect is a Chrome snippet manager for saving, organizing, searching, copying, backing up, exporting, and selectively sharing reusable text.

## Is yDirect free?

Yes. The current `1.3.x` release line has no subscriptions, payments, advertising, or paid features.

## Is yDirect open source?

No. The extension and backend source code are private and proprietary. This public repository contains product documentation and approved showcase media so the product can be evaluated without publishing its implementation.

## Why have a public GitHub repository without source code?

It provides a durable, transparent place for product documentation, architecture, privacy and permission explanations, roadmap, changelog, issue reporting, media assets, and ownership information. It also gives recruiters and collaborators a reviewable project record while protecting private implementation and operational material.

## When can I install it?

Version `1.3.1` is available now from the [official Chrome Web Store listing](https://chromewebstore.google.com/detail/ydirect-%E2%80%94-smart-snippet-m/ehkahipeoahnbfbahlkedgdcjefejihg). Version `1.3.2` is release-ready and will update the same listing after Store submission and review.

## Does yDirect read every webpage?

No. The workspace runs in Chrome's native side panel and is not embedded into the website. The extension does not request a persistent all-sites content script. Temporary `activeTab` and `scripting` access is used only after a user gesture to install or health-check the optional floating shortcut on supported pages.

## Why did version 1.3.2 move to Chrome's native side panel?

The native side panel is browser-owned and is not subject to a website's iframe, CSS, Trusted Types, or Content Security Policy rules. This gives yDirect a consistent surface across ordinary and restrictive websites while keeping the current page visible.

## Does yDirect collect browsing history?

No. Browsing-history collection is not part of the product.

## Where are snippets stored?

The working library is local-first in Chrome storage and separated by signed-in account. Authenticated cloud services are used for optional backup, workspaces/sharing, feedback, and account operations.

## Is masking the same as encryption?

No. Masking reduces casual visibility on screen. It does not encrypt stored content.

## Can I use yDirect as a password manager?

No. Do not store passwords, private keys, recovery codes, payment-card data, or other highly sensitive information as ordinary snippets.

## What backup formats are available?

yDirect supports JSON, passphrase-encrypted JSON, and Excel import/export. Optional cloud backup keeps the latest successful backup and one previous recovery point.

## Can I share only one folder or snippet?

Yes. The workspace model supports scoped folder and snippet access for verified yDirect accounts. Recipients do not automatically receive the owner's entire personal library.

## What is the difference between Super Admin, Core Member, and Member?

- A Super Admin owns and controls the workspace.
- A Core Member can organize workspace content and add Members, within release limits.
- A Member sees explicitly shared resources and may manage only their own contributions inside directly shared folders.

See [Features](FEATURES.md) for the full role table.

## Does yDirect automatically paste text?

The current core workflow copies the selected snippet to the clipboard. The user remains in control of where and when it is pasted.

## Does yDirect download remote code?

No. The extension package executes code included in the reviewed package. Backend requests exchange data, not executable JavaScript or WebAssembly.

## How can I report a bug or request a feature?

Use [GitHub Issues](https://github.com/abhay-yemekar/ydirect/issues) for non-sensitive reports. Follow [SECURITY.md](../SECURITY.md) for vulnerabilities.

## Who owns yDirect?

yDirect is created, owned, and maintained by **Abhay Yemekar**. Contact [abhay.yemekar@ydirect.tech](mailto:abhay.yemekar@ydirect.tech) for owner, partnership, resume, or press inquiries. Use [support@ydirect.tech](mailto:support@ydirect.tech) for product support.
