# Data and permissions

The server operator controls the server and its retained data.

## Incoming Mercari alerts

Android grants broad notification access. Monitor processes only recognized saved-search new-item alerts from Mercari Japan. Transaction notifications and other apps' notifications are excluded. Sending also requires the separate **Send Mercari alerts** switch.

An event contains its title (up to 240 characters), text (up to 1,000), time and technical identifiers. It is sent over authenticated HTTPS to the paired server. Pending uploads are encrypted on the phone, limited to 200 events and expire after 24 hours. Android can delay delivery and cleanup.

## Search data and photos

The server reads search terms and recognized price and condition filters from the alert. When enabled, an unofficial Mercari adapter uses those criteria to fetch a limited set of products. Monitor does not read Mercari account credentials or make purchases.

Product photos load from Mercari's public image CDN. The widget keeps a small encrypted photo cache; ordinary app images also use Android's image cache.

## Your device and local preferences

Pairing creates credentials for that device. Keys, favorites and hidden-item preferences use secure storage on the phone. Favorites and hidden items do not sync between phones.

Monitor's product notifications need a separate Android permission. Adding a widget does not turn on notification reading or sending.

## Retention and removal

The server retains notification history and saved results until its operator removes them. Forgetting the server or revoking a device stops future access but does not delete existing server history. Contact the operator who provided your access to request removal.

Telegram delivery is optional and must be configured separately on the server. The app does not collect email.

See [installation](INSTALL.md) for setup. When reporting a problem, leave out private codes, keys, notification text and server databases.
