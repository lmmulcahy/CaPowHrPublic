# CaPowHr Privacy Policy

Effective date: 2025-10-12

This Privacy Policy explains how the CaPowHr watchOS app (the "App") accesses, uses, and stores your information. We designed CaPowHr to work entirely on your Apple Watch and to keep your data on your device and in Apple Health.

We do not collect, transmit, sell, rent, or share your personal data with anyone. The App does not use analytics, advertising, or tracking SDKs.

## Summary
- The App connects to Bluetooth cycling sensors (power/cadence/FTMS) and uses the Watch’s heart rate sensor to record indoor cycling workouts.
- Workout data is saved to Apple Health (HealthKit) on your device, under your control.
- No data is transmitted to our servers or third parties by the App.

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
The App connects to compatible Bluetooth Low Energy cycling sensors (e.g., power meters, cadence sensors, FTMS bikes). Sensor data is processed on-device to display live metrics and, when applicable, saved to Apple Health. The App does not transmit Bluetooth data off your device.

## Data Storage and Retention
- Workout data that you choose to save is stored in Apple Health on your iPhone/Apple Watch per your Health settings.
- The App keeps only transient/in-memory values to display live metrics during a workout. These values are not uploaded and are discarded when the session ends or you discard the workout.
- You control retention of saved workouts and metrics via the Health app. You can view, edit, or delete data at any time in the Health app.

## Data Sharing
- The App does not share your data with the developer or any third party.
- Optional third-party imports (e.g., Strava) are managed by those apps and Apple Health. If you connect Strava to Health, Strava may read workouts you saved in Health. That integration and any data transfer are outside of CaPowHr’s control and subject to Strava’s policies.

## Permissions and Your Controls
- Health Permissions: You can grant or revoke Health read/write permissions at any time in the Health app (Health → Profile → Apps → CaPowHr).
- Bluetooth Permission: You can control Bluetooth access in Settings.
- In-App Controls: You can start/stop a workout; connect/disconnect sensors; save or discard a workout. Discarding a workout prevents any new data from being written to Health from that session.

## Security
- Health data is stored by Apple Health on-device and (if enabled) in iCloud per your Apple settings.
- Bluetooth connections use system-level BLE security. CaPowHr does not implement any additional network connections.

## Children’s Privacy
CaPowHr is intended for general audiences and is not directed to children under 13. If you believe a child provided data via the App, you can delete any saved workout data in the Health app.

## Changes to This Policy
We may update this policy from time to time to reflect product or regulatory changes. Material updates will be reflected in this file with a new effective date.

## Contact
If you have questions about this Privacy Policy or the App, please contact: [Your contact email/website]

---

App Facts for App Review:
- Uses HealthKit to read Heart Rate and write Indoor Cycling workouts, Cycling Power, Cycling Cadence, Distance (Cycling), and Active Energy Burned.
- Uses CoreBluetooth to connect to cycling sensors. No location services. No analytics or advertising SDKs. No data leaves the device.

