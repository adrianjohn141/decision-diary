# Privacy Policy

Effective: September 30, 2026 · Document version 1

## 1. Scope and contact

This notice explains how Decision Diary, provided by Aj Escaño, handles information in the Android application, promotional website, release downloads, and public support pages. The application works offline. The website and downloads are hosted by GitHub and have different data-handling practices.

Privacy contact: https://github.com/adrianjohn141/decision-diary/issues

Do not post private diary information, passcodes, or backup files in public issues. Ask for a suitable private contact channel before disclosing sensitive details.

## 2. Information processed on your device

The app stores the decisions, options, reasons, expectations, confidence ratings, concerns, review dates, outcomes, journal notes, and conversation messages you enter. It also stores your optional companion profile, app preferences, security settings, and reminder-delivery records. These records support journaling, reviews, insights, reminders, and the optional reflection companion. You choose what to enter and which optional features to enable.

App passcodes are verified using salted PBKDF2 hashes rather than stored as plaintext. The credential store is encrypted using an Android Keystore-backed key. Biometric/device authentication is handled by Android. The app receives authentication results; it does not receive or store fingerprint images, face images, or biometric templates.

Aj Escaño does not receive your journal records from the app. There are no app accounts, analytics, advertising trackers, remote crash reports, cloud synchronization, or cloud AI services. The app has no Internet permission. It does not request contacts, location, microphone, or camera access for journaling. Android notification permission is used only for optional review reminders.

## 3. Optional local AI

When enabled, AI uses relevant decision context, companion preferences, and recent conversation text locally to generate a reflection. Prompts are not sent to Aj Escaño or a remote AI service. Generated replies saved in a conversation remain part of the local diary. No automated decision is made on your behalf, and reflection is not professional advice. Basic local prompts may be used when the model cannot run.

Disabling AI prevents new companion replies and unloads the local inference model. It does not delete existing conversation history. You can keep writing personal notes or delete stored conversations and entries through the app.

## 4. Storage and security boundaries

Diary records use Android app-private storage. The Room database does not have a separate application-level encryption key. App lock, biometric/device unlock, auto-lock, and screen-capture protection reduce unwanted access but cannot guarantee protection on a compromised or unlocked device. Credentials and optional encrypted backup archives are encrypted. The app does not log journal text as diagnostic content.

Automatic Android cloud backup and device-transfer participation are disabled in the app configuration. Device and operating-system behavior may vary. Protect your device, keep backups you control, and avoid entering information you cannot safely store locally.

## 5. Export, import, and storage providers

Exports contain diary records and ordinary app preferences; they do not contain your app-lock passcode, credential hash, or device-bound key. You choose the destination with Android's document picker. A provider you select, such as a cloud-backed file service, may synchronize the exported file under its own policy even though Decision Diary has no Internet permission.

Passphrase-encrypted archives protect file contents with AES-256-GCM. Plaintext JSON exports are readable without a passphrase. Imported files merge journal records and restore supported preferences. Exported copies are not removed when you delete data inside the app. Keep passphrases secure; the provider cannot recover them for you.

## 6. Retention and your controls

Local data remains until you delete entries or conversations, use Delete all diary data, clear app storage, or uninstall. Access and edit your records in the app and use export for a portable copy. You control reminders, AI, and app-lock settings. Deleting all diary entries does not necessarily erase app preferences or security credentials; clearing storage or uninstalling removes those local app records. Deletion does not guarantee forensic erasure from device storage or remove backups you exported elsewhere.

Because the provider does not receive the app's diary database, Aj Escaño cannot access, edit, recover, or remotely delete that database for you. To ask about privacy or exercise rights concerning information you separately send to support, use the contact page without posting sensitive data publicly. Applicable statutory rights are unaffected.

## 7. Website, downloads, and support

The promotional site uses local screenshots and plain HTML/CSS, without analytics, tracking scripts, advertising, or embedded remote AI. Screenshot entries are fictional examples. GitHub processes hosting and download requests, including technical request information such as IP addresses, under GitHub's privacy policy. GitHub may use cookies on its own repository, account, download, or support pages. The Android app's offline privacy statements do not describe GitHub's services.

When you open a public issue or comment, GitHub displays the information you submit and your account details according to its settings. Aj Escaño may read and use that information to answer requests, diagnose issues, or maintain the app. Public discussions can remain visible until removed under GitHub's controls and policies. Avoid private diary content and unnecessary personal information.

GitHub privacy policy: https://docs.github.com/en/site-policy/privacy-policies/github-general-privacy-statement

## 8. Updates

Material changes will be reflected in the effective date or document version and distributed with app or website updates. Any future addition of remote collection or processing would need a revised notice and appropriate user controls before that behavior begins. This version describes the current offline application and GitHub-hosted services.
