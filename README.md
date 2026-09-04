# 01_App_Build - Signed Release App Bundle (.aab)

This directory is designated for storing the compiled and signed Android App Bundle (`app-release.aab`) ready for upload to Google Play Console.

## Build Instructions (Android Studio)
1. Open the project in Android Studio.
2. Select **Build** -> **Generate Signed Bundle / APK...** from the top menu.
3. Choose **Android App Bundle** and click **Next**.
4. Select your keystore file located in `02_Signing/thyrocheck-release-key.jks` and enter key passwords.
5. Choose **release** build variant and click **Create**.
6. Copy the output `app-release.aab` file into this `01_App_Build/` directory.

## Build Instructions (Command Line)
```bash
./gradlew bundleRelease
```
The output `.aab` bundle will be generated at `app/build/outputs/bundle/release/app-release.aab`.
