# 📱 SafeRecorder — Installation & Setup Guide

A discreet, high-reliability personal safety companion designed for rapid on-device evidence preservation and emergency protection.

---

## 📋 Quick Reference Card

| Setting / Action | Value / Pattern |
|---|---|
| **Entry Disguise** | **Organizer** (Interactive Daily Checklist & Planner) |
| **Dashboard Unlock** | Tap the **"Organizer"** header **5 times** rapidly |
| **Default Access Password** | `80085` |
| **Pocket Trigger Gesture** | **Volume Down → Volume Up → Volume Down** (within 2.5 seconds) |
| **Haptic Confirmation** | Dual vibration pulse confirms recording started |
| **Stop Recording Gesture** | Press **Volume Down → Volume Up → Volume Down** again |
| **Haptic Stop Confirmation** | Single long vibration pulse confirms recording stopped |

---

## 🚀 Chronological Setup Guide (New Phone Setup)

Follow these steps in order when setting up SafeRecorder on a new or wiped phone:

### Step 1: Install the APK & Bypass Play Protect
Because SafeRecorder utilizes advanced hardware features (Accessibility Service for hardware key triggers, background camera/microphone, and direct file management), Google Play Protect will prompt during manual sideloading.

1. Transfer `SafeRecorder_vFinal.apk` to your phone's **Downloads** folder (or install via USB debugging: `adb install -r -d SafeRecorder_vFinal.apk`).
2. Open your phone's **Files / My Files** app and tap the APK to install.
3. If Google Play Protect displays a warning dialog:
   * Tap **"More details"** (or the dropdown arrow).
   * Tap **"Install anyway"**.
4. *(Optional — Recommended for seamless sideloading)*: If Play Protect completely blocks installation:
   * Open **Google Play Store** > Tap your **Profile Icon** (top right) > **Play Protect**.
   * Tap the **Gear Icon ⚙️** (top right).
   * Temporarily toggle off **"Scan apps with Play Protect"**.
   * Install the APK, then re-enable the scanner if desired.

---

### Step 2: First Launch & Unlocking the Dashboard
1. Open the application from your app drawer (it launches directly into the **Organizer** screen).
2. Tap the **"Organizer"** header text at the top-left of the screen **5 times in quick succession** (within 2 seconds).
3. A security prompt will appear asking to **"Enter password"**.
4. Enter the default password: **`80085`**.
5. Tap **Unlock** to reveal the main SafeRecorder dashboard.

---

### Step 3: Grant Essential Hardware Permissions
Upon unlocking the dashboard, grant the core permissions required for autonomous operation:

1. **Camera & Microphone**:
   * Tap the large **Start Safe Recording** button once.
   * Android will prompt for Camera and Audio recording permissions.
   * Select **"While using the app"** (Android grants foreground/background service access).
2. **All Files Access (Storage)**:
   * Tap the **Storage** tile or when prompted, allow "All files access" so recorded video files and encrypted bundles can be saved reliably to your device storage without being constrained by scoped storage limits.
3. **Battery Optimization Exemption (Crucial)**:
   * Tap the **Battery Shield** card or go to your phone's **Settings > Apps > SafeRecorder > Battery**.
   * Change battery usage from *Optimized* to **Unrestricted** (prevents Android's Doze mode from sleeping background services).

---

### Step 4: Enable Pocket Volume Gesture (Accessibility Service)
To trigger emergency recording silently from inside your pocket with the screen off:

1. On the SafeRecorder main dashboard, tap the **Pocket Gesture Card** (or open phone **Settings > Accessibility**).
2. Look for **Installed apps** or **Downloaded services**.
3. Locate and tap **SafeRecorder**.
4. Toggle the switch to **ON**.
5. When Android prompts for permission, tap **Allow**.

> [!NOTE]
> **Android 13+ "Restricted Setting" Prompt**:
> If Android displays *"Restricted setting: For your security, this setting is currently unavailable"*:
> 1. Open phone **Settings > Apps > SafeRecorder**.
> 2. Tap the **Three Dots (⋮)** in the top-right corner.
> 3. Tap **"Allow restricted settings"** and confirm with your device biometric/PIN.
> 4. Return to **Accessibility > SafeRecorder** and turn it ON.

---

### Step 5: How to Use the Pocket Volume Trigger
Once the Accessibility Service is enabled, the pocket trigger operates 24/7, even when the phone is locked:

1. **To Start Recording**:
   * Press **Volume Down → Volume Up → Volume Down** in sequence within 2.5 seconds.
   * The phone will produce **two quick vibration pulses** confirming recording is active.
   * The camera and microphone silently record high-definition rolling segments.
2. **To Stop Recording**:
   * Press **Volume Down → Volume Up → Volume Down** again.
   * A single long vibration pulse confirms recording has stopped.

---

### Step 6: Customizing Settings & Changing Password
Once inside the unlocked SafeRecorder dashboard:

1. **Change Local Password**:
   * Scroll to the **Local Device Password** tile under System Access & Control.
   * Tap the tile to open the password dialog.
   * Enter your new custom PIN and tap **Save PIN**.
   * *(Note: You can reset back to `80085` at any time from this dialog).*
2. **Select Camera Mode**:
   * Tap the **Camera Mode** tile to switch between:
     * **0.6x Ultrawide Camera** (maximum field of view)
     * **Director Dual PiP** (front and rear combined)
     * **Front Camera**
     * **Standard Rear Camera**
3. **Anti-Uninstall (Device Administrator)**:
   * Tap **Anti-Uninstall (Device Admin)** to activate Android Device Administrator status. This protects the app from being uninstalled without entering your device security credentials.
4. **Relock the App**:
   * Tap the lock icon in the top header to immediately return to the **Organizer** disguise.

---

## 📁 Storage Location of Recordings

All encrypted segments and emergency recordings are saved locally on your phone under:
* `/sdcard/Movies/SafeRecorder/`
* `/sdcard/DCIM/SafeRecorder/`
* `/sdcard/Android/data/com.saferecorder/files/`

---

*SafeRecorder — Autonomous, private, and resilient safety on your terms.*
