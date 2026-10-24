ALPHA OS TV - Android TV / Fire TV app project

BUILD (on your Windows PC)
1. Install Android Studio (free, developer.android.com/studio).
2. In Android Studio choose Open, then pick this AlphaTV folder. Let Gradle sync finish (needs internet).
3. Build > Build Bundle(s) / APK(s) > Build APK(s). The file appears at app/build/outputs/apk/debug/app-debug.apk

INSTALL ON THE FIRE TV STICK
1. On the Stick: Settings > My Fire TV > About, press OK on the device name 7 times to enable Developer options.
2. Settings > My Fire TV > Developer options: turn on ADB debugging and Apps from Unknown Sources.
3. Find the Stick IP address under Settings > My Fire TV > About > Network.
4. On your PC with Android platform-tools: adb connect STICK_IP:5555 then adb install app-debug.apk
   (or host the APK and install it with the Downloader app).
5. Open ALPHA OS from Your Apps and Channels.

The whole interface is app/src/main/assets/index.html - edit it and rebuild to change anything.
Voice: press the Menu (three lines) button on the remote, or choose Voice on the home screen.
