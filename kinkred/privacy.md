---
layout: page
title: Kinkred — Privacy Policy
permalink: /kinkred/privacy/
---

**Effective date:** 2026-05-17

**Applies to:** the Kinkred Android application ("the App") published by
Universe Devel team ("we", "us").

## Summary

- The App is **local-first**. All of your data — profiles, ratings,
  partners, activities, notes, and any photos you add — is stored on
  your device.
- We do **not** operate a server for your data, and we never collect,
  receive, or transmit it. (The App does download one small public file
  — an affiliate shop catalogue — from our website; that request sends
  nothing about you. See "Affiliate links and the shop catalogue" below.)
- The App has **no third-party analytics, tracking, or advertising
  SDKs**.
- Pairing with a partner uses **Google Nearby Connections** — a direct
  peer-to-peer channel between your phone and your partner's phone over
  Bluetooth and/or Wi-Fi. Your data is exchanged only with that peer
  after you both visually confirm a matching 4-digit code.

## Data we process

All of the following is processed entirely on your device:

- **Profile information** you create: display name, avatar image (if
  provided), and kink preference ratings.
- **Partner information** you receive from a peer via Nearby
  Connections: their display name, avatar (if shared), and kink
  preference ratings.
- **Activities** you plan and complete: date, partner (if any), notes,
  per-kink ratings, and overall ratings.
- **App security data**: a PBKDF2 hash of your PIN and a random salt,
  plus a boolean preference indicating whether biometric unlock is
  enabled.

## Data we do not process

- We do not collect personally identifying information server-side —
  because we do not operate any server.
- We do not use analytics or crash reporting SDKs.
- We do not include advertising SDKs.
- We do not read your contacts, SMS, location history, or browsing
  data.

## Permissions the App requests and why

- **Bluetooth (scan, advertise, connect)** and **Nearby Wi-Fi Devices**:
  used only by Google Nearby Connections to discover and pair with a
  partner's phone for profile and activity sharing. No data is
  transmitted before both users visually confirm a matching auth code.
- **Location (legacy Android <= 11 only)**: required by the Android
  platform for Bluetooth scanning on older OS versions. Kinkred does
  not use or store your location.
- **Post notifications (Android 13+)**: used to show reminders for
  activities you have planned. You can decline this permission at any
  time.
- **Internet**: used only to download the public affiliate shop
  catalogue described under "Affiliate links and the shop catalogue".
  No personal data is sent.

## Media and photo selection

When you choose an avatar, Kinkred uses Android's photo picker. The
selected image is resized locally and stored in the App's private
database; the original photo is not uploaded anywhere.

## Nearby Connections — what is shared and when

When you pair with a partner:

1. Both devices advertise and discover each other over the Google
   Nearby Connections service.
2. Before any data is exchanged, both devices display the same 4-digit
   authentication code. You must visually verify the codes match and
   tap "Match" on both phones.
3. Only after both confirm does each side send the current profile's
   snapshot (display name, avatar bytes, ratings) to the other.
4. During an activity-planning session, edits to the shared draft are
   exchanged in real time between the two paired phones. Nothing is
   persisted on either phone until both users confirm.

The data exchanged is limited to the current profile snapshot and the
activity draft. Previous partners, unrelated profiles, and app
settings are never shared.

## Backup and restore

The App can export all of its local data to a file through Android's
Storage Access Framework. You choose the destination (for example, your
device's Downloads folder or a cloud folder you have already connected).
The App does not write to the cloud itself.

Every exported backup file is **encrypted** (AES-256-GCM). You may set a
password when exporting; if you leave it blank the file is still
encrypted, so your data is never written out as readable text.
"Restore from backup" lets you pick a backup file previously exported
from the App — entering its password if one was set — and replaces the
current local data with its contents.

## Affiliate links and the shop catalogue

Some kinks show an optional "shop the gear" link to an external
retailer. These are **affiliate links** — if you buy something after
following one, we may earn a small commission, at no extra cost to you.
Following a link opens your normal web browser; what you do on the
retailer's site is governed by that retailer's own privacy policy.

To keep those links current, the App periodically downloads a small
public catalogue file from our website. That request is an ordinary web
download and includes **no information about you or your data**. If it
fails, or you are offline, the App uses the last copy it had — or shows
no shop links at all.

## Security

- Your PIN is stored as a **PBKDF2-HMAC-SHA256** hash with a
  per-profile random salt and 120,000 iterations.
- Biometric unlock is a convenience alternative to entering the PIN;
  the PIN remains available at all times.
- The App locks automatically after a configurable interval of
  inactivity (default: 5 minutes), and can be locked manually from the
  Profiles screen.
- Data is persisted in the App's private storage sandbox, which is not
  readable by other apps on a non-rooted device.

## Children

Kinkred is intended for **adults only (18 years of age or older)**.
The App presents a consent gate on first launch requiring an adult
affirmation. We do not knowingly process data from anyone under 18.

## Your rights

Because your data stays on your device:

- You can view, edit, or delete any entry at any time through the App.
- You can delete a profile, a partner, an activity, or a rating.
- You can uninstall the App to remove all local data.
- You can export a full backup or restore from one at any time.

We cannot delete data on your behalf because we do not have it.

## Changes to this policy

If we change this policy, the updated version will be included in a
subsequent release of the App and hosted at the same URL provided in
the Play Store listing. The "Effective date" at the top will be
updated.

## Contact

Questions about this policy: **universedevel.help@outlook.com**
