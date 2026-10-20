# Privacy Policy for Aura TV

**Last Updated:** October 20, 2026

Aura TV ("we", "us", or "our") respects your privacy. This Privacy Policy describes how your information is handled when you use the Aura TV application for **iOS, iPadOS, and tvOS** (the "App").

---

## 1. Summary — Privacy First

Aura TV is designed from the ground up to protect your privacy:

* **Zero Tracking:** We do not track you, build behavioral profiles, or include third-party advertising SDKs.
* **No Accounts Required:** You do not need to create an Aura TV account or provide an email address to use the App.
* **Your Credentials Stay Yours:** Your playlist server URLs, usernames, and passwords are stored securely on your device and are never transmitted to us or any third-party analytics servers.
* **Direct Connections Only:** The App connects directly to the IPTV streaming providers and servers that you configure.

---

## 2. Information We Handle and How It Is Used

### A. Playlist Configuration and Credentials
* **What is handled:** Server URLs, M3U/M3U8 playlist addresses, XMLTV EPG links, usernames, and passwords entered by you.
* **Storage:** Stored locally on your device within the App’s sandboxed SQLite database and local preferences.
* **Transmission:** Transmitted directly and exclusively to your configured IPTV streaming server or provider to authenticate your subscription, fetch channel manifests, and stream media. We do not operate intermediary proxy servers or store your credentials on our own servers.

### B. Optional Apple iCloud Synchronization
* **Functionality:** If you enable iCloud Sync, your playlist metadata, favorite channels, and watch progress synchronize across your Apple devices (iPhone, iPad, Apple TV).
* **Security:** Synchronization operates through Apple's native iCloud Key-Value Store (`NSUbiquitousKeyValueStore`). All sync data is encrypted in transit and at rest within your personal Apple iCloud account.
* **Access:** Only you and your authenticated Apple ID have access to this synchronized data. The developers of Aura TV have no access to your iCloud sync payloads.

### C. Viewing History and Offline Storage
* **Watch Progress:** Resume positions, Continue Watching states, and playback history are stored locally in the App’s on-device SQLite database to provide seamless multi-room resume.
* **Downloads (iOS):** Downloaded video files are saved exclusively to your device's local application storage for offline playback. You can delete downloads at any time from the Downloads & History settings screen.

### D. Third-Party Metadata and Public APIs
To provide rich poster artwork, synopsis details, and sports schedules, the App queries public APIs:
* **The Movie Database (TMDB):** The App queries TMDB for movie and TV series metadata and poster artwork using sanitized titles. No personal identifying information or credentials are sent to TMDB.
  * *Attribution Notice:* This product uses the TMDB API but is not endorsed or certified by TMDB.
* **Sports Scoreboard APIs (ESPN, TheSportsDB):** The App queries public scoreboard feeds to display match fixtures, kick-off times, and live scores. These requests are anonymous public HTTP/HTTPS queries.

### E. Local Network and AirPlay Remuxing (iOS)
* **Local Network Usage:** The iOS App utilizes local networking (`NWListener`) solely to cast transcoded/remuxed video streams to your Apple TV or AirPlay-compatible receivers on your local home Wi-Fi network. No media or network data is transmitted outside your local area network.

---

## 3. Data Retention and Deletion

* **In-App Deletion:** You can delete any playlist at any time by tapping **Settings → Delete Playlist**. This instantly and permanently purges the playlist, credentials, and associated catalog from your device.
* **Clear Cache:** You can clear cached posters, EPG data, and artwork from the in-app Settings menu at any time.
* **App Uninstallation:** Deleting the App from your Apple device completely removes all local sandboxed storage, databases, and preferences.

---

## 4. Third-Party Links and User Content Disclaimer

Aura TV is a generic media player client. The App does not bundle, pre-load, host, or distribute any media streams, channels, or playlists:
* Users must supply their own legally obtained M3U playlists or Xtream Codes subscriptions.
* We do not endorse, facilitate, or condone the unauthorized streaming of copyrighted material.
* Content streamed through user-provided links is governed by the terms and privacy practices of the respective third-party streaming providers.

---

## 5. Children's Privacy

Aura TV does not knowingly collect or solicit any personal information from children under the age of 13. The App includes an optional **Adult Content Filter** to hide adult categories and streams when configured by the user.

---

## 6. App Store Privacy Declarations

In compliance with Apple's App Store Privacy Requirements (Apple Privacy Manifest):

| Category | Declaration | Reason |
|---|---|---|
| **Tracking** | `NSPrivacyTracking: false` | No tracking across apps or websites. |
| **Data Collection** | None collected by developer | All data stays on-device or within your private iCloud account. |
| **UserDefaults API** | Reason `CA92.1` | Used strictly to read and write in-app preferences within the App container. |
| **File Timestamp API** | Reason `C617.1` | Used strictly to verify local SQLite database and cache file modification dates. |
| **Disk Space API** | Reason `E174.1` | Used strictly to check available storage before saving offline downloads or database chunks. |

---

## 7. Changes to This Privacy Policy

We may update this Privacy Policy from time to time. Any revisions will be reflected with an updated "Last Updated" date at the top of this document and made accessible within the App settings.

---

## 8. Contact Information

If you have any questions or feedback regarding this Privacy Policy, please contact us:

* **email:** pgvd.nagendra@gmail.com
