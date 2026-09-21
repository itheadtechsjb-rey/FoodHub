# My Food Store - Android app

Your my_food_store_final_v2.html wrapped in a native Android WebView app (works offline, no internet permission).
The web app lives in app/src/main/assets/index.html - edit it and rebuild to change the app.

## Get the APK (pick one)

A. Android Studio (easiest on a PC)
1. Install Android Studio, then File > Open > select this folder. Wait for Gradle sync.
2. Build > Build Bundle(s) / APK(s) > Build APK(s).
3. APK: app/build/outputs/apk/debug/app-debug.apk - copy it to your phone and install it
   (allow "install unknown apps" when asked).

B. No install - GitHub builds it for you
1. Create a free GitHub repo and upload everything in this folder (including the hidden .github folder).
2. Open the repo's Actions tab > "Build APK" > Run workflow.
3. When it finishes, download MyFoodStore-APK from the run's Artifacts.

## What was changed in the HTML for the app
- Back button closes the cart / leaves Admin before exiting the app
- Storage-full warning instead of silent failure
- Print makes a readable receipt (Android print dialog / Save as PDF) instead of raw JSON
- Fixed prompts that showed literal "\n" text
- Alerts, confirms, PIN prompts (masked) and the photo picker work natively

Default admin PIN is 1234 - change it in Admin after first launch.
