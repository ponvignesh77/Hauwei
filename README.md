# HawkAI Air Gestures + HawkAI Home (Samsung Galaxy F23 5G)

System-wide hand gestures using the front camera + MediaPipe hand tracking.

## Build & install
1. Open this folder in **Android Studio** (Koala or newer). Let Gradle sync (internet needed once;
   the hand model `hand_landmarker.task` is downloaded into `app/src/main/assets` automatically).
2. Enable Developer options + USB debugging on the F23, plug in, press **Run**
   (or Build > Build APK and install the APK).

## First-time setup on the phone (in the app's Setup card)
1. Allow Camera + Notifications.
2. Enable the accessibility service: Settings > Accessibility > Installed apps > HawkAI Air Gestures.
   (If Android blocks it: App info > ⋮ > "Allow restricted settings", then try again.)
3. Allow unrestricted battery. Also: Settings > Battery > Background usage limits >
   Never sleeping apps > add HawkAI (Samsung kills background apps otherwise).
4. Tap **Start**. A notification shows while the camera is watching.

## Default gestures (changeable in the app)
Open palm hold = screenshot · Fist hold = Back · Peace hold = Home · Pinch hold = Play/Pause
Swipe hand left/right = next/previous page · up/down = scroll

## Notes
- Hold poses ~0.7 s, a bit away from the camera, with good light.
- If swipes go the wrong way, turn on "Invert swipe direction".
- Camera pauses when the screen is off. Android shows its camera indicator dot while active.
- On Android 14+, auto-start after reboot may be blocked; open the app once and tap Start.

## HawkAI Home (the launcher / home screen)
The app is also a launcher with the HarmonyOS-style look: clock widget, paged app grid of your real apps,
dock (Phone, Messages, Browser, Camera) and an Air gestures switch on the widget.
Long-press an app for App info / Uninstall.
Make it your home screen: press Home, choose **HawkAI Home** > Always. Or
Settings > Apps > Choose default apps > Home app > HawkAI Home.
Switch back the same way (pick One UI Home).
