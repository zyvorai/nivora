# Installing Nivora

**Requirements:** macOS 15 or later, Apple silicon.

**Production use (₹999 incl. GST).** After payment you receive an email with a GST invoice and a download link. Verify the
download against the `.sha256` shown on the payment page or sent on request. Licences are bought at https://zyvor.dev/buy.

## Install

1. Download `Nivora-X.Y.Z.dmg` and `Nivora-X.Y.Z.dmg.sha256` from [Releases](https://github.com/zyvorai/nivora/releases).
2. Verify the download: `shasum -a 256 Nivora-X.Y.Z.dmg` must print the value in the `.sha256` file.
3. Open the DMG and drag **Nivora** to **Applications**.
4. Open Nivora. The build is signed with our Apple Developer ID. Notarized by Apple; macOS shows its standard first-open confirmation for apps downloaded from the internet.

Closing the window keeps Nivora in the menu bar; **Quit** is in the menu-bar menu. A welcome sheet appears once on first launch.

## Trial key and licence

The app runs without a key. For a free 30-day trial key, email sales@zyvor.dev. Paste the key under **Nivora > Licence…**; the sidebar then shows your licence
status. Nothing is disabled without a key. To buy a licence, go to https://zyvor.dev/buy. Earlier paid purchases keep their
perpetual licence and need no key.

## What the notarized build can and cannot do

| Works | Not in the notarized build |
| --- | --- |
| Per-app flows and byte counters through the built-in collector | Content-filter system extension (per-flow app attribution from the system) |
| Interfaces, DNS, routes, VPNs, neighbours, listeners | Capture helper (root `tcpdump`, approved in System Settings) |
| Time Machine history, health, exports, filters, menu bar, widget | Blocking rules taking effect |

The content filter and the capture helper need an Apple NetworkExtension entitlement that is not available to us, so per-app
attribution uses the collector. Nivora runs in observe-first mode.

## Uninstall

```bash
pkill -x Nivora
rm -rf /Applications/Nivora.app
rm -rf ~/.local/share/nivora          # history; optional
```
