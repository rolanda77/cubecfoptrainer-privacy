# Legal notice and privacy policy – CFOP Trainer

[Deutsch (binding version)](README.md) · **English** · [Français](README.fr.md) · [Italiano](README.it.md) · [Español](README.es.md)

*Courtesy translation. In case of discrepancies, only the German version is binding.*

## Legal notice (Impressum)

Information pursuant to § 5 DDG (German Digital Services Act, formerly § 5 TMG):

Roland Albrecht
Im Jägeracker 42
79312 Emmendingen
Germany

Contact: rca@quantentunnel.de

## Privacy policy

Last updated: 18 October 2026

### 1. Controller

Roland Albrecht
E-mail: rca@quantentunnel.de

The person named above, as the developer of the app "CFOP/Fridrich-Algorithmen-Trainer" (hereinafter "the app"), is the controller within the meaning of the General Data Protection Regulation (GDPR) for the data processing described below.

### 2. Summary

The app does not collect, store or transmit **any personal data to the developer or to third parties**. There is:

- no user account and no sign-in,
- no internet connection (the app does not request the corresponding permission and does not communicate with any server),
- no analytics, tracking or advertising services (no Google Analytics, no crash reporting or ad SDKs),
- no sharing of data with third parties, simply because no data leaves the device.

All data created within the app remains exclusively local on the user's device. This also applies to the optional Bluetooth connection to a smart cube: it exists only directly between the device and the cube, without location access (section 5).

### 3. What data is stored locally on the device?

So that the app can provide its training functions (algorithm training, CFOP course, spaced-repetition reviews), it stores the following data **exclusively locally in a database on the respective device**:

- training and practice statistics per algorithm case (e.g. number of attempts, success rate),
- schedule/due-date data of the spaced-repetition reviews (date of the next due review per case),
- progress in the guided CFOP course (which levels/cases have already been unlocked or consolidated),
- custom move-sequence variants for individual algorithm cases saved by the user,
- the selected app language (German, English, French, Italian or Spanish) and other app settings (e.g. sticker look default, daily streak display),
- when a smart cube is used (section 5): name and Bluetooth address of the most recently connected cube together with the related settings (connect automatically, use the cube's orientation) and, for each practice attempt, whether it was performed by touch or with the smart cube.

Technically, this data is kept on the device in a local Room database (SQLite) and in local settings storage (SharedPreferences). This is not a transmission to the developer – nobody other than the person using the device has access to this data.

### 4. Backup function (local backup file)

In the settings menu, the app optionally lets you create a local backup file of the success statistics, the practice history including the schedule/due dates of the spaced-repetition reviews, the CFOP course progress, the favourite algorithm variants and the custom algorithms you saved, and to load a previously created backup file again. The file is saved to, or read from, a location chosen by the user exclusively via the file picker provided by the operating system – the app does not choose a location automatically and never transmits the file to the developer or to third parties. If the user chooses a cloud-synchronised folder as the location (e.g. a Drive or OneDrive integration on the device), further processing of this file is governed by the privacy policy of the respective cloud provider, not by that of this app.

### 5. Bluetooth connection to a smart cube (optional)

From Android 12 onwards, the app can optionally be connected to a Bluetooth-enabled puzzle cube ("smart cube", currently GAN i4 and GoCube) that reports the turns made on the cube to the app. The feature is voluntary; without it, the app remains fully usable by touch.

- **Local connection only:** The app searches for smart cubes nearby via Bluetooth Low Energy and connects directly to the selected cube. No server, no manufacturer account and no internet connection is involved.
- **Data processed:** From the cube, the app receives only move events (which face was turned in which direction, with a timestamp), orientation events (the cube's orientation in space), the battery level as well as the device name, model and hardware information. This data is used only for the current exercise; of it, only the usual training data from section 3 is stored (move sequence, time and rating of an attempt, plus the input source).
- **Saved cube:** So that the app can reconnect to the same cube on the next start, it stores the cube's name and Bluetooth address locally on the device. This entry can be deleted at any time via "Remove" in the smart cube menu. This information is not part of the backup file (section 4).
- **No location access:** For this, the app uses only the "Nearby devices" permission (section 8) and explicitly declares to the system that it does not derive a location from the Bluetooth scan. Other Bluetooth devices found are neither displayed nor stored.
- **No transmission:** Neither the cube data nor the saved Bluetooth address leaves the device.

### 6. No data transmission, no server, no account

The app neither needs nor has permission to access the internet. Consequently, at no time does the app itself transmit data to the developer, to Google or to any other third party. There is no user account, no registration and no cloud synchronisation.

### 7. No analytics, tracking or advertising services

The app contains no analytics software (e.g. Firebase Analytics), no crash reporting services (e.g. Crashlytics) and no advertising SDKs. No usage profiles are created, no location is determined and no advertising ID is read.

### 8. App permissions

The app does not request any special device access permissions (e.g. no access to the camera, location, contacts, microphone or internet) – with one exception: for the optional smart cube connection (section 5), it uses the "Nearby devices" permission from Android 12 onwards (`BLUETOOTH_SCAN` with the declaration that no location is derived, and `BLUETOOTH_CONNECT`). It is requested only when the user searches for a cube or connects in the smart cube menu, and it can be revoked at any time in the Android settings; the rest of the app works without it as well. The backup function (section 4) uses the system's own file picker (Storage Access Framework), which does not require any additional permission.

### 9. Storage period and deletion

The data listed in section 3 remains stored locally on the device until it is:

- reset using the functions built into the app (e.g. "Reset statistics" or "Delete own algorithms" in the settings menu), or
- completely removed from the device by uninstalling the app.

The saved smart cube (section 5) can additionally be deleted at any time via "Remove" in the smart cube menu.

Since no data is stored outside the device, no further copy of the data remains after the app has been uninstalled – with the exception of a backup file created by the user (section 4), which remains at its chosen location independently of the app and can be deleted by the user if required.

### 10. Rights of the data subject

Since the app does not transmit any personal data to the developer, all data listed in section 3 is exclusively within the direct access and under the full control of the user (access, rectification and erasure take place directly via the app or by uninstalling it). Nevertheless, the contact given in section 1 can be used at any time for questions about data protection in relation to the app.

### 11. Minors

The app is not specifically aimed at children and does not collect any personal data, regardless of the user's age.

### 12. Changes to this privacy policy

This privacy policy may be amended if necessary, for example if new app features require an update. The current version is always available at the address linked in the Play Store listing.

### 13. Contact

If you have any questions about this privacy policy or the app, please contact:

rca@quantentunnel.de
