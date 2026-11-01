# Virtual Memorial Space Privacy Policy

**Effective Date: November 1, 2026**

## 1. Introduction

Virtual Memorial Space ("the App", "we", "us") is an iOS app for creating private memorial spaces, performing remembrance rituals, and writing letters. This Privacy Policy explains what information the App handles, where it is stored, and what choices you have.

The App does not require an account. Your memorial content stays on your device. Our server is used only for Memorial Tokens, the optional in-app tokens used for premium offering styles.

By using the App, you acknowledge that you have read and understood this Privacy Policy.

## 2. Information We Do Not Collect

The App does not collect or ask for:

- Your name, email address, phone number, or any login account
- The names, photos, dates, descriptions, letters, or messages in your memorials
- Access to your whole photo library, or your camera, microphone, contacts, or location
- Your payment card details
- An advertising identifier (IDFA). The App does not track you across other companies' apps or websites and does not show the App Tracking Transparency prompt.
- Analytics or usage events. The App contains no analytics SDK and no advertising.

## 3. Memorial Content Stored Only on Your Device

The following is saved in the App's private storage on your iPhone or iPad:

- Memorial spaces: name, type (for example loved one, partner, friend, or pet), description, birth date, remembrance date, theme, and reminder setting
- Photos you add to a memorial
- Ritual records: which candle, flower, or paper offering was used, the number of tokens spent, the time, and any message you add
- Letters you write, including drafts
- Preferences: language, reduced effects, whether traditional paper offerings are shown, whether onboarding is finished, a pending purchase-sync flag, and a counter that limits rating prompts
- The last token balance received from our server, used only for offline display

This content is not uploaded to our server, is not used for advertising, and is not used for any artificial intelligence (AI) feature or training. If iCloud Backup is turned on, iOS may include this data in your device backup, which Apple handles under your Apple ID. The App has no cloud sync of its own.

**Photos.** You choose photos through the system photo picker. The App receives only the photos you select and does not access your whole photo library. A compressed copy of each selected photo is saved inside the App's storage.

## 4. Memorial Tokens and Our Server

Memorial Tokens are consumable in-app purchases. So that your balance survives reinstalling the App, it is kept on our server ("appapi"), which runs on Vercel and stores data in Vercel KV (Upstash Redis).

The server stores only:

- A randomly generated user ID, not linked to your name, email address, or Apple ID
- A digest (hash) of the access token issued for that user ID. The token itself is not stored on the server.
- Your token balance
- Purchase records: product ID, Apple transaction ID, number of tokens, and time
- Spending records: offering ID (for example a type of candle), number of tokens, the request key used to avoid double charging, balance afterwards, and time
- A ledger of credits, spends, and refunds with their amounts and related transaction or spending IDs

Each request to the server also carries the App version and a device identifier (the iOS identifierForVendor), which are used to verify the request signature. As with any web service, our hosting provider may process your IP address in routine request logs to deliver and protect the service.

The server does not store your name, email address, or anything about the people or pets you remember: no memorial names, photos, letters, or messages.

The user ID and token are stored in the iOS Keychain on your device. They may sync through iCloud Keychain, so your balance is available after reinstalling the App or on another device signed in to the same Apple ID.

## 5. Purchases

- **Apple (App Store)** processes all payments through your Apple ID. We never receive your payment card details. Apple's privacy policy: https://www.apple.com/legal/privacy/
- **RevenueCat** validates transactions. RevenueCat receives the random user ID above, transaction information (such as product ID, Apple transaction ID, and purchase time), and basic technical information such as App version, operating system version, and App Store country. Our server asks RevenueCat to confirm purchases, and RevenueCat notifies our server of purchases and refunds, so tokens are credited only once and taken back after a refund. RevenueCat's privacy policy: https://www.revenuecat.com/privacy

Memorial Tokens have no real-world monetary value. Refunds are handled by Apple under its rules. The terms of use are Apple's standard license agreement: https://www.apple.com/legal/internet-services/itunes/dev/stdeula/

## 6. Notifications (Optional)

If you turn on a remembrance-date reminder for a memorial, the App asks for notification permission and schedules local notifications on your device. Reminders do not go through our server. You can turn them off in the App or in iOS Settings.

## 7. How We Use Information

We use the information above only to:

- Show and keep your memorials, rituals, and letters on your device
- Create your token wallet, credit purchased tokens once per transaction, deduct tokens when you choose a premium offering, and take tokens back after a refund
- Verify requests and prevent fraud or duplicate credits
- Respond to your support requests

We do not sell or rent personal information, we do not use it for advertising, and we do not build advertising profiles.

## 8. Sharing

We share information only with the service providers needed to run the App (Apple, RevenueCat, and Vercel / Upstash for hosting and storage), or when required by law or a valid legal process.

## 9. Deleting Your Data

In the App's Settings:

- **Delete All Data** deletes all memorial content on this device: memorial spaces, photos, ritual records, letters, and messages.
- **Delete Token Data** deletes your wallet on our server: the user ID record, token hash, balance, purchase and spending records, and ledger. Your balance becomes zero and cannot be restored. To stop the same purchase from being credited again, we keep only the Apple transaction ID (with its product ID), with the user ID removed. The user ID and token are then removed from your Keychain.

Deleting the App removes its local content from the device, but deleting the App does **not** delete your wallet on our server. To delete it, use Delete Token Data before deleting the App, or contact us. Deleted local data may remain in earlier iCloud device backups until Apple replaces or deletes them.

You can also ask us to request deletion of the purchase record held by RevenueCat.

## 10. Security and Retention

Connections to our server, Apple, and RevenueCat use encrypted HTTPS. Requests are signed, the server stores only a hash of your token, and your identity is kept in the iOS Keychain. No method of storage or transmission is completely secure.

- Local content remains until you delete it or delete the App.
- Server wallet data remains until you use Delete Token Data or ask us to delete it.
- Apple transaction IDs without a user ID are kept to prevent duplicate credits.
- Apple and RevenueCat keep purchase records under their own policies and legal obligations.

## 11. Children's Privacy

Virtual Memorial Space is not directed at children. We do not knowingly collect personal information from children under 13 (or the minimum age required in your country). If you believe a child has provided personal information to us, contact us and we will delete it.

## 12. International Processing

Our hosting and storage providers and RevenueCat may process data in the United States or other countries different from your own. We rely on these providers' safeguards for such processing.

## 13. Your Rights

Depending on where you live, you may have the right to access, correct, delete, or restrict the processing of your personal information. Most data is on your device and under your control. For data on our server, use Delete Token Data or contact us. We may ask for information that helps us find the related records.

## 14. Changes to This Policy

We may update this Privacy Policy. The date at the top will change when we do. If the App starts collecting new kinds of data, we will update this policy first.

## 15. Contact Us

If you have questions about this Privacy Policy, contact us:

- Email: lpjustdoit@163.com

---

## Other languages

- [English](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/en/privacy.md)
- [简体中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh/privacy.md)
- [繁體中文](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/zh-tw/privacy.md)
- [日本語](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ja/privacy.md)
- [한국어](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ko/privacy.md)
- [Deutsch](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/de/privacy.md)
- [Français](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/fr/privacy.md)
- [Español](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/es/privacy.md)
- [Italiano](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/it/privacy.md)
- [Português (Portugal)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-PT/privacy.md)
- [Português (Brasil)](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/pt-BR/privacy.md)
- [ไทย](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/th/privacy.md)
- [Tiếng Việt](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/vi/privacy.md)
- [Bahasa Indonesia](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/id/privacy.md)
- [Bahasa Melayu](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ms/privacy.md)
- [العربية](https://raw.githubusercontent.com/51yourdream/privacy/refs/heads/main/memorial/ar/privacy.md)
