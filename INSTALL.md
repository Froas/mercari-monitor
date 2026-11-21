# Installation

You need Android 9 or newer on a 64-bit ARM phone, access to the app's server and a pairing code from its operator. Codes are single-use and expire after 10 minutes. The APK also supports x86_64 emulators.

## Install and connect

These steps apply to previously downloaded copies.

1. Open the APK on your phone and confirm installation. If asked, allow installation for the browser or file manager you used. Keep Play Protect enabled.
2. Open Mercari Monitor and enter your pairing code.
3. In the official Mercari Japan app, configure saved searches and enable their push notifications.
4. In Monitor, review the permission explanation, grant Android notification access and enable **Send Mercari alerts**. Reading notifications and sending them are separate choices.

For Monitor's own alerts, enable **Product notifications** and confirm Android's notification permission. It starts with future results, without replaying old history.

For a widget, choose **Settings → Home screen widget → Add** and place it on your home screen. Product notifications can stay off.

If Android blocks notification access for a downloaded app, see its [restricted settings guide](https://support.google.com/android/answer/12623953).

## Check the download

If you saved `SHA256SUMS` with the APK, compare the APK's SHA-256 with that file. On macOS, run `shasum -a 256 FILE.apk`; on Linux, use `sha256sum FILE.apk`.

## Updating

Install the newer APK over the existing app. Updates need the same package and signing key; this version retains the development key used by earlier builds. Uninstalling first removes the local connection and preferences.

## Server access

This APK is built for one HTTPS server. Changing the address in Settings does not make native forwarding, product notifications or the widget work with another server; that requires a matching build. The server must remain online, and its temporary tunnel address can change.

See [data and permissions](DATA.md) before enabling collection. Keep pairing codes and device keys private.
