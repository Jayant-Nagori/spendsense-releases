# SpendSense

A personal expense tracker. It catches UPI, bank and card payments from bank SMS and payment-app notifications, asks what each payment was for and whether you split it, and answers questions about your spending. All data stays encrypted on your phone.

This repository only hosts the app downloads. The source code is private.

## Android

1. **Updating?** Install the new version over the top — don't uninstall first, or your data is deleted. If Android says "App not installed", you have an early test build signed with a different key: take a backup first (see below), then uninstall, install and restore.
2. Download **[SpendSense.apk](https://github.com/JayantNagori-TAP/spendsense-releases/releases/latest/download/SpendSense.apk)** on your phone.
3. Open it and allow your browser to install unknown apps when asked.
4. Follow the setup screen. If SMS or notification access is greyed out with "Restricted setting": open **App info → ⋮ (top right) → Allow restricted settings**, then try again.

Later versions from this page install over the old one, and your data is kept.

## iPhone

iPhone builds install through [SideStore](https://sidestore.io) or [AltStore](https://altstore.io), signed with your own free Apple ID. Needs iOS 17.2 or later.

1. Install SideStore or AltStore by following its own setup guide.
2. In SideStore/AltStore open **Sources → +** and add:
   `https://raw.githubusercontent.com/JayantNagori-TAP/spendsense-releases/main/altstore-source.json`
3. Open the SpendSense source and tap **Install**. (Or download **SpendSense.ipa** from the latest release and open it in SideStore/AltStore.)
4. Turn on **Settings → Privacy & Security → Developer Mode** if iOS asks, and restart.
5. With a free Apple ID, apps must be refreshed every 7 days: open SideStore/AltStore and tap **Refresh All** (or let its background refresh do it). Your data is kept when you refresh or update.

**Bank SMS on iPhone:** iOS doesn't let apps read SMS. Set up a Shortcuts automation instead: **Shortcuts → Automation → + → Message**, Message Contains `debited` (add more for `spent`, `credited`), choose **Run Immediately**, and add the action **SpendSense → Log bank SMS** with the message as input. You can also import Gmail alerts or PDF statements inside the app.

## Your data, updates and backups

- Updating (Android: over the top; iPhone: Update/Refresh in SideStore/AltStore) keeps all your data.
- **Uninstalling the app or clearing its data deletes everything**, including notes. The encryption key never leaves your phone, so nobody — not even the developer — can recover it.
- Take a backup in **Settings → Backup**: an encrypted file protected by a password you choose, saved wherever you like (Drive, Files, etc.). On Android, turn on weekly auto-backup; on iPhone, take one now and then. Restore it on a new phone from the same screen. Backups never contain your AI keys or passwords.

## Check you have the genuine app

Only install SpendSense from this page. The genuine Android app is signed with this certificate:

```
SHA-256: AD:F4:B2:1E:B8:8F:68:04:22:F6:67:9B:A1:0A:DC:87:43:5A:8A:03:BB:35:14:C8:11:0B:5B:95:C7:9C:9F:C7
```

Each release lists SHA-256 checksums for its files. A copy signed with any other key shows an "isn't genuine" screen and won't open your data.

**SpendSense never asks for your bank password, OTP, card number, CVV or UPI PIN.** If an app or person claiming to be SpendSense asks for any of these, it's a scam.

## License

All rights reserved. See [LICENSE](LICENSE).
