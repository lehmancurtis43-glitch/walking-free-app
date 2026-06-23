# **Walking Free Android App Source**
---

---

#### **About This App:**


###### This app was designed by Isaac Weigner to be a companion for people in recovery from active addiction. It has many useful features. Those will be listed later. This is a passion project designed and built by people in recovery for people in recovery. The hope is that this app will be instrumental in helping people who are trying to put their lives together, whether it be for the first or one-hundredth time.


## **How To Build This Project:**

###### **Before building this project, you will need to have Android Studio setup along with Java (openjdk-21-jdk was used when I built it) Make sure you have your $JAVA_HOME variable correct as well as $ANDROID_HOME (neither will be explained in detail here) Inside the project you will need to open the gradle.properties file in either a text editor or IDE and ensure the JAVA_HOME variable is correct with machine.**

###### __On Ububtu, this project can be built one of two ways.__
1. This project can be built with Android Studio.
   - First point the IDE to the path of the project folder.
   - Secondly sync the project with Gradle by clicking on the elephant icon in the top corner.
   - Third step is to build the debug apk and/or aab by clicking the folder icon in the upper left corner to expose the menus.
   Highlight the build menu, scroll down to build apks and bundles, and select the option you wish to build.
   - Finally, you are ready to assemle the release apk and/or aab. For this part locate the terminal symbol on the lower-left hand side of the IDE. Once you have selected this option, the terminal should appear in the bottom panel, central to the IDE display. To build the release apk use the command
   ```bash
   ./gradlew assembleRelease
   ```
   And to build the Android App Bundles use the command
   ```bash
   ./gradlew :app:bundleRelease
   ```
   - After you have finished the build, the completed files will be located in the project root directory under the the path 
   ```
   [PROJECT_ROOT]/app/build/outputs/apk/debug/app-debug.apk
   [PROJECT_ROOT]/app/build/outputs/bundle/debug/app-debug.aab
   [PROJECT_ROOT]/app/build/outputs/apk/release/app-release.apk
   [PROJECT_ROOT]/app/build/outputs/bundle/release/app-release.aab
   ```
2. This project can be built from the terminal.
   - Open the terminal and point it to the root directory of this project with a command like
   ```bash
   cd [path/to/root/director]
   ```
   replacing [path/to/root/directory] with the actual path
   - First run the command
   ```bash
   ./gradlew clean
   ```
   to set up the environment.
   - Second, to build the debug apk run the command
   ```bash
   ./gradlew assembleDebug
   ```
   - Third, to build the debug Android App Bundles run the command
   ```bash
   ./gradlew bundleDebug
   ```
   - The forth step is the build the release apk, and can be done by running the command
   ```bash
   ./gradlew assembleRelease
   ```
   - Then, for five, build the release Android App Bundles with the command
   ```bash
   ./gradlew bundleRelease
   ```
   - After this you will find all of the built files in the following locations starting at the project root directory
   ```
   [PROJECT_ROOT]/app/build/outputs/apk/debug/app-debug.apk
   [PROJECT_ROOT]/app/build/outputs/bundle/debug/app-debug.aab
   [PROJECT_ROOT]/app/build/outputs/apk/release/app-release.apk
   [PROJECT_ROOT]/app/build/outputs/bundle/release/app-release.aab
   ```
