# SpendSense

A personal expense tracker. It catches UPI, bank and card payments from bank SMS and payment-app notifications, asks what each payment was for and whether you split it, and answers questions about your spending. All data stays encrypted on your phone.

This repository only hosts the app downloads. The source code is private.

## Android

1. If Android says the app isn't compatible or can't be installed, uninstall your older SpendSense first. Early test builds were signed with a different key.
2. Download **[SpendSense.apk](https://github.com/JayantNagori-TAP/spendsense-releases/releases/latest/download/SpendSense.apk)** on your phone.
3. Open it and allow your browser to install unknown apps when asked.
4. Follow the setup screen. If SMS or notification access is greyed out with "Restricted setting": open **App info → ⋮ (top right) → Allow restricted settings**, then try again.

Later versions from this page install over the old one, and your data is kept.

## iPhone

iPhone builds install through [SideStore](https://sidestore.io) or [AltStore](https://altstore.io) with your own free Apple ID. Instructions will be added here with the first iPhone release.

## Check you have the genuine app

Only install SpendSense from this page. The genuine Android app is signed with this certificate:

```
SHA-256: AD:F4:B2:1E:B8:8F:68:04:22:F6:67:9B:A1:0A:DC:87:43:5A:8A:03:BB:35:14:C8:11:0B:5B:95:C7:9C:9F:C7
```

Each release lists SHA-256 checksums for its files. A copy signed with any other key shows an "isn't genuine" screen and won't open your data.

**SpendSense never asks for your bank password, OTP, card number, CVV or UPI PIN.** If an app or person claiming to be SpendSense asks for any of these, it's a scam.

## License

All rights reserved. See [LICENSE](LICENSE).
