---
title: PriceLens privacy policy
---

# PriceLens privacy policy

Last updated: 13 November 2026

This policy explains what the PriceLens app for Android, as distributed on Google Play, does with information on your phone. PriceLens is published by the PriceLens developer. The same policy is published at https://sexualmoose.github.io/app-privacy/pricelens/ and is included in the app (About > Privacy policy).

## Summary

- PriceLens has no accounts, no ads, no analytics and no tracking.
- Everything PriceLens reads is processed on your phone. The developer receives no data from the app.
- The only thing PriceLens downloads is public exchange rates. Those requests contain no personal information; what they do contain is listed in full under "What leaves your phone".

## What PriceLens uses and why

### Accessibility service (what is on your screen)

- PriceLens uses Android's Accessibility service (the Accessibility API) to learn which app is in front, so that its small currency button appears only over the camera or translate apps you selected. PriceLens is not an assistive tool for people with disabilities.
- Only after you tap that button, and only while live conversion is on, PriceLens captures pictures of that app's window (a few per second) and reads where the app's on-screen controls are. Text recognition (Google ML Kit, built into the app) runs on your phone to find prices, and PriceLens draws converted amounts on top.
- On Android 14 and newer each picture shows that app's window only. On Android 11 to 13 the system can only provide a picture of the whole screen: PriceLens keeps just the part where that app is and discards the rest at once, so something shown on top of that app at that moment (for example a notification banner) can be in that part.
- Each picture is kept in memory only while it is being read and is then discarded. Pictures and recognised text are never saved, never sent anywhere and never shared.
- PriceLens never taps, types, changes settings or does anything in other apps on your behalf.
- PriceLens shows its own disclosure and asks for your agreement before you turn the service on, and the service does nothing until you have agreed. You can switch it off at any time in Android's Accessibility settings, or pause it from the PriceLens Quick Settings tile.

### Location

- If you allow it, PriceLens uses your approximate location to work out which country (and, in the United States and Canada, which state or province) you are in. That tells it the local currency and the local sales tax. The lookup uses a map of borders built into the app; your location is never sent anywhere.
- Location is checked only when one of your selected camera apps opens, when you start live conversion or when you open PriceLens's settings (each time only if the last check is more than about 20 minutes old), or when you tap Refresh.
- PriceLens keeps its latest result (the country and the approximate position it came from) on your phone, replacing it at each check, and relies on it for at most 7 days.
- Without location access, PriceLens guesses the country from your mobile network's country code and your time zone, both read on your phone, or you can choose the currency yourself.

### Other information used on your phone only

- Installed apps: to let you choose which apps PriceLens works with, it lists the apps on your phone that have a launcher icon or can take pictures. The list is not stored or sent.
- Camera in use: PriceLens checks whether any app is currently using a camera (not what the camera sees), so the button only appears while the camera is on.
- Motion sensor: while live conversion is on, PriceLens reads the phone's gyroscope to keep labels steady as you move.
- Photos you pick: in the "Try it" preview you can choose one of your own photos to test with. It is read in memory on your phone and is not stored or sent.
- Settings: your choices (selected apps, currencies, display options) are stored on your phone. They are excluded from Android's cloud backup and device-to-device transfer.

## What leaves your phone

Only requests for public exchange-rate tables. PriceLens sends nothing else.

- When: when a selected camera app opens, when you start live conversion or when you open PriceLens's settings (each time only if the stored rates are at least 6 hours old or a new day's rates are out), or when you tap Refresh. After a failed attempt PriceLens waits between 15 minutes and 6 hours before trying again by itself.
- To whom: three public providers. Frankfurter (api.frankfurter.dev), ExchangeRate-API (open.er-api.com) and the fawazahmed0 currency API (cdn.jsdelivr.net and currency-api.pages.dev).
- What each request is: an encrypted (HTTPS) GET request for a fixed address that is the same for every user and returns the whole table of every currency against the US dollar. The addresses are https://api.frankfurter.dev/v2/rates?base=USD and https://open.er-api.com/v6/latest/USD and, for the fawazahmed0 currency API, https://cdn.jsdelivr.net/npm/@fawazahmed0/currency-api@DATE/v1/currencies/usd.min.json or https://latest.currency-api.pages.dev/v1/currencies/usd.min.json or https://DATE.currency-api.pages.dev/v1/currencies/usd.min.json, where DATE is today's or yesterday's date (UTC).
- What each request contains, in full: that address; the app's name and version, sent as "User-Agent: PriceLens/VERSION (Android)" where VERSION is the version you have installed (for example 0.1.7); the line "Accept: application/json"; the standard technical headers "Host", "Connection" and "Accept-Encoding: gzip"; and, when PriceLens asks again for a table it already has, the version markers ("If-None-Match" and "If-Modified-Since") that the same provider sent with that table, so an unchanged table is not downloaded twice.
- What no request contains: your location or country, the currencies you use, anything read from your screen, the apps you use, your phone's model or Android version, cookies, advertising or device identifiers, or any account.
- Like any internet request, each one shows the provider your device's IP address. Each provider may keep ordinary server logs under its own privacy policy. The developer of PriceLens runs no server and receives none of this.
- The usage reporting that ML Kit normally includes is switched off in PriceLens, so the app sends no recognition data or diagnostics to Google.
- If you have chosen to share usage and diagnostics data with Google in Android's settings, Android itself may send crash reports about PriceLens to Google, which shows them to the developer only in aggregate. That is controlled by your Android settings, not by PriceLens.

## Sharing

PriceLens does not sell, share or transfer any personal or sensitive data to anyone.

## Keeping and deleting data

- Screen pictures and recognised text: discarded immediately after reading, never stored.
- Stored on your phone: your settings, the latest country result and the downloaded exchange rates.
- To delete everything PriceLens has stored, open Android Settings > Apps > PriceLens > Storage and tap Clear storage, or uninstall PriceLens. The developer holds no data about you, so there is nothing to delete anywhere else.
- To stop location use, remove PriceLens's location permission in Android's settings.

## Children

PriceLens is a general travel and shopping utility. It is not directed at children and collects no data from anyone.

## Security

Exchange rates are downloaded over encrypted connections (HTTPS) only. Everything PriceLens stores stays in its private app storage on your phone.

## Changes to this policy

If this policy changes, the new version will be published at the address above and included in the next version of the app, with a new date at the top. If PriceLens ever needs to collect any data, it will tell you and ask first.

## Contact

Questions or requests: open an issue at https://github.com/SexualMoose/app-privacy/issues or email the developer address shown on the app's Google Play page.
