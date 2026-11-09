# Privacy Policy for AQI Now

**Last Updated: November 9, 2026**  
**Effective Date: November 9, 2026**

**Application Name:** AQI Now  
**Package Name:** `com.mylocalaqi.app`  
**Developer / Operating Entity:** Excel Technologies India ("we," "us," or "our")  
**Contact Email:** [exceltechnologiesindia@gmail.com](mailto:exceltechnologiesindia@gmail.com)  
**Official Policy URL:** [https://anupamkhurana.github.io/AQINow/](https://anupamkhurana.github.io/AQINow/)

---

## 1. Introduction & Core Privacy Principles

Excel Technologies India operates the **AQI Now** mobile application (the "App"). We are committed to protecting your privacy and ensuring transparency regarding how data is handled. This Privacy Policy is tailored specifically to comply with **Google Play Developer Program Policies** (including the Location Permissions Policy and Data Safety requirements) as well as applicable data protection laws (such as GDPR and CCPA).

### Our Core Privacy Commitments:
- **No User Accounts:** You can use AQI Now without registering, logging in, or creating an account. We do not collect names, phone numbers, or email addresses.
- **No Advertisements:** AQI Now contains no third-party advertisements, banner ads, interstitial ads, or ad-tracking SDKs.
- **No Sale of Data:** We do not sell, rent, monetize, or trade your personal or location data to data brokers, advertisers, or any third party.
- **Data Minimization:** We collect and process only the minimal technical data strictly necessary to provide live air quality indices and health recommendations.

---

## 2. Location Information & Google Play Disclosures

Because air pollution varies significantly by neighborhood and city, location information is essential for calculating and displaying accurate Air Quality Index (AQI) readings.

### A. Foreground Location (Approximate and Precise)
- **Permissions:** `android.permission.ACCESS_COARSE_LOCATION` and `android.permission.ACCESS_FINE_LOCATION`
- **When It Is Used:** Only when you are actively using the App.
- **Purpose:** Your device coordinates (Latitude and Longitude) are used to query nearby official Central Pollution Control Board (CPCB) monitoring stations, calculate the localized AQI via inverse-distance interpolation, and center the interactive air quality map on your current area.
- **Processing:** Coordinates are transmitted ephemerally over encrypted HTTPS to our API server to query nearby monitoring stations. They are not stored, logged, or tied to your personal identity.

### B. Background Location (Prominent Disclosure)
- **Permission:** `android.permission.ACCESS_BACKGROUND_LOCATION`
- **Prominent Disclosure (Google Play Requirement):**  
  > **AQI Now accesses location data in the background, even when the App is closed or not in use.**
- **Why Background Location is Required:**
  1. **Home Screen Widgets (`AqiWidgetMedium`):** To keep your home screen widget updated with the latest local AQI for your immediate geographic area without requiring you to open the App.
  2. **Periodic Air Quality Notifications:** To evaluate local air quality conditions and trigger health advisories or severe pollution alerts at your chosen notification interval (via Android WorkManager).
- **Non-Advertising Guarantee:** Background location data is **never** used to serve advertisements, **never** used for behavioral profiling, and **never** shared with third-party tracking services.
- **User Control & Revocation:** Background location is strictly optional. You can grant, deny, or revoke background location access at any time through your device's Android settings:
  > **Android Settings > Apps > AQI Now > Permissions > Location > Select "Allow only while using the app" or "Don't allow"**
  If denied, the App will still function fully in the foreground, and home screen widgets will update using your last known or manually selected location.

---

## 3. Google Play Data Safety Alignment Table

To assist users and Google Play review teams, the following table details our declarations in the Google Play Console **Data Safety section**:

| Data Type | Collected? | Shared? | Handled Ephemerally? | Purpose |
| :--- | :--- | :--- | :--- | :--- |
| **Approximate Location** | Yes | No | Yes | App functionality (Hyperlocal AQI calculation, widget updates) |
| **Precise Location** | Yes | No | Yes | App functionality (Nearby station lookup, map display, notifications) |
| **Personal Info** (Name, Email, Phone, User IDs) | **No** | **No** | N/A | None collected |
| **Financial Info** | **No** | **No** | N/A | None collected |
| **Health & Fitness** | **No** | **No** | N/A | None collected |
| **Messages / SMS** | **No** | **No** | N/A | None collected |
| **Photos / Videos / Files** | **No** | **No** | N/A | None collected |
| **Contacts / Calendar** | **No** | **No** | N/A | None collected |
| **App Activity** (In-app Search History) | Saved locally only | No | Stored on-device | App functionality (Quick access to recent cities) |
| **Device / Other Identifiers** (Advertising ID) | **No** | **No** | N/A | None collected |

---

## 4. Notifications & Device Features

- **Permission:** `android.permission.POST_NOTIFICATIONS` (Android 13+)
- **Purpose:** AQI Now sends local notifications to alert you to significant changes in air quality or provide periodic health summaries.
- **User Choice:** You can configure the notification frequency (e.g., every 2 hours, 4 hours, or disabled) directly within the App settings, or turn off notifications altogether in Android system settings.

---

## 5. Local Storage & Data Retention

- **Local Storage:** The App stores user preferences (such as selected language, preferred notification intervals, and recent location searches) locally on your device using Android SharedPreferences and a local SQLite database (Room).
- **Retention:** This data remains exclusively on your device. We do not store or mirror this data on any remote server.

---

## 6. User Data Deletion Instructions

In compliance with Google Play's user data policies:

- **Clearing Search History:** You can clear your saved search history directly within the App at any time.
- **Complete Data Deletion:** Because AQI Now does not require user accounts, all user-associated data resides locally on your device. You can permanently wipe all stored data, preferences, and cache at any time by going to:
  > **Android Settings > Apps > AQI Now > Storage & Cache > Clear Storage (or Clear Data)**  
  Alternatively, uninstalling the App immediately and permanently deletes all local data from your device.
- **Data Inquiries:** If you have questions regarding data deletion or wish to confirm our data handling, you may contact us at [exceltechnologiesindia@gmail.com](mailto:exceltechnologiesindia@gmail.com).

---

## 7. Third-Party Services & Data Sources

To deliver accurate air quality metrics and map visuals, AQI Now interacts with the following trusted third-party services:

1. **AQI Now Backend (`https://anupamkhurana.com/aqi`)**
   - **Role:** Secure proxy and caching server that computes distances to nearby monitoring stations and aggregates historical pollutant trends.
   - **Security:** All transmissions use Transport Layer Security (TLS/HTTPS). No individual tracking profiles are maintained.
2. **Central Pollution Control Board (CPCB) India**
   - **Role:** Official government source providing ambient air quality monitoring readings across Indian cities.
3. **Open-Meteo Air Quality API / Copernicus Atmosphere Monitoring Service (CAMS)**
   - **Role:** Provides secondary meteorological/modeled atmospheric data and historical pollutant trend curves (PM2.5, PM10) when official station feeds are undergoing maintenance.
4. **MapLibre & OpenFreeMap / OpenStreetMap**
   - **Role:** Supplies open-source map tiles for the interactive station map. No user identifiers are passed to map tile servers.
5. **Google Play Services**
   - **Role:** Delivers standard Android platform support, including In-App Reviews and In-App Update checks.

---

## 8. Data Security Practices

We implement industry-standard safeguards to protect data:
- **Encryption in Transit:** All communications between the App and our servers utilize modern HTTPS/TLS encryption protocols (TLS 1.2+).
- **No Unnecessary Storage:** Real-time user GPS coordinates are never retained in server databases.
- **No Third-Party Trackers:** No analytics SDKs or advertising SDKs are embedded in the App.

---

## 9. Children’s Privacy (COPPA & Family Policy Compliance)

AQI Now is designed for a general audience (ages 13 and older). The App does not knowingly collect personally identifiable information from children under 13 years of age. If you are a parent or guardian and believe that a child has inadvertently provided personal data, please contact us immediately at [exceltechnologiesindia@gmail.com](mailto:exceltechnologiesindia@gmail.com), and we will take prompt steps to address it.

---

## 10. Changes to This Privacy Policy

We may update this Privacy Policy from time to time to maintain compliance with relevant laws and Google Play Developer Program policies. Any revisions will be published at [https://anupamkhurana.github.io/AQINow/](https://anupamkhurana.github.io/AQINow/) with an updated "Last Updated" date. We encourage users to review this page periodically.

---

## 11. Developer Contact Information

If you have questions, feedback, or concerns regarding this Privacy Policy or our privacy practices, please contact:

- **Entity:** Excel Technologies India
- **Application:** AQI Now
- **Email:** [exceltechnologiesindia@gmail.com](mailto:exceltechnologiesindia@gmail.com)
