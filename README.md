# Cava Reader — downloads

**This repository only holds Cava Reader's releases.** There is no source code here. It exists so
that anyone can download the app and, more importantly, keep it updated without the Play Store.

Android 8.0 or newer. The app is signed with the same key as the Google Play build, so a download
from here and an install from Play are interchangeable.

Current release: **1.0.0-pre6**.

---

## Install and keep it updated (read this bit)

Set this up once and Cava Reader updates itself from then on. Without it you have to come back here
and download a new file every time, which is the thing most people forget to do.

We use **[Obtainium](https://github.com/ImranR98/Obtainium)**, a small open-source app that watches
a releases page and installs each new version for you. It is the same idea as a store, except the
"store" is this repository.

1. **Install Obtainium.** It is on
   [GitHub](https://github.com/ImranR98/Obtainium/releases) and
   [F-Droid](https://f-droid.org/packages/dev.imranr.obtainium.fdroid/). Either is fine.
2. **Open Obtainium and tap "Add App".**
3. **Paste this repository's address:**

   ```
   https://github.com/cava-reader/releases
   ```

4. **Tap "Add".** Obtainium reads the releases here, works out which build matches your device, and
   shows you the latest version. Tap install.
5. **Leave "Auto update" switched on** if you want new versions installed for you, or off if you
   would rather be asked each time. Either way you get a notification when a release appears.

That is the whole of it. You never have to know whether your phone is arm64, and you will never have
to remember to check back here.

> **If you are reading this while the repository is private**, Obtainium cannot read it, so use the
> manual route below instead. This page is written for the repository being public.

### Or install by hand

Open the [latest release](../../releases/latest) and tap the APK that matches your device:

| File | For |
| --- | --- |
| `CavaReader-<version>-arm64-v8a.apk` | Almost every phone and tablet made since about 2016. **Pick this one if you are unsure.** |
| `CavaReader-<version>-armeabi-v7a.apk` | Older 32-bit devices. |
| `CavaReader-<version>-x86_64.apk` | Emulators and some Chromebooks. |
| `CavaReader-<version>-universal.apk` | Works anywhere. About twice the size, because it carries every architecture. |

Android will ask you to allow installs from your browser or file manager the first time. That prompt
is normal for any app that does not come from a store.

To update by hand, download the newer APK from the newer release and install it over the top. Your
library, your place in every book, and Full all survive an update.

---

## Cava Reader Full

Everything in Cava Reader is free: reading, listening, and the whole Public Domain library with read
along included. **Cava Reader Full** is the one thing that costs money, and it is a one-time
purchase with no subscription. It keeps read along switched on for the books you bring yourself,
past the four free hours.

There are two ways to buy it, and you can use either one regardless of how you installed the app.

### Buying it on our website (works without any Google account)

Go to **[cavareader.app/get](https://cavareader.app/get)**. You get a **licence key** by email
within a minute or two.

Then, in the app:

1. Open the **Full** screen (Settings → About → *Get Cava Reader Full*, or the button any time the
   app mentions the free hours).
2. Tap **"Bought on our website? Enter your licence key"**.
3. Paste the key in and tap **Activate**.

Read along on your own books turns on for good. No Google account, no Play Store, and no Play
services are needed at any point.

### Buying it on Google Play

If your device has Play, you can also buy it from the **Full** screen in the app, and Play handles
it. Play uses your local currency, and the purchase follows your Google account, so a new phone gets
it back by itself.

### Already bought it, and moving to a new device?

**A licence key works on one device at a time.** To move it to a new phone:

1. On the **old** device, open Settings → About and use the licence section to release it, or follow
   the "manage your licence" link in your purchase email. If the old device is lost or broken, use
   the link in the email; that is exactly what it is for.
2. Install Cava Reader on the **new** device and enter the same key, as above.

Nothing is charged again. A Google Play purchase has no such limit, which is the one practical
reason to prefer Play when your device has it.

**Lost your key?** Look for the email from our store. If you cannot find it, write to the support
address on your receipt.

---

## Verifying a download

Every APK here is signed with Cava Reader's release key, the same one the Play listing uses. To
check one you have:

```bash
apksigner verify --print-certs CavaReader-1.0.0-pre6-arm64-v8a.apk
```

The certificate's SHA-256 digest is the same for every release in this repository and for the Play
build. If a file you downloaded shows a different one, it did not come from us. Delete it.

---

## Questions

- **Something wrong with the app?** Use the
  [issue tracker](https://github.com/cava-reader/bug-tracker).
- **Something wrong with a purchase?** Write to the support address on your receipt.
- **Privacy, or anything else?** See [cavareader.app](https://cavareader.app); the privacy policy is
  a short one and worth reading.

*Cava Reader is an independent app. This repository contains no source code, no build scripts and no
credentials, only what you install.*