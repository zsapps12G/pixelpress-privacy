# Privacy Policy — PixelPress

**Developer:** ZS Apps  
**Contact:** indiedev71@gmail.com  
**Effective date:** 2026-05-06  
**Applies to:** PixelPress for Android, version 1.0.0 and above

---

## The short version

PixelPress does not collect, transmit, or share any data about you or your photos. Everything happens on your device. Nothing leaves your phone.

The longer version below explains exactly what the app does and does not do, so you can verify it for yourself.

---

## 1. What the app accesses

**Your photos — only when you choose them.**

When you tap "Convert a Photo" or "Convert Multiple", the app opens the Android system photo picker. You select the photos you want to compress or convert. The app reads those photos into memory solely to perform the compression or conversion you requested.

The app does not browse your photo library in the background. It does not access photos you have not explicitly selected.

---

## 2. What is stored on your device

PixelPress stores two types of data locally on your device using Android's standard SharedPreferences storage. This data never leaves your device.

**Compression history**  
After each successful conversion, the app saves a record containing:
- The original file's name (e.g., `IMG_0042.HEIC`)
- The output format you chose (JPG, PNG, or WebP)
- The original file size in bytes
- The compressed file size in bytes
- The quality setting you used (0–100)
- The date and time of the conversion

This is the data shown in the History screen. The history is capped at 200 entries. You can delete it at any time: open History → tap the menu (⋮) → Clear all.

**Settings**  
The app remembers your preferred default output format and default quality level so you do not have to reset them each time. These two values are stored locally and are not linked to any account or identity.

**Temporary files**  
During compression, the app writes the output file to Android's temporary directory (`getCacheDir`). This is managed by the operating system. The file is accessible to you only through the Save to Gallery or Share actions. It is not stored permanently by the app.

---

## 3. What is NOT collected, transmitted, or shared

The following is an explicit list of things PixelPress does not do:

- Does not send any data to any server
- Does not use any analytics or crash-reporting service (no Firebase, no Crashlytics, no Sentry, no similar tools in v1.0)
- Does not display advertisements (no AdMob or any other ad network in v1.0)
- Does not require or create a user account
- Does not collect your name, email address, or any personal identifier
- Does not read your device's advertising ID, IMEI, or any unique hardware identifier
- Does not access your location
- Does not access your camera
- Does not access your contacts or call logs
- Does not access your microphone
- Does not send push notifications
- Does not share anything with third parties

The app has no INTERNET permission. It is technically incapable of making a network connection.

---

## 4. Permissions and why the app needs them

| Permission | Android version | Why it is needed |
|---|---|---|
| `READ_MEDIA_IMAGES` | Android 13 and above | To read the photos you select from the system picker |
| `READ_EXTERNAL_STORAGE` | Android 12 and below | Same purpose on older Android versions |
| `WRITE_EXTERNAL_STORAGE` | Android 9 and below | To save the compressed output to your gallery on very old Android versions |

The app does not request any other permissions — not camera, location, microphone, contacts, notifications, or advertising ID.

---

## 5. Third-party open-source libraries

PixelPress uses the following open-source packages. All processing happens on your device. None of these libraries transmit data off your device.

| Library | Purpose |
|---|---|
| `flutter_image_compress` | Performs image compression and HEIC conversion on-device |
| `image_picker` | Presents the Android system photo picker |
| `gal` | Saves the compressed output to your gallery via Android's MediaStore API |
| `share_plus` | Opens the Android system share sheet so you can send the file to another app |
| `url_launcher` | Opens links (Privacy Policy, Play Store) in your device's browser — the app itself makes no network call |
| `shared_preferences` | Stores history and settings locally on your device |
| `path_provider` / `path` | Resolves file paths on-device — no network involvement |

---

## 6. Children's privacy

PixelPress is a general-purpose utility app. It is not directed at children under the age of 13 and does not knowingly collect personal information from anyone, including children. Given that the app collects no data at all, there is no special handling required — but we confirm explicitly that no children's data is collected or processed.

---

## 7. Your rights

Because PixelPress stores data only locally on your device, you have full control:

- **Delete history:** History → ⋮ → Clear all
- **Delete everything:** Uninstall the app. Android removes all app data, including SharedPreferences, on uninstall.

There is no server-side data to request deletion of, because no data is ever sent to a server.

---

## 8. Future versions

PixelPress v1.0 has no advertising and no analytics. Future versions (v1.1 onwards) may introduce Google AdMob banner ads and optional analytics. If that happens:

- This privacy policy will be updated to accurately describe what is collected and shared
- The update will be published at this URL before the new version is released
- The "Effective date" at the top of this page will be updated
- The Data Safety section in the Google Play listing will be updated to match

We will not add any data-collection feature without updating this policy first.

---

## 9. Changes to this policy

If this policy changes, the revised version will be published at this same URL with an updated effective date. Continued use of the app after a policy update constitutes acceptance of the updated policy. For material changes, we will note what changed and when.

---

## 10. Jurisdiction and applicable law

ZS Apps is based in Melbourne, Victoria, Australia. This policy is written to comply with the Australian Privacy Act 1988 (Privacy Act).

If you are located in the European Economic Area, you have rights under the General Data Protection Regulation (GDPR). If you are located in California, USA, you have rights under the California Consumer Privacy Act (CCPA). Because PixelPress collects no personal data, no special action is required on our part under these laws — but we acknowledge them and will comply fully with any valid data request.

---

## 11. Contact

For any privacy-related questions or concerns:

**Email:** indiedev71@gmail.com  
**Subject line:** PixelPress Privacy

We aim to respond within 5 business days.
