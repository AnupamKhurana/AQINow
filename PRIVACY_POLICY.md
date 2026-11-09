# Privacy Policy for AQI Now

**Last Updated: November 9, 2026**

Excel Technologies India ("we," "us," or "our") operates the **AQI Now** mobile application (the "App"). This Privacy Policy explains how we collect, use, and protect your information when you use our App, and describes your privacy rights in accordance with Google Play Developer Policies and global data protection regulations.

---

### Core Principles
- **No User Accounts:** You can use AQI Now without creating an account, registering, or providing any personal information (such as your name, email address, or phone number).
- **No Advertisements:** AQI Now contains no third-party advertisements or ad tracking SDKs.
- **No Data Selling:** We never sell, monetize, or rent your data to third parties.

---

## 1. Information Collection and Permissions

### Location Data (Foreground and Background)
AQI Now is an air quality monitoring application designed to provide hyperlocal Air Quality Index (AQI) readings, health advisories, and nearby station data. To deliver these services, the App requires access to your device location:

1. **Foreground Location (Approximate and Precise):**
   - **Permissions:** `android.permission.ACCESS_COARSE_LOCATION` and `android.permission.ACCESS_FINE_LOCATION`.
   - **Purpose:** When the App is open, your location coordinates (Latitude and Longitude) are used to find the nearest official air quality monitoring stations, compute hyperlocal AQI values, and display your relative position on the air quality map.
   - **Processing:** Coordinates are sent securely via HTTPS to our API server to query nearby monitoring stations. Your coordinates are never stored in tracking profiles or linked to your identity.

2. **Background Location (Prominent Disclosure):**
   - **Permission:** `android.permission.ACCESS_BACKGROUND_LOCATION`.
   - **Why Background Location is Needed:** AQI Now provides **Home Screen Widgets** and **Periodic Air Quality Notifications**. To ensure your home screen widget displays the current air quality for your immediate area and to deliver timely health advisories even when you are not actively using or looking at the App, AQI Now may access your location periodically in the background.
   - **User Control:** Background location access is strictly optional. You can grant, deny, or revoke background location access at any time through your device's Android Settings (`Settings > Apps > AQI Now > Permissions > Location`). If you choose not to grant background location access, the App will still function fully in the foreground, and widgets can update using your last searched or manually set location.
   - **No Background Tracking:** Background location data is used exclusively to fetch relevant air quality readings. It is never used for advertising, behavioral profiling, or background movement tracking.

### Notifications
- **Permission:** `android.permission.POST_NOTIFICATIONS` (Android 13+).
- **Purpose:** To deliver periodic AQI updates, health recommendations, and severe pollution alerts based on your preferences.
- **Control:** You can customize the notification frequency (e.g., every 2 hours, 4 hours, or off) directly in the App's settings or disable notifications completely in Android system settings.

### On-Device Local Storage
- **Data Stored:** The App stores your preferred settings (such as notification intervals, language selection, and recent AQI search history) locally on your device using Android SharedPreferences and a local SQLite database.
- **Storage Scope:** This data remains strictly on your device and is never uploaded, synced, or backed up to our remote servers.

---

## 2. How We Use Information

We use the information collected solely to provide and improve the App's functionality:
- To calculate and display accurate, real-time Air Quality Index (AQI) values and individual pollutant levels (PM2.5, PM10, NO2, SO2, CO, OZONE).
- To update your home screen widgets with relevant local data.
- To send periodic local air quality notifications when enabled.
- To display nearby monitoring stations on an interactive map.

---

## 3. Third-Party Services and Data Sources

To calculate and present air quality data and map visualizations, the App interacts with the following services:

- **AQI Now API Backend (`https://anupamkhurana.com/aqi`):**
  Provides proximate station lookup and historical AQI trend data. All transmissions are encrypted using HTTPS/TLS. The backend does not log or store individual user location histories.
- **Central Pollution Control Board (CPCB) India:**
  Official government air quality monitoring station data used to deliver official Indian National AQI (NAQI) figures.
- **Open-Meteo Air Quality API / CAMS:**
  Used as a modeled fallback source and for historical trend calculations when local physical stations are unavailable.
- **MapLibre & OpenFreeMap / OpenStreetMap:**
  Used to display vector map tiles for station visualization. No personally identifiable information is transmitted to map tile providers.
- **Google Play Services:**
  Provides standard Google Play In-App Updates and In-App Reviews.

---

## 4. Data Retention and Deletion (User Data Rights)

Because AQI Now does not require user accounts, we do not store personal profiles on our servers.

### How to Delete Your Data:
- **Search History:** You can clear your search history at any time from within the App by tapping the clear history option.
- **Complete Data Removal:** You can permanently delete all locally stored data, preferences, and cached readings at any time by going to your device's:  
  `Settings > Apps > AQI Now > Storage > Clear Storage / Clear Data`  
  or by uninstalling the application.

---

## 5. Security of Your Data

We take the security of your data seriously:
- **Encryption in Transit:** All communications between the App and our backend servers are secured using Transport Layer Security (TLS/HTTPS).
- **No Server-Side Tracking:** We do not maintain databases tracking individual user locations, IP addresses, or device identifiers.

---

## 6. Children's Privacy

AQI Now does not knowingly collect or solicit personal information from children under the age of 13. Since our App does not collect personally identifiable information from any user, children can safely view air quality information. If you have reason to believe that a child has provided us with personal information, please contact us so that we can take appropriate steps.

---

## 7. Changes to This Privacy Policy

We may update our Privacy Policy periodically to reflect changes in our practices or regulatory requirements. Any updates will be posted on this page with an updated "Last Updated" date. We encourage you to review this page periodically.

---

## 8. Contact Us

If you have questions, suggestions, or concerns regarding this Privacy Policy or our data practices, please contact us:

- **Developer:** Excel Technologies India
- **Email:** [exceltechnologiesindia@gmail.com](mailto:exceltechnologiesindia@gmail.com)
