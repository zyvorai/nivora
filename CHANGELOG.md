# Changelog

Release notes for Nivora, the macOS network intelligence app.

## 0.5.4 — 2026-11-19

- Licence: an optional licence key. **Nivora > Licence…** shows your licence status. A free 30-day trial key is available from sales@zyvor.dev; licences are bought at https://zyvor.dev/buy. Nothing is disabled without a key. Earlier paid purchases keep their perpetual licence and need no key.
- Native: a refresh interval setting (1, 2 or 5 seconds; the default stays 2 seconds), pinned applications (starred apps are listed first in Applications and in the menu bar), launch at login (macOS may ask for approval in System Settings) and diagnostics.
- Requirement: Nivora now needs macOS 15 or later (it ran on macOS 14 before).
- The notarized build still leaves out the content filter and the capture helper (no Apple NetworkExtension entitlement), so per-app attribution uses the collector.

## 0.5.3 — 2026-11-06

- Native: Network Map, Domains, DNS, Routes and VPN panes, a ⌘K command palette over panes, apps and actions, and two Shortcuts actions ("Top apps", "Unblock an app").
- Collector: opt-in alert delivery (webhook or syslog, with a severity threshold and a cooldown), configurable history retention, a user tracker list and optional local country/ASN labels.
- Command line and MCP: `nivoractl` gains JSON output, a watch mode, a version check and shell completions; the read-only MCP server adds tools for trust, privacy, egress, usage, listeners, FluxVM, profiles and the timeline.

## 0.5.2 — 2026-10-16

- Fix: "Collector unavailable" no longer appears on Macs that run FluxVM.
- Fix: the app no longer flashes "Collector unavailable" while the bundled collector starts.
- Native: when the content filter is not part of the build, the app says so instead of showing a raw system error.
- A Developer ID signed, notarized and stapled build, without the content filter and the capture helper.

## 0.5.1 — 2026-10-15

- The release app is sealed with an ad-hoc signature so the bundle verifies as intact.

## 0.5.0 — 2026-10-15

- A "Network" widget (small and medium) and Shortcuts/Siri actions ("How is my network?", "Block an app for one hour").
- Insights: a trust score per app, a privacy report card, verified process identity, situation profiles, policy dry-runs, a FluxVM sandbox egress view and a multi-Mac fleet view.
- Time-travel diff and an incident narrative, an on-demand path check, "Why this flow?" evidence for each flow, and shadow rules that show what a block would match before it is enabled.
- LAN change detection (new device, IP-to-MAC change, gateway change, Wi-Fi network change, DNS bypassing the VPN).
- Daily per-app usage with optional budgets, project attribution and Prometheus metrics.
- Fix: the bundled collector no longer outlives the app.

## 0.3.0 — 2026-10-13

- Live throughput strip and sparklines, filter bar with saved views, flow inspector, grouped Flows views and baseline compare.
- Opt-in, headers-only packet capture through a separately approved helper (needs a signed, provisioned build).
- Export of flows, apps, timeline and snapshots as CSV, JSON, NDJSON or zip, with optional redaction.
- A shared flow filter grammar across the app, dashboard and command line.
- A Time Machine pane, a command palette and keyboard shortcuts.

## 0.2.0 — 2026-10-13

- Live per-flow and per-app rates, a 0–100 network health score with explained components and a local network diagnosis.
- App to interface to destination Network Map, neighbours, listening services and exposure classification.
- Learning of destination behaviour with first-seen findings and Time Machine events.
- FluxVM network health and endpoints, with host-flow correlation.

## 0.1.0 — 2026-10-13

- Initial release: per-app flows, DNS, routes, interfaces and VPNs, FluxVM integration, a SQLite history with a Network Time Machine, observe/allow/block rules, a local investigator, a dashboard and a native SwiftUI app.
