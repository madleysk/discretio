# Privacy Policy for Discretio Secure Vault

**Status: DRAFT / SAMPLE — placeholder text for Play Store submission, pending final legal review. Do not treat as a finished legal document.**

*Last updated: [DATE]*

*[Lire cette politique en français](PRIVACY_POLICY.fr.md)*

This Privacy Policy describes how Discretio Secure Vault ("the app", "we", "us") — package name `com.vault.trueaes` — handles information when you use it.

## Summary

Discretio is an offline, on-device encrypted vault. **We do not operate any server, and the app never uploads, syncs, or transmits your files, notes, photos, folders, passwords, or vault contents anywhere.** Everything you store in the vault is encrypted (AES-256-GCM for files, AES-256-XTS for hidden containers) and stays on your device. We have no account system and no backend, so we have no ability to see, access, recover, or hand over your vault contents to anyone, including ourselves.

The only data that ever leaves your device is described in the "Purchases" section below, and that data goes to Google, not to us.

## Data we collect

We — the developers of Discretio — do not collect, store, or have access to any personal data, vault contents, or usage analytics. The app does not currently integrate any analytics, crash-reporting, or advertising service.

## Data handled by third-party services

The app embeds Google Play Billing to process in-app purchases. It operates under Google's own privacy policy, linked below.

### Purchases (Google Play Billing)

- In-app purchases (e.g. unlocking premium features) are processed entirely by Google Play Billing.
- We do not receive or store your payment method, card details, or billing address — that information is handled by Google. We only receive confirmation that an entitlement was purchased, which is stored locally on your device to unlock the corresponding feature.
- Google Play Billing may process account and transaction information per [Google's Privacy Policy](https://policies.google.com/privacy).

## Permissions the app requests, and why

| Permission | Purpose |
|---|---|
| Camera / Microphone | Only used when you choose to use the in-app Secure Capture feature to photograph/record directly into the encrypted vault. Nothing is captured without you actively opening that feature. |
| Biometric / Fingerprint | Used only to unlock the app/vault with your device's biometric hardware, as an alternative to your master password. Biometric data itself is handled entirely by the Android OS and never reaches the app or us. |
| Storage / Photos & Videos (media permissions) | Used only when you choose to import an existing file/photo/video into the vault, or export/share one back out. |
| Notifications | Used for local, on-device notifications (e.g. related to the vault's auto-lock/background service). We do not use push notifications from a server, because we have no server. |
| Internet / Network State | Used exclusively by the Google Play Billing SDK described above. The vault's encryption, storage, and file management code never makes a network request. |

## Data retention and deletion

Because nothing you store in the vault is ever sent to us, there is nothing on our end to retain or delete. Your vault data lives only on your device (or wherever you've configured local/removable storage to point), encrypted at rest, until you delete it yourself or uninstall the app.

## Children's privacy

The app is not directed at children, and we do not knowingly collect personal information from anyone, regardless of age — this follows automatically from the app having no data-collection mechanism in the first place.

## Security

Vault contents are encrypted on-device using AES-256-GCM (individual files) or AES-256-XTS (hidden VeraCrypt-compatible containers), with keys derived from your master password via Argon2id/PBKDF2. Master key material is generated randomly and only ever exists in native memory, never written to disk in plaintext. See the app's public source code for implementation details.

## Disclaimer of liability

Discretio Secure Vault is provided "as is," without warranty of any kind. Because of the zero-knowledge design described above, we have no way to access, view, back up, or recover your data or your Master Password under any circumstances — including a forgotten password, misuse of the app, device loss or damage, or an app malfunction. You are solely responsible for remembering your Master Password (or safely storing the app's optional, one-time password-recovery code, if you choose to generate one) and for keeping your own backups — use the app's Encrypted Backup feature (Settings → Encrypted Backup) regularly, since device loss, damage, or an uninstall can otherwise mean permanent loss of everything in your vault. To the fullest extent permitted by law, the developer is not liable for any data loss or other damages arising from use of this app.

## Changes to this policy

If this policy changes, we will update the "Last updated" date above and, for material changes, note it in the app's release notes.

## Contact

Questions about this policy can be raised via the project's GitHub Issues page:
https://github.com/madleysk/TrueAESVault/issues

*(Placeholder contact email — replace before final publication: `[INSERT CONTACT EMAIL]`)*

---

*This document is a draft sample prepared ahead of Google Play Store submission and is intended to be reviewed, refined, and replaced with a final version — including a real "last updated" date and verified contact details — before the app is published.*
