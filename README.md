# Ionic4-Cordova-Start Template
This is a Ionic4-Cordova-Start template with the Ionic/Angular version 4.0.0.

## Required software
Please install the following software before continue.
1. Node.js (v10.15.0 LTS) [https://nodejs.org/](https://nodejs.org/)   
   ```bash
   // Verifying of the installation:
   $ node --version
   ```
2. NPM (v6.6.0)
   ```bash
   $ sudo npm install -g npm@6.6.0
   ```
   ```bash
   // Verifying of the installation:
   $ npm --version
   ```
3. Ionic CLI
   ```bash
   $ sudo npm install -g ionic@4.9.0
   ```
   ```bash
   // Verifying of the installation:
   $ ionic --version
   ```

---

## How to get the template?
There a three ways to get the template.
#### a) Download the repository
Download the files from the repository: [https://github.com/joerg-holland/ionic4-cordova-start](https://github.com/joerg-holland/ionic4-cordova-start)
   
#### b) Clone the repository with Git
Please install the software Git.
1. Git (v2.20.1) [https://git-scm.com/](https://git-scm.com/)
   ```bash
   // Verifying of the installation:
   $ git --version
   ```
2. Clone the repository with the command:
   ```bash
   $ git clone https://github.com/joerg-holland/ionic4-cordova-start
   ```

#### c) Create this template with Ionic CLI
1. Please run the command to create a new Ionic tabs project using the Ionic CLI:
   ```bash
   $ ionic start ionic4-cordova-start tabs --type=angular
   ```
---

## How to build and run the application?

### Web application
1. Open the Command Line Interface (recommended with admin rights) and open the project folder.
   ```bash
   $ cd c:/<YOUR_PROJECT>/
   ```
2. Install the packages (if you downloaded or cloned the template):
   ```bash
   $ npm install
   ```
3. Build the current version of the app:
   ```bash
   $ ionic build
   ```
4. Run a live-mode of the current version of the app (for development):
   ```bash
   $ ionic serve
   ```

### Device
#### Required software
Please install the following software before continue.

##### Apache Cordova
Version: 8.1.2
```bash
$ sudo npm install -g cordova@8.1.2
```
```bash
// Verifying the installation:
$ cordova --version
```

##### Android
If you want to deploy and run the app on a Android device.
1. Java SE Development Kit (v11.0.2) [https://www.oracle.com/technetwork/java/javase/downloads/index.html](https://www.oracle.com/technetwork/java/javase/downloads/index.html)

2. To build an Android app, the Android-SDKs must be installed with the Android Studio **OR** manually with the Android SDK-Tools and Gradle. If an Android-Emulator is used you must install the Android Studio.

   ###### Android Studio
   Android Studio (Version: 3.3) [https://developer.android.com/studio/](https://developer.android.com/studio/)
   
   ###### Android SDK-Tools and Gradle
   a) Android SDK-Tools (Version: Revision 26.1.1)
   1. Android SDK-Tools [https://developer.android.com/studio/](https://developer.android.com/studio/) (Link is available at the end of the site)
   2. Unzip everything and copy the 'tools'-folder to:
      ```bash
      "C:\Android\sdk"
      ```
   3. Set the system variable (as administrator):
      ```bash
      $ sudo setx ANDROID_HOME "C:\Android\sdk" /M
      ```
   4. Add to the path variable:
      ```bash
      $ set PATH=%PATH%;C:\Android\sdk\platforms
      $ set PATH=%PATH%;C:\Android\sdk\tools
      $ set PATH=%PATH%;C:\Android\sdk\tools\bin
      ```
   5. Verifying the installation:
      ```bash
      $ sdkmanager --list
      ```
   6. Add the SDK-Platforms (e.g. API Level 26 = Android 8.0):
      ```bash
      $ sdkmanager "platforms;android-26"
      ```
   7. Add the SDK-Build-Tools:
      ```bash
      $ sdkmanager "build-tools;26.1.1"
      ```
   b) Gradle (Version: 5.1.1) 
   1. Please download the software from the following website: [https://gradle.org/releases/](https://gradle.org/releases/) (binary-only)
   2. Unzip everything and copy the 'tools'-folder to:
      ```bash
      "C:\Program Files\Gradle"
      ```
   3. Set the system variable (as administrator):
      ```bash
      $ sudo setx GRADLE_HOME "C:\Program Files\Gradle\bin"
      ```
   4. Add to the path variable:
      ```bash
      $ set PATH=%PATH%;C:\Program Files\Gradle\bin
      ```
   5. Verifying the installation:
      ```bash
      $ gradle --version
      ```

##### iOS
If you want to deploy and run the app on a iOS device.
1. xCode (Version: 10) [https://developer.apple.com/xcode/](https://developer.apple.com/xcode/)
2. Install the NPM-package `ios-deploy`:
   ```bash
   $ sudo npm install ios-deploy@1.9.4 -g
   ```
      
##### Windows
If you want to deploy and run the app on a Windows device.
Visual Studio (Version: 2017) [https://visualstudio.microsoft.com/](https://visualstudio.microsoft.com/)

#### Build and deploy the app to a device

##### Android
More information: [https://beta.ionicframework.com/docs/building/android](https://beta.ionicframework.com/docs/building/android)

1. Generate the native project, if it does not already exist:
   ```bash
   $ ionic cordova prepare android
   ```
2. Install the platform:
   ```bash
   $ ionic cordova platform add android --save
   ```
3. Build the current version of the app:
   ```bash
   $ ionic build
   ```
4. Build the native app:
   ```bash
   $ ionic cordova build android
   ```
4. Deploy the app to device:
   ```bash
   $ ionic cordova run android --device
   ```

Substitute `android` for `ios` if on a Mac.

## Debugging
### Google Chrome 
To list all connected devices and to debug an app on a device, open the web browser and enter:
`chrome://inspect`

## Troubleshooting
### Android Debug Bridge
If the device is not found during the deploy process, please start the Android Debug Bridge:
1. Open the Command Line Interface and open the folder:
   ```bash
   "C:\Users\<USER>\AppData\Local\Android\sdk\platform-tools"
   ```
2. Run the Android Debug Bridge with the command:
   ```bash
   $ cmd adb.exe
   ```
3. List all devices:
   ```bash
   $ adb devices
   ```

## IDEs
- Visual Studio Code [https://code.visualstudio.com/](https://code.visualstudio.com/)
- JetBrains WebStorm [https://www.jetbrains.com/webstorm/](https://www.jetbrains.com/webstorm/)
- StackBlitz [https://stackblitz.com/](https://stackblitz.com/)

## Help

### Official documentation
[https://beta.ionicframework.com/docs/](https://beta.ionicframework.com/docs/)

### Josh Morony
- Website: [https://www.joshmorony.com/](https://www.joshmorony.com/)
- Youtube: [https://www.youtube.com/user/LittlejTFS](https://www.youtube.com/user/LittlejTFS)

### Simon Reimler
- Ionic Academy: [https://ionicacademy.com/](https://ionicacademy.com/)
- Youtube: [https://www.youtube.com/user/saimon1924](https://www.youtube.com/user/saimon1924)
- devdactic: [https://devdactic.com/](https://devdactic.com/)

### Paul Halliday
- Blog: [https://blog.paulhalliday.io/](https://blog.paulhalliday.io/?)
- Youtube: [https://www.youtube.com/channel/UCYJ9O6X1oFt7YGXpfRwrcWg](https://www.youtube.com/channel/UCYJ9O6X1oFt7YGXpfRwrcWg)

### Apache Cordova:
#### Official documentation
- [https://cordova.apache.org/docs/en/latest/](https://cordova.apache.org/docs/en/latest/)

#### Plugins supported with Ionic
- [https://beta.ionicframework.com/docs/native](https://beta.ionicframework.com/docs/native) 