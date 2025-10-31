# 🚗 Parked Car Locator (Boater‑Aid Blue Edition)

**Purpose:**  
A Progressive Web App (PWA) that helps you remember where you parked your car — with GPS coordinates, compass bearing, map, note, photo, and parking‑timer reminder. Designed for offline use and installable directly from your browser.

## 🔧 Features
- Live GPS tracking (update or re‑center your current position)
- Park Here to save location, note, and optional photo
- Distance + Compass showing direction to your parked car
- Parking Timer with alert when time expires
- Offline support via service worker caching
- Share & Route buttons for Google Maps navigation
- Boater‑Aid blue icon + dark navy theme

## 📱 How to Install on Android (Samsung S24 or similar)
1. Open Chrome and navigate to your hosted file, e.g. [https://boater‑aid.com/parkedcar/index_pwa.html](https://boater‑aid.com/parkedcar/index_pwa.html)
2. Tap the ⋮ menu → **Add to Home screen**
3. Choose **Install app** when prompted.
4. The app appears on your home screen with its blue car‑pin icon.
5. Grant **Location** and **Motion/Compass** permissions when asked.
6. Use **Update My Position** first, then **Park Here** to save your spot.

💡 *This installs as a “web app” inside Chrome. It will not appear under Settings → Apps unless converted to a native APK.*

## 💻 Optional: Use on Desktop
- Open the same page in Chrome or Edge.
- Click the Install icon (computer + down‑arrow in the address bar).
- Launch it later from your desktop or start menu.

## 🧱 Advanced Option: Make it a True Android App (APK)
If you want it listed in Android’s “Apps” list:

```bash
npm install -g @bubblewrap/cli
bubblewrap init --manifest=https://boater‑aid.com/parkedcar/index_pwa.html
bubblewrap build
adb install app‑release.apk
```

The app will now appear in **Settings → Apps** like a normal Play‑Store app.

## ⚠️ Troubleshooting
| Issue | Fix |
|-------|-----|
| ❌ User denied geolocation | In Chrome → tap the ⓘ icon → Permissions → Allow Location, then reload |
| ⚠️ Compass not moving | Allow Motion sensors in Chrome site settings |
| 🗺️ Map tiles not loading offline | The map requires internet, but GPS + compass still work offline |
| 🕒 Timer doesn’t alert | Keep Chrome notifications allowed for this web app |

## 🧾 Version Info
- **App:** Parked Car Locator PWA
- **Theme:** Boater‑Aid Blue (`#1462FF` / `#0B1220`)
- **Author:** Glen Carruthers
- **Version:** 1.0 PWA (October 2025)
