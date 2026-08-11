# Feature guide

This guide describes user-visible behavior in yDirect `1.3.1`. It avoids private implementation details and does not promise unreleased roadmap items.

## Snippet library

- Create, edit, move, and delete folders and snippets within the user's access level.
- Switch between folder and list views.
- Search by the user-visible snippet information available to the signed-in library.
- Sort content and use timestamps/copy counts as lightweight context.
- Copy a selected snippet with one action.
- Copy the last-used snippet with the `Alt+C` keyboard shortcut.
- Optionally mask displayed snippet values to reduce casual shoulder-surfing.

Masking changes what is visible on screen. It does not encrypt the stored content and must not be treated as protection for high-risk secrets.

## Attached workspace

- Open yDirect from the Chrome toolbar or `Alt+S`.
- Attach the workspace to the right edge of a normal `http://` or `https://` page.
- Keep the current page visible while browsing the library.
- Use a standalone extension page when Chrome does not allow injection into a restricted page.
- Move or remove the optional floating shortcut and restore it from the toolbar.

yDirect does not request persistent access to every website. Access to the active page follows the user's toolbar click or shortcut.

## Accounts and local state

- Register with email and password or continue with Google.
- Verify an email account before protected cloud/workspace actions.
- Keep local library state separated by signed-in account.
- Sign out, clear browser-local data, or request account deletion from settings.
- Use generic account messages designed to avoid revealing whether another account exists.

## Import and export

| Format | Primary use |
| --- | --- |
| JSON | Restorable yDirect backup and transfer |
| Passphrase-encrypted JSON | Portable backup when a user wants file-level passphrase protection |
| Excel | Human-readable review and editing in spreadsheet tools |

Exports start only after a user selects an export action. yDirect does not read, monitor, open, or modify existing downloads.

Before any destructive import or account operation, keep a verified export of content that cannot be replaced.

## Optional cloud backup

- Cloud backup is a deliberate, authenticated feature.
- Automatic backup defaults to off.
- A successful backup is read back and checked for integrity.
- The service keeps the latest successful backup and one previous recovery point.
- Restore is a recovery convenience, not an archival or disaster-recovery guarantee.

Users should keep independent exports of important content.

## Workspaces and selective sharing

Every account has a personal/home workspace and may participate in other workspaces. Resource IDs and permissions stay scoped to their workspace.

### Roles

| Role | Content | Sharing | Membership |
| --- | --- | --- | --- |
| **Super Admin** | Organize all content in the owned workspace | Share folders/snippets and revoke resource access | Add Members and Core Members; retains final control |
| **Core Member** | Organize workspace content | Share folders/snippets and revoke resource access | Add Members; cannot add another Core Member or transfer ownership in this release |
| **Member** | View explicitly shared resources; add to directly shared folders; edit/delete only their own contributions | Share content from their own workspace; cannot re-share another person's protected content | May remove their own access |

### Sharing rules

- A direct folder grant includes the folder and its current/future snippets, except resources the recipient explicitly removed.
- A direct snippet grant includes that snippet plus a context-only folder shell.
- A context-only folder does not allow contributions.
- A Member may contribute only inside a directly shared folder.
- A Member's contribution records its creator and remains editable/deletable by that creator and workspace managers.
- Removing access removes the recipient's future view; it does not delete the owner's content.
- Cloud access is enforced by authenticated backend checks, not only by the interface.

## Appearance and accessibility

- Light and dark themes.
- Keyboard-accessible dialogs with focus movement, trapping, Escape dismissal, and restoration.
- Narrow layouts designed for popup and attached-panel widths.
- Long content wraps rather than relying on horizontal scrolling.

## Support and legal surfaces

- Public account-action pages for email verification and password reset.
- Public Support Center with safe troubleshooting guidance.
- Public Privacy Policy and Terms of Service.
- Uninstall guidance and a public changelog.

## Safety boundaries

yDirect is not designed to store:

- passwords or one-time codes;
- payment-card or banking information;
- private keys, recovery codes, or signing material;
- regulated health, identity, or customer records;
- any data whose exposure would create serious harm.

Treat copied text as a draft: verify the recipient, facts, names, links, and context before sending it.
