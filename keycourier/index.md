---
title: KeyCourier privacy policy
---

# KeyCourier privacy policy

Last updated: 13 November 2026

KeyCourier is published by the KeyCourier developer. This policy describes what the KeyCourier app
for Android, as distributed on Google Play, does with your data. The current version is published at
https://sexualmoose.github.io/app-privacy/keycourier/ and a copy is built into the app (Settings,
Privacy policy).

## In short

- Everything you put into KeyCourier stays on your phone. The app has no internet access: it does
  not include Android's Internet permission, so it cannot send anything to the developer or to any
  other online service.
- There are no accounts, ads, analytics or tracking, and no third-party code that collects data.
- The developer never receives your passwords or any other data from the app.

## What the app stores on your phone

- **Your vault:** the devices you add (a name, an icon and the Bluetooth address and name of the
  computer you paired), your logins and their steps (including the usernames, passwords and other
  values you type into them), and your NFC tags and which logins they start. The vault is encrypted
  with AES-256-GCM using a key kept in your phone's Android Keystore (in secure hardware where the
  phone has it). The key cannot be used while your phone is locked.
- **Preferences:** settings such as the re-lock delay, the unlock method and which login the Quick
  Settings tile sends. They contain no passwords and are kept in the app's private storage.
- **Bluetooth self-repair record:** if you turn on the optional Bluetooth self-repair (see
  Permissions), the app briefly keeps a note of the radio settings it must put back.

All of this is excluded from Android cloud backup and from device-to-device transfer.

## What leaves your phone

- **Typing into your computer.** When you send a login, KeyCourier acts as a Bluetooth keyboard and
  types it into the computer you paired your phone with. The keystrokes go only to that computer,
  over the Bluetooth connection you set up.
- **Export files, only when you ask.** "Transfer / migrate" saves your vault to a file at a place
  you choose. The file is encrypted with a passphrase you pick (AES-256-GCM, key derived with
  PBKDF2-HMAC-SHA256). Anyone who has both the file and the passphrase can open it, so keep them
  apart and safe.
- **Crash statistics from Google, only if you opted in.** KeyCourier itself reports nothing. If you
  have chosen on your phone to share usage and diagnostics data with Google, Google Play may show
  the developer crash and performance reports for the app. Android and Google Play do this, not
  KeyCourier, under Google's privacy policy.
- Nothing else. The app sends no data to the developer or to any third party.

## Notification access (optional)

A "wait for code" step can type a one-time sign-in code that arrives by SMS or email. This only
works if you turn on Notification access for KeyCourier in Android's settings; the app explains
what it does and asks you first. With access on, KeyCourier reads the text of incoming
notifications on your phone to find the code. Recent notification text is kept only in the app's
memory, for about one minute, and is cleared after each send. It is never saved to storage and
never sent anywhere; only the code itself is typed into your paired computer. The code it typed is
kept in memory for up to two minutes, so you can send it again if it didn't arrive, and is then
forgotten. After typing a code, KeyCourier dismisses the notification it came from. You can turn
Notification access off at any time in Android's settings.

## NFC tags (optional)

A tag written by KeyCourier holds only a random identifier, never a login, name or password. The
link between a tag and a login is stored in your encrypted vault. An existing tag or card you
register is recognized by its serial number, which is also stored only in the vault.

## Permissions

- **Nearby devices / Bluetooth:** to act as a Bluetooth keyboard, to make your phone visible for
  pairing and to connect to your paired computers.
- **NFC:** to read and write KeyCourier tags.
- **Biometric:** to unlock the app with your fingerprint, face or screen lock.
- **Run at startup:** used only by the optional Bluetooth self-repair, to finish putting a radio
  setting back if the phone restarted in the middle of a repair.
- **Modify secure system settings:** never granted by installing the app. Only if you grant it
  yourself, from a computer with Android's adb tool, can KeyCourier restart Bluetooth when the
  phone's Bluetooth keyboard service gets stuck. It does so by switching a radio mode on for a few
  seconds and then back to how it was.

## Retention and deletion

Your data stays on your phone until you delete it in the app or uninstall the app. Uninstalling
deletes the vault, your preferences and the encryption key. Because the developer holds no copy of
your data, there is nothing for the developer to delete on request.

## Children

KeyCourier is not directed at children.

## Changes to this policy

If this policy changes, the new version is published at the address above and in the next version
of the app, with a new "Last updated" date.

## Contact

Questions or requests: open an issue at https://github.com/SexualMoose/app-privacy/issues or email the developer address shown on the app's Google Play page.
