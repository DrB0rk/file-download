# file-download

Static host for internal iPad app installs.

## Install StudioSattelite on an iPad

**👉 https://drb0rk.github.io/file-download/**

Open that link in **Safari on the iPad**, tap **Install on this iPad**, and trust
the developer profile on first launch
(Settings → General → VPN & Device Management).

## What's here

| File | URL |
|------|-----|
| Install page | `https://drb0rk.github.io/file-download/` |
| IPA | `https://drb0rk.github.io/file-download/StudioSattelite.ipa` |
| itms manifest | `https://drb0rk.github.io/file-download/manifest.plist` |

## Requirements

- iPad whose UDID is registered on Apple Developer team **`L34UB8AH3J`**
- Safari (the itms-services install link only works from Safari on iOS)
- The app is development-signed; trust the developer profile on first launch

## Updating the IPA

1. Replace `StudioSattelite.ipa` with the new build (same filename to avoid cache issues,
   or bump the filename if iOS caches the manifest)
2. If you bump the filename, also update the `url` field in `manifest.plist`
3. Commit & push to `main` — Pages redeploys automatically (~30s)