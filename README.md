# Decision Diary

A free, offline Android decision journal with an author's notebook aesthetic.

- **Website:** https://adrianjohn141.github.io/decision-diary/
- **Download the latest APK:** https://github.com/adrianjohn141/decision-diary/releases/latest/download/decision-diary.apk
- **Release notes:** https://github.com/adrianjohn141/decision-diary/releases/latest

This public repository contains the website, promotional screenshots, and APK releases. The Android application source is maintained separately in a private repository.

## Features

Capture decisions and original reasoning; revisit expectations and outcomes; explore personal insights; write reflection notes with optional on-device AI; protect app access with passcode/biometric unlock; and export/restore passphrase-encrypted backups. The Android application has no Internet permission, accounts, analytics, or cloud AI.

## Current download

Version 0.2.0 is a signed **development preview**, not a production release. Android 8.0+ is required. The APK is approximately 412 MB because it includes the offline AI model. Performance depends on the device; the core journal works without AI. Back up important entries before updating or replacing an installation.

## Website maintenance

The site uses plain HTML/CSS and local assets. There are no third-party scripts, remote fonts, analytics, build dependencies, or paid hosting services. GitHub Pages publishes `main` at the repository root. `.nojekyll` keeps these files as a plain static site. Push a commit to `main` to update the website.

Local preview:

```sh
python -m http.server 8765
```

Open http://localhost:8765/ . Screenshots show fictional decisions from a separate promo build; they contain no personal diary records. They were captured from the real application on a Samsung A53 and cropped to remove system bars.

## Publishing future APKs

Keep the release asset filename **`decision-diary.apk`**. Both website download buttons use GitHub's stable `/releases/latest/download/decision-diary.apk` endpoint. Publish each new version as the latest release with that asset name; no button changes are required.

Before publishing, verify the APK's application ID, version, signature, bundled model, and permissions; run the project's test/lint/build gates; and test installation on a device. Stable public releases should use a dedicated production signing key stored securely outside GitHub. Preserve the signing key for upgrades, and never publish passwords or keystores.

Example after preparing the APK and release notes locally:

```sh
gh release create v0.3.0 /path/to/decision-diary.apk /path/to/SHA256SUMS.txt \
  --repo adrianjohn141/decision-diary --latest \
  --title "Decision Diary 0.3.0" --notes-file /path/to/release-notes.md
```

Update the displayed version/approximate size in `index.html` when publishing a new version. Marking a release as a GitHub prerelease prevents the standard latest-release endpoint from selecting it; use a prerelease-specific link when appropriate.

## Privacy and third-party components

The app keeps journal records in Android app-private storage. Credentials and optional backup archives are encrypted; the Room database itself does not use a separate app-level encryption key. App-level third-party component and model acknowledgements are available in the app's Licenses screen.

This website has no tracking scripts. GitHub Pages and GitHub Downloads are hosted by GitHub and subject to GitHub's privacy policy and standard service limits.
