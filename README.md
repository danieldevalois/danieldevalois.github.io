# Privacy, Data Protection, and Deletion Policy for FitOwn

**Last Updated / Effective Date:** October 05, 2026

Welcome to **FitOwn**. We are committed to protecting your personal information and your right to privacy. This document outlines our data privacy practices, third-party integrations, and the explicit steps you can take to manage or permanently delete your information.

---

## 1. Core Architecture: 100% Local and Offline-First

FitOwn is designed from the ground up to respect your absolute sovereignty over your personal metrics.
* **Local Criptographed Storage:** All your fitness routines, workout sets, supplement schedules, weight metrics, and clinical biomarkers (blood work evaluations) are stored **exclusively on your physical device**.
* **On-Device Security:** Your local database is fully encrypted using AES-256 via SQLCipher powered by native Rust execution. 
* **Zero Cloud Tracking:** We do not host external user authentication servers. We do not collect, view, or track your biometric entries or workout schedules under any circumstances.

---

## 2. Integrated Essential Services and Data Flow

To deliver a reliable commercial software experience, FitOwn integrates industry-standard third-party Software Development Kits (SDKs). These services do not touch your local health metrics, but they do process technical data:

* **RevenueCat & Google Play Billing:** If you opt to purchase our Premium or Lifetime licenses, transaction metadata, purchase tokens, and secure device identifiers are processed anonymously. This guarantees that your paid status can be restored seamlessly across device upgrades.
* **Google Mobile Ads (AdMob):** The free tier displays advertisements strictly during workout rest timers. Google AdMob utilizes your device’s Advertising ID (GAID) and IP address to deliver regional relevant ads, monitor deployment health, and prevent invalid automated ad fraud.
* **Technical Diagnostics (Crashlytics):** Automated technical logs, diagnostic reports, and performance metrics are tracked to monitor the runtime stability of the Flutter-to-Rust bridge and fix system-level bugs.

---

## 3. Voluntary Cloud Backups (Google Drive)

FitOwn offers an optional, user-initiated cloud backup feature:
* **Authentication:** If you choose to enable cloud backups, the app requests authorization via the secure Google Sign-In API.
* **Storage Isolation:** The encrypted database file is sent directly to your personal Google Drive account into a hidden, isolated application folder (`appDataFolder`). FitOwn never accesses your private Google files, nor do we store your Google credentials on external servers.

---

## 4. Comprehensive Data Deletion Guide

Since you retain absolute ownership over your fitness and health data, you can permanently erase your footprint at any moment using these options:

### A. In-App Immediate Wipe
1. Open the **FitOwn** application.
2. Navigate to the **Settings** tab.
3. Tap the **"Delete All Local Data"** button.
4. This command instantly and permanently deletes the local encrypted SQLite database from your smartphone storage. This action is irreversible.

### B. Device Uninstallation
1. Open your Android device **System Settings**.
2. Go to **Apps & Notifications** and find **FitOwn** on the list.
3. Select **Uninstall**.
4. The Android operating system will automatically purge all locally stored system files, application caches, and database folders bound to the app.

### C. Cloud Backup Removal
If you have voluntarily created Google Drive backups, you can delete them permanently at any time directly through your personal Google Drive platform under the **"Manage Apps"** data section. FitOwn does not maintain historical archives of your backup files.

---

## 5. Global Privacy Rights Compliance (GDPR, CCPA & LGPD)

Even though FitOwn processes all primary user metrics locally on-device, we strictly adhere to global privacy frameworks. You have the right to access, rectify, restrict, or completely delete your information. Because our architecture delegates absolute data control to the user, you can exercise these rights independently at any second by using the local data management tools inside the app. All background network tráfego initiated by licensing or ad protocols is fully encrypted in transit via secure HTTPS layers.

---

## 6. Contact and Support

If you have questions regarding this privacy framework, data ownership protocols, or how to manage your encrypted databases, please submit an official support ticket using the **Support/Report** hub located inside the application settings tab.
