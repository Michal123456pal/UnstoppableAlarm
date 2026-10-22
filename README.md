# Unstoppable Alarm 🚨

A simple prank Android app that:

1. When launched, **hides itself from the Recent Apps** list.
2. Schedules a one-time alarm for **30 minutes** later.
3. After 30 minutes:
   - Sets the device **alarm volume to maximum**
   - Plays a loud looping alarm sound
   - Shows a full-screen message: **"Unstoppable :D"**

## Important Notes

- This is a **prank app**. Use responsibly and only on devices you own or have permission to prank.
- On Android 12+ you must grant **Alarms & reminders** (exact alarm) permission.
- On Android 13+ you must grant **Notifications** permission.
- The app uses `STREAM_ALARM` so the sound can play even if media volume is low (but alarm volume must be high).
- Battery optimization / Doze may delay the alarm slightly on some devices; `setExactAndAllowWhileIdle` is used.

## How to build & install

1. Open the project in **Android Studio** (Hedgehog or newer recommended).
2. Let Gradle sync.
3. Connect a device or start an emulator (API 26+).
4. Run the app.
5. Grant the requested permissions when prompted (especially Alarms & reminders).
6. The app will immediately disappear from Recents and schedule the alarm.

## Permissions used

- `SCHEDULE_EXACT_ALARM` / `USE_EXACT_ALARM`
- `POST_NOTIFICATIONS`
- `WAKE_LOCK`
- `VIBRATE`
- `USE_FULL_SCREEN_INTENT`

## Disclaimer

This project is for educational / fun purposes only. The author is not responsible for any misuse.
