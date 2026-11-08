# ValioKey — Privacy Policy

Updated November 8, 2026.

ValioKey is a zero-knowledge password manager for iPhone. This policy covers the TestFlight beta. Use made-up test logins only: do not store real passwords in this beta.

## What the server cannot read

Your logins are encrypted on your iPhone before they are sent. The server stores them only as encrypted data and cannot read their contents. It never receives your master password or your recovery key. Because of this, ValioKey cannot reset your master password or recover your vault for you.

## What the server stores

- **Account:** your email address, an optional display name, when the account was created, and whether a deletion is scheduled.
- **Sign-in checks and keys:** values that let the server check your sign-in without knowing your master password, encryption settings, public keys, and encrypted copies of your keys.
- **Devices:** each signed-in device's platform, app version, public key, an encrypted device name, sign-in session dates, when it was last seen, and its last IP address.
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

## Deleting your account

In the app, open Settings → Account → Delete account. Deletion takes effect after a 7-day grace period, during which you can cancel. Your account and its encrypted data are then removed from the server, and remaining copies leave backups as they expire. You can also ask us by email.

## Beta resets

Beta data may be reset. We will give notice by email except in an emergency. All beta accounts are deleted after the beta ends.

## Apple and TestFlight

Apple provides TestFlight distribution, diagnostics and beta feedback under Apple's policies. Reports and screenshots you choose to send may reach the developer. Never include a master password, a recovery key or real login details.

## Contacting support

If you email support, we receive your address, your message and any attachments through our email provider, so that we can respond. Do not send master passwords, recovery keys or real login details.

## This website

These pages are hosted by GitHub Pages. GitHub handles website connection information under its [Privacy Statement](https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement).

## Contact

[valiokey@valioguard.com](mailto:valiokey@valioguard.com). Beta testers can also use Send Beta Feedback in TestFlight.
