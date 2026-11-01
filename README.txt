DAS ELECTRICAL CALCULATOR — ANDROID STUDIO PROJECT
=================================================
This is the Android source project for the English-language DAS Electrical Calculator.
It includes offline calculators for:
- Cable size screening and voltage drop
- Motor current and apparent power
- kW / kVA / kVAR conversion
- Preliminary generator running-load estimate
- Basic protection coordination checks

BUILD APK
---------
1. Install Android Studio (current stable) and Android SDK Platform 35.
2. Open this folder in Android Studio.
3. Allow Gradle sync and install any requested Android Gradle plugin.
4. Select Build > Build Bundle(s) / APK(s) > Build APK(s).
5. The debug APK will be generated under app/build/outputs/apk/debug/.

IMPORTANT ENGINEERING LIMITATIONS
---------------------------------
The calculators are preliminary educational/engineering aids, not certified design software.
Cable ampacity values are broad indicative reference values and are not installation-specific.
Final cable sizing must use the applicable IEC/national standard and cable manufacturer data,
including installation method, ambient temperature, grouping, insulation, harmonics, protective
device coordination, fault level, earth conductor and disconnection time.
Generator sizing requires the motor starting-current/torque data and generator transient
performance. A Star-Delta label alone does not establish generator adequacy.
Protection outputs are screening checks, not final breaker/overload settings.
Have a qualified electrical engineer verify designs before installation.


AUTOMATIC CLOUD APK BUILD (NO ANDROID STUDIO REQUIRED ON YOUR PHONE)
---------------------------------------------------------------------
The project includes .github/workflows/build-apk.yml.
1. Extract this ZIP on a computer.
2. Create a GitHub repository and upload the extracted project files.
3. In the repository, open Actions and run "Build DAS Electrical Calculator APK"
   (or push to the main branch).
4. When the workflow finishes, open its run and download the
   "DAS-Electrical-Calculator-APK" artifact.
5. Extract the artifact ZIP to get app-debug.apk, then transfer it to Android
   and install it. Android may ask you to allow installation from that source.

This workflow builds an unsigned debug APK suitable for testing and personal use.
A signed release APK should be generated separately for public distribution.
