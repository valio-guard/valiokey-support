# ValioKey — Privacy Policy

Updated November 16, 2026.

ValioKey is a zero-knowledge password manager. This policy covers the iPhone app in its TestFlight beta and the ValioKey for Chrome extension in its invitation-only beta. Both use the same server and the same rules. Use made-up test logins only: do not store real passwords in either beta.

## What the server cannot read

Your logins are encrypted on your device (your iPhone, or your browser for the Chrome extension) before they are sent. The server stores them only as encrypted data and cannot read their contents. It never receives your master password or your recovery key. Because of this, ValioKey cannot reset your master password or recover your vault for you.

## What the server stores

- **Account:** your email address, an optional display name, when the account was created, and whether a deletion is scheduled.
- **Sign-in checks and keys:** values that let the server check your sign-in without knowing your master password, encryption settings, public keys, and encrypted copies of your keys.
- **Devices:** each signed-in device's platform (for example "ios" or "chrome"), app version, public key, an encrypted device name, sign-in session dates, when it was last seen, and its last IP address.
- **Vault:** your encrypted logins, earlier encrypted versions, and information the server needs to sync them, such as their number, sizes and timestamps. The server can see this information even though it cannot read the logins.
- **Security events:** a record of events such as sign-ins and password changes, with the time, device, platform, app version and IP address.
- **Email and abuse protection:** queued emails until they are handled, and limited records used to slow repeated attempts.

## Email

We send email for verification and sign-in codes, recovery, password and recovery-key changes, new-device notices, attempts to register your address, and account deletion. Email is sent through Amazon Simple Email Service.

## Where data is kept

The beta server, its database and its encrypted backups run on Amazon Web Services in the United States (us-east-1).

## How long data is kept

| Data | Kept for |
|---|---|
| Earlier encrypted versions of a login | 30 days after being replaced |
| Revoked or inactive devices | Removed after 30 days |
| IP address on a device or security event | Cleared after 30 days |
| Security events | 365 days |
| Handled emails | Recipient and content erased once handled; the remaining record goes after 7 days |
| Database backups | About 14 days, and deleted backup versions up to 14 more days |
| Marker that an account was deleted (keyed values, not your email address in readable form) | 365 days |

## Sharing

We do not sell your data and do not share it with anyone except the services that run the beta (Amazon Web Services for hosting and email). We do not use your data for advertising, and we do not use it to decide credit.

## ValioKey for Chrome

What the extension does on your computer:

- It keeps an encrypted copy of your vault and its sync state in this browser, and its settings: auto-lock time, clipboard-clearing time, appearance, and your filling preferences (the login-field menu, the save and update offers, and the sites you chose never to save for).
- While your vault is unlocked, it holds the unlock state in Chrome's session storage, which is cleared when the vault locks or the browser closes. It locks when you choose (when the popup closes, after 1, 5 or 15 minutes, after 1, 4 or 8 hours, or when Chrome closes) and always when the browser closes.
- It reads the address of the tab you are on, and of that tab's frames, only on your computer, to show the logins for that site and to fill the one you choose. It does not keep a history of the sites you visit and does not send them anywhere.
- When you press Fill, it puts the login you chose into the login fields of the page you are on. A web page can read what is in its own fields once they are filled; no password manager can prevent this.
- If you turn on the login-field menu and allow site access, a small script looks for login fields on the websites you visit and shows the ValioKey button in them. The menu that opens from it is drawn by the extension, not the page, and shows only the titles and usernames of your logins for that site.
- On those same sites, when you sign in, the script hands the username and password you typed to the extension so it can offer to save a new login or update a changed password. They stay in the extension's memory for at most 5 minutes and are written to your vault (encrypted) only if you press Save or Update. You can turn either offer off, or block a site, in Settings.
- The Security tab checks your passwords for weakness and reuse inside the extension. The results are not stored and not sent.
- When you copy a password, the extension keeps a one-way fingerprint of it and clears the clipboard after the time you set, only if the clipboard still holds that password. It never reads the clipboard at any other time. Clipboard contents can reach your other devices through the system's clipboard sync, which ValioKey does not control. A copied password is cleared only while Chrome is running.
- It has no analytics, no advertising and no third-party tracking code, and it loads no code from the internet.

Permissions: the extension asks Chrome for these, each only for the purpose shown: storage (settings and your encrypted local data), alarms (timed locking, sync and clipboard clearing), activeTab (the tab you clicked the toolbar button on), scripting (putting the chosen login into the page, and the optional login-field menu), offscreen, clipboardRead and clipboardWrite (copying a password and clearing it safely), webNavigation (choosing the right frame to fill, and showing the save offer on the next page), and access to the ValioKey server. Access to all websites is optional, is requested only if you turn on the login-field menu, and can be turned off at any time in Settings or in Chrome.

Signing out in the extension removes the account's data from this browser. Removing the extension removes the extension's local data from your browser.

## Deleting your account

In the iPhone app, open Settings → Account → Delete account. Deletion takes effect after a 7-day grace period, during which you can cancel. Your account and its encrypted data are then removed from the server, and remaining copies leave backups as they expire. You can also ask us by email.

## Beta resets

Beta data may be reset. We will give notice by email except in an emergency. All beta accounts are deleted after the beta ends.

## Apple and TestFlight

Apple provides TestFlight distribution, diagnostics and beta feedback under Apple's policies. Reports and screenshots you choose to send may reach the developer. Never include a master password, a recovery key or real login details.

## Google and the Chrome Web Store

Google provides the Chrome Web Store and the Chrome browser under Google's policies. Chrome may send Google information about the extension under Google's own privacy policy; ValioKey does not control that.

## Contacting support

If you email support, we receive your address, your message and any attachments through our email provider, so that we can respond. Do not send master passwords, recovery keys or real login details.

## This website

These pages are hosted by GitHub Pages. GitHub handles website connection information under its [Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

## Contact

[valiokey@valioguard.com](mailto:valiokey@valioguard.com). Beta testers can also use Send Beta Feedback in TestFlight.
