---
title: OpenCube privacy policy
---

# OpenCube privacy policy

Last updated: 13 November 2026

OpenCube is published by the OpenCube developer. This policy describes what the OpenCube app for Android, as
distributed on Google Play, does with your data. OpenCube is an app for one Wi-Fi 360° cube camera: it works with
the SooCoo Cube 360 / GVT-360i, and it is unofficial and not affiliated with the camera's maker. The current
version of this policy is published at https://sexualmoose.github.io/app-privacy/opencube/ and a copy is built
into the app (Settings > About > Privacy policy), where it reads without a network connection.

## In short

- OpenCube collects no personal data. Nothing is sent to the developer or to anyone else.
- It has no accounts, ads, analytics, crash reporting or tracking.
- It never connects to the internet. It talks only to your camera, over the camera's own Wi-Fi.

## What OpenCube handles, and where it stays

- **Your camera.** OpenCube joins the camera's Wi-Fi network and talks only to the camera at 192.168.0.1:
  commands and settings, the live video, and the files on its memory card. This traffic goes between your phone
  and the camera and nowhere else.
- **Videos and photos.** Clips you download from the camera, recordings made on the phone, 360° exports and
  snapshots are kept in OpenCube's own storage on your phone. They leave it only when you choose Save to Gallery
  (they are copied to Movies/OpenCube or Pictures/OpenCube) or Share (you pick the app that receives them).
- **Settings.** The camera's Wi-Fi name, your viewing and picture choices and the camera's lens calibration are
  stored on your phone.
- **The camera's Wi-Fi password.** If you set one in OpenCube, it is stored on your phone encrypted with a key held
  in Android Keystore, used only to rejoin the camera, and sent only to the camera when you set it.
- **Camera details** shown in Settings (model, firmware version, serial number) are read from the camera when you
  connect. They are not stored or sent anywhere.
- **The time.** OpenCube sets the camera's clock from your phone's date and time (when it connects, unless you
  switch that off, or when you tap it in Settings), so the camera's recordings carry the right time.

## Permissions

- **Nearby Wi-Fi devices** (Android 13 and later): to find and join the camera's Wi-Fi. OpenCube declares to
  Android that it never uses this to work out your location, and it asks for no location permission.
- **Notifications:** to show download progress.
- **Network access and Wi-Fi state:** to join the camera's network and talk to the camera. OpenCube uses network
  access only on the camera's own Wi-Fi.
- **Foreground service (data sync), run at startup and prevent sleep:** to keep a download you started running
  after you leave the app, and to keep track of one that was interrupted.

OpenCube asks for no location, storage, contacts, camera, microphone or account permissions.

## Sharing and selling

OpenCube does not sell data and does not share data with anyone.

## Security

The camera's Wi-Fi password is encrypted on your phone (AES-256-GCM, with a key that never leaves Android
Keystore). OpenCube's files and settings are in its own app storage. The camera only supports unencrypted
connections, and its Wi-Fi is open until you set a password for it; OpenCube lets you set one, and its Settings
show when the camera's network is open.

## Backups, retention and deletion

OpenCube's data is left out of Android cloud backups and device-to-device transfers. Everything stays on your
phone until you delete it:

- delete individual files in OpenCube's Library;
- remove all of OpenCube's data in Android Settings > Apps > OpenCube > Storage > Clear storage;
- or uninstall OpenCube. Copies you saved to your Gallery stay there until you delete them.

Recordings on the camera's memory card stay on the card until you delete them or format the card.

## Children

OpenCube is not directed at children and is not designed for them.

## Changes

Changes to this policy are published at the address above with a new "Last updated" date.

## Contact

Questions or requests: open an issue at https://github.com/SexualMoose/app-privacy/issues or email the developer address shown on the app's Google Play page.
