---
layout: page
title: Kinkred — Privacy Policy
permalink: /kinkred/privacy/
---

**Effective date:** 2026-10-31

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
  Bluetooth and/or Wi-Fi. You confirm a matching 4-digit code once, when
  you first pair; after that the two phones sync automatically whenever
  both are nearby with the app open. Nothing is ever sent to a server.
- If you choose to send us feedback or a bug report, the App only
  prepares an email; **your own email app sends it**, and only what you
  choose to include. See "Feedback and bug reports" below.

## Data we process

All of the following is processed entirely on your device:

- **Profile information** you create: display name, avatar image (if
  provided), and kink preference ratings.
- **Partner information** you receive from a peer via Nearby
  Connections: their display name, avatar (if shared), and kink
  preference ratings.
- **Activities** you plan and complete: date, partner (if any), notes,
  per-kink ratings, and overall ratings.
- **App security data**: if you set a PIN (it is optional), a PBKDF2
  hash of it and a random salt, plus a boolean preference indicating
  whether biometric unlock is enabled. A boolean preference also records
  whether you have answered the optional "set up a PIN?" prompt.

## Data we do not process

- We do not collect personally identifying information server-side —
  because we do not operate any server.
- We do not use analytics or crash reporting SDKs.
- We do not include advertising SDKs.
- We do not read your contacts, SMS, location history, or browsing
  data.

## Permissions the App requests and why

- **Bluetooth (scan, advertise, connect)** and **Nearby Wi-Fi Devices**:
  used only by Google Nearby Connections to discover paired partners'
  phones and sync profile and activity data peer-to-peer. Data is
  exchanged only with a device you have explicitly paired with.
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

## Nearby Connections — pairing and automatic sync

**Pairing (one time).** To link with a partner, both phones advertise
and discover each other over Google Nearby Connections and display the
same 4-digit code. You visually verify the codes match and tap "Pair" on
both phones. Pairing establishes a shared secret the two phones keep — it
is your explicit, ongoing consent to sync with that partner.

**Automatic sync (after pairing).** Once paired, whenever both phones are
near each other with Kinkred open, they re-authenticate using that shared
secret (no code, no tap) and exchange data automatically:

- your profile snapshot — display name, avatar, kink ratings;
- locked activities you have with that partner, and each side's per-kink
  ratings of them.

Sync runs only while the app is open in the foreground — there is no
background service. It remains **strictly peer-to-peer**: data goes only
between the two paired phones, never to a server. You can pause auto-sync
for any partner, or unlink them entirely, at any time. Previous partners,
unrelated data, and app settings are never shared.

## Feedback and bug reports

If you choose to send feedback or report a bug (the small feedback
button shown on the App's screens, or Settings → Help → Send feedback or
report a bug), Kinkred prepares a message and opens **your own email
app**. The App sends nothing itself, and nothing is sent until you press
Send in your email app. You can read, edit, or remove anything before
sending.

Besides your description, you can choose to include the following. Every
option starts switched off; nothing extra is added unless you tick it.

- **Device info:** app version, Android version, device manufacturer and
  model, and language.
- **Anonymized app details:** counts and settings only (for example the
  number of rated kinks or partners, or whether background sync is on).
  Names, notes, photos, individual ratings, and identifiers are never
  included.
- **Screenshots:** when you tap the feedback button, Kinkred captures the
  App screen you were on (only Kinkred's own content, nothing else on
  your phone) and shows it to you; it's attached only if you tick it. You
  can also add screenshots from your gallery. Tap any screenshot to cover
  names or anything private with black bars; covered areas are removed
  from the image itself, not just hidden. Screenshots are resized and
  re-encoded on your device, which removes metadata such as location, but
  they can't be anonymized automatically: they show whatever was on
  screen, so please check them before sending.

We receive your message like any email, so it includes your email
address. We use it only to look into your report and reply to you, and
we don't combine it with any other data, because we don't have any. If
you prefer, you can send from a separate or throwaway email address; that
doesn't affect how we handle your report. Your email provider handles the
message under its own privacy policy. We delete reports once they're
resolved, or sooner on request at universedevel.help@outlook.com.

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

- A PIN lock is optional. You can set one up, change it, or remove it
  at any time in Settings → Security. Without a PIN, the App opens
  without a lock screen.
- If you set a PIN, it is stored as a **PBKDF2-HMAC-SHA256** hash with a
  per-profile random salt and 120,000 iterations; removing the PIN
  deletes the hash and salt.
- Biometric unlock is a convenience alternative to entering the PIN;
  the PIN remains available at all times.
- While a PIN is set, the App locks automatically after a configurable
  interval of inactivity (default: 5 minutes), and can be locked
  manually from the home screen.
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
