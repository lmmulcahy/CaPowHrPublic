# CaPowHr Privacy Policy

Effective date: 2026-01-02

This Privacy Policy explains how the CaPowHr watchOS app (the "App") accesses, uses, and stores your information. We designed CaPowHr to work entirely on your Apple Watch and to keep your data on your device and in Apple Health.

We do not collect, transmit, sell, rent, or share your personal data with anyone—except when you explicitly choose to use the optional BLE Diagnostic Log Upload feature described below. The App does not use analytics, advertising, or tracking SDKs.

## Summary
- The App connects to Bluetooth cycling sensors (power/cadence/FTMS) and uses the Watch's heart rate sensor to record indoor cycling workouts.
- Workout data is saved to Apple Health (HealthKit) on your device, under your control.
- No data is transmitted to our servers or third parties by the App, except via the optional, user-initiated BLE Diagnostic Log Upload feature.

## Data We Access and Why

### HealthKit (Apple Health)
The App requests access to the following HealthKit data types solely to support cycling workouts:
- Read:
  - Heart Rate (to display current heart rate during a workout)
- Write:
  - Workouts (Indoor Cycling)
  - Cycling Power
  - Cycling Cadence
  - Distance (Cycling)
  - Active Energy Burned

We do not request access to any other Health types. We only read heart rate during an active workout that you start, and we only write the above metrics while a workout is in progress and when you choose to save it.

### Bluetooth (CoreBluetooth)
The App connects to compatible Bluetooth Low Energy cycling sensors (e.g., power meters, cadence sensors, FTMS bikes). Sensor data is processed on-device to display live metrics and, when applicable, saved to Apple Health. The App does not transmit Bluetooth data off your device unless you explicitly use the optional BLE Diagnostic Log Upload feature.

## Optional BLE Diagnostic Log Upload

The App includes an optional diagnostic feature to help troubleshoot Bluetooth sensor connectivity issues. This feature is:

- **Completely optional**: You must navigate to Settings and explicitly initiate a capture.
- **User-initiated**: You tap "Start Capture" to begin and "Upload Log" to transmit.
- **For debugging purposes only**: The logs help the developer diagnose sensor compatibility problems.
- **Discardable at any time**: You can cancel or discard captured logs without uploading.

### What Data Is Captured

When you initiate a BLE diagnostic capture, the App records approximately 20 seconds of Bluetooth communication data, including:

- Bluetooth sensor names and unique device identifiers (UUIDs)
- Signal strength (RSSI) values
- Service and characteristic UUIDs advertised by sensors
- Raw sensor data packets in hexadecimal format (e.g., power readings, cadence counts)
- Timestamps of Bluetooth events
- App version and build number

### What Data Is NOT Captured

The BLE diagnostic log does **not** include:

- Health data (heart rate, calories, workout summaries)
- Personal identifying information (your name, Apple ID, location, etc.)
- Any data from Apple Health

### Where Logs Are Uploaded

If you choose to upload a log, it is sent to a **public** GitHub repository (github.com/lmmulcahy/CaPowHrPublic) and posted as an issue. Because this is a public repository, the uploaded log will be publicly visible on the internet. Do not upload logs if you are uncomfortable with this.

### Your Controls

- You choose whether to start a capture.
- You choose whether to upload after capture—you can discard instead.
- Logs are stored locally on your device in the App's Documents folder and can be deleted by removing the App.
- Uploading requires a valid GitHub token (either bundled with the App or configured by you).

## Data Storage and Retention
- Workout data that you choose to save is stored in Apple Health on your iPhone/Apple Watch per your Health settings.
- The App keeps only transient/in-memory values to display live metrics during a workout. These values are not uploaded and are discarded when the session ends or you discard the workout.
- BLE diagnostic logs are stored locally in the App's Documents folder until you delete the App.
- You control retention of saved workouts and metrics via the Health app. You can view, edit, or delete data at any time in the Health app.

## Data Sharing
- The App does not share your data with the developer or any third party, except when you explicitly use the BLE Diagnostic Log Upload feature.
- Optional third-party imports (e.g., Strava) are managed by those apps and Apple Health. If you connect Strava to Health, Strava may read workouts you saved in Health. That integration and any data transfer are outside of CaPowHr's control and subject to Strava's policies.

## Permissions and Your Controls
- Health Permissions: You can grant or revoke Health read/write permissions at any time in the Health app (Health → Profile → Apps → CaPowHr).
- Bluetooth Permission: You can control Bluetooth access in Settings.
- In-App Controls: You can start/stop a workout; connect/disconnect sensors; save or discard a workout. Discarding a workout prevents any new data from being written to Health from that session.
- BLE Diagnostic Capture: This feature is entirely opt-in and user-initiated. You control whether to capture, upload, or discard logs.

## Security
- Health data is stored by Apple Health on-device and (if enabled) in iCloud per your Apple settings.
- Bluetooth connections use system-level BLE security. CaPowHr does not implement any additional network connections except for the optional BLE Diagnostic Log Upload.
- BLE diagnostic logs are transmitted over HTTPS to GitHub's API when you choose to upload.

## Children's Privacy
CaPowHr is intended for general audiences and is not directed to children under 13. If you believe a child provided data via the App, you can delete any saved workout data in the Health app.

## Changes to This Policy
We may update this policy from time to time to reflect product or regulatory changes. Material updates will be reflected in this file with a new effective date.

## Contact
If you have questions about this Privacy Policy or the App, please contact: [Your contact email/website]

---

App Facts for App Review:
- Uses HealthKit to read Heart Rate and write Indoor Cycling workouts, Cycling Power, Cycling Cadence, Distance (Cycling), and Active Energy Burned.
- Uses CoreBluetooth to connect to cycling sensors. No location services. No analytics or advertising SDKs.
- Optional BLE Diagnostic Log Upload: User-initiated feature that captures Bluetooth sensor data and, if the user chooses, uploads it to a public GitHub repository for debugging. This feature requires network access and is entirely opt-in.
