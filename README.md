# Mercari Monitor

An Android app for following saved searches on Mercari Japan. It collects product results in one feed, with photos, prices, favorites and hidden items. You can also turn on product notifications or add the feed to your home screen.

[Download 0.8.6 APK](https://github.com/Froas/mercari-monitor/releases/download/v0.8.6/mercari-monitor-0.8.6.apk) · [Release notes](https://github.com/Froas/mercari-monitor/releases/tag/v0.8.6) · Android 9+ · 64-bit

The app needs a running server and a private pairing code from its operator. This APK connects to the server it was built for; installing it alone does not provide server access.

## Setup

1. Install the APK and connect using your pairing code.
2. Set up saved searches and their push notifications in the official Mercari app.
3. In Monitor, grant Android notification access and enable **Send Mercari alerts**.
4. If wanted, enable **Product notifications** or add a widget from **Settings → Home screen widget → Add**.

See [installation and updates](INSTALL.md) and [data and permissions](DATA.md) for details.

## How results work

A saved-search alert triggers a limited search on the server. Monitor saves the returned products and marks those it has not seen before. A result is not necessarily the exact item that caused the original alert, and the feed does not cover every matching listing.

Favorites, hidden items, local search and sorting help manage the feed. Monitor filters are separate from the saved searches configured in Mercari.

## Before installing

- Android 9 or newer is required. The APK supports arm64-v8a phones and x86_64 emulators.
- The server must stay online. Using a different server address requires a matching APK build.
- Android can delay background updates.
- This version keeps the existing development signing key so it can update earlier installations.

Mercari Monitor uses an unofficial Mercari adapter and is not affiliated with Mercari.
