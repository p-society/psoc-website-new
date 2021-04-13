---
title: "Session 1 Prerequisites"
date: 2021-04-13T15:16:56+05:30
draft: false
---

## Setup your Flutter environment according to your system:
1) Windows
2) Linux
3) MacOS

# Windows

You can follow steps on [https://flutter.dev/docs/get-started/install/windows](https://flutter.dev/docs/get-started/install/windows),
but we have simplified this to the steps you need:

### Minimum System Requirements for setting up Flutter environment:

-   **Operating Systems**: Windows 7 SP1 or later (64-bit), x86-64 based
-   **Disk Space**: 1.64 GB (does not include disk space for IDE/tools).
-   **Tools**: Flutter depends on these tools being available in your environment.
-   **Windows PowerShell 5.0 or newer** (this is pre-installed with Windows 10.
>   To check the version of powershell you have, follow the following steps:
> -   Open the Start menu or switch to the Start screen by pressing the "**Win**" key on the keyboard. Start typing "**powershell**".
> -   Type or copy-paste the following command: `Get-Host | Select-Object Version`
> -   In the output, you will see the version of PowerShell.

>(if you don’t have the required version which is very unlikely, you can install the newer version from: [https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-7.1](https://docs.microsoft.com/en-us/powershell/scripting/install/installing-powershell-core-on-windows?view=powershell-7.1))

-   **Git for Windows**: If you don’t have, download git from  [https://git-scm.com/download/win](https://git-scm.com/download/win)    

> If Git for Windows is already installed, make sure you can run git commands from the command prompt or PowerShell.

## Steps to install flutter (for Windows) :
-  Download **Flutter SDK** zip file from link [https://drive.google.com/drive/folders/10clpfOsjbDEVdj8l8nLbPzGjcvMxHm6i?usp=sharing](https://drive.google.com/drive/folders/10clpfOsjbDEVdj8l8nLbPzGjcvMxHm6i?usp=sharing)
-  Extract the zip file and place the contained flutter in the desired installation location for the Flutter SDK. (for example, C:\src\flutter).

> Warning: Do not install Flutter in a directory like C:\Program Files\ that requires elevated privileges.
  
Now, you need to update your `PATH` to run flutter from regular Windows Console. For this, follow the following steps:

 - From the Start search bar, enter `env` and select Edit environment variables for your account.
 - Under User variables check if there is an entry called Path:
-   If the entry exists, append the full path to flutter\bin using `;` as a separator from existing values.
-   If the entry doesn’t exist, create a new user variable named Path with the full path to flutter\bin as its value.
    

You have to close and reopen any existing console windows for these changes to take effect.

Now, run the following command:

`C:\src\flutter> flutter doctor`

  

This command checks your environment and displays a report of the status of your Flutter installation. Check the output carefully for other software you might need to install or further tasks to perform (shown in bold text).

For Example:

[-] Android toolchain - develop for Android devices
• Android SDK at D:\Android\sdk
✗ Android SDK is missing command line tools; download from https://goo.gl/XxQghQ
• Try re-installing or updating your Android SDK,

visit https://flutter.dev/setup/#android-setup for detailed instructions.

The following sections describe how to perform these tasks and finish the setup process. Once you have installed any missing dependencies, you can run the flutter doctor command again to verify that you’ve set everything up correctly.

(Remaining steps are below the macOS installing section)

# For Linux
You can follow steps on [https://flutter.dev/docs/get-started/install/linux](https://flutter.dev/docs/get-started/install/linux),
but we have simplified this to the steps you need:

### Minimum System Requirements for setting up Flutter environment:

-   **Operating Systems**: Linux (64-bit)  
-   **Disk Space**: 600 MB (does not include disk space for IDE/tools).
-   **Tools:** Flutter depends on these command-line tools being available in your environment.

   -   bash
   -   curl
   -   file
   -   git 2.x
   -   mkdir
   -   rm
   -   unzip
   -   which
   -   xz-utils
   -   zip

-   **Shared libraries**: Flutter test command depends on this library being available in your environment.
    -   **libGLU.so.1** - provided by mesa packages such as libglu1-mesa on Ubuntu/Debian and mesa-libGLU on Fedora.

### Steps to Install Flutter using snapd:

The easiest way to install Flutter on Linux is by using snapd. For more information, see [Installing snapd](https://snapcraft.io/docs/installing-snapd).
-  Once you have `snapd` run the following command on the command line:
    
`$ sudo snap install flutter --classic`

>Note: Once the snap is installed, you can use the following command to display your Flutter SDK path:

`$ flutter sdk-path`

(Note this path somewhere you might need it later)

- Run the following command to see if there are any dependencies you need to install to complete the setup:
    
`$ flutter doctor`

This command checks your environment and displays a report to the terminal window. The Dart SDK is bundled with Flutter; it is not necessary to install Dart separately. Check the output carefully for other software you might need to install or further tasks to perform (shown in bold text).

For example:
[-] Android toolchain - develop for Android devices
• Android SDK at D:\Android\sdk
✗ Android SDK is missing command line tools; download from https://goo.gl/XxQghQ
• Try re-installing or updating your Android SDK,
visit https://flutter.dev/setup/#android-setup for detailed instructions.

(Remaining steps are below the macOS installing section)

#  For macOS
    
You can follow steps on [https://flutter.dev/docs/get-started/install/macos](https://flutter.dev/docs/get-started/install/macos),
but we have simplified this to the steps you need:

### Minimum System Requirements for setting up Flutter environment:

-   **Operating Systems**: macOS (64-bit)
-   **Disk Space**: 2.8 GB (does not include disk space for IDE/tools).
-   **Tools**: Flutter uses git for installation and upgrade. We recommend installing [Xcode](https://developer.apple.com/xcode/), which includes git.

### Steps to Install Flutter:

1.  Download the following installation bundle to get the latest stable release of the Flutter SDK from the link: [https://drive.google.com/file/d/1jT862lzjYuPfs0_XFHHsbgcTC8sGzCsz/view?usp=sharing](https://drive.google.com/file/d/1jT862lzjYuPfs0_XFHHsbgcTC8sGzCsz/view?usp=sharing)
2.  Extract the file in the desired location, for example:

`cd ~/development`

`$ unzip ~/Downloads/flutter_macos_2.0.4-stable.zip`

### Update Your Path:

1.  Determine the path of your clone of the Flutter SDK. You need this in Step 3.
2.  Open (or create) the rc file for your shell. Typing echo $SHELL in your Terminal tells you which shell you’re using. If you’re using Bash, edit $HOME/.bash_profile or $HOME/.bashrc. If you’re using Z shell, edit $HOME/.zshrc. If you’re using a different shell, the file path and filename will be different on your machine.
3.  Add the following line and change [PATH_OF_FLUTTER_GIT_DIRECTORY] to be the path of your clone of the Flutter git repo:
    
`$ export PATH="$PATH:[PATH_OF_FLUTTER_GIT_DIRECTORY]/bin"`

4.  Run `source $HOME/.<rc file>` to refresh the current window, or open a new terminal window to automatically source the file.
5.  Verify that the flutter/bin directory is now in your PATH by running:
    
`$ echo $PATH`

Verify that the flutter command is available by running:

`$ which flutter`

### Platform Setup (for macOS):

To develop Flutter apps for iOS, you need a Mac with Xcode installed.

1.  Install the latest stable version of Xcode (using [web download](https://developer.apple.com/xcode/) or the [Mac App Store](https://itunes.apple.com/us/app/xcode/id497799835)).
    
2.  Configure the Xcode command-line tools to use the newly-installed version of Xcode by running the following from the command line:

`$ sudo xcode-select --switch /Applications/Xcode.app/Contents/Developer`

`$ sudo xcodebuild -runFirstLaunch`

This is the correct path for most cases, when you want to use the latest version of Xcode. If you need to use a different version, specify that path instead.

3. Make sure the Xcode license agreement is signed by either opening Xcode once and confirming or running sudo xcodebuild -license from the command line.


## The following steps are common for all Windows, Linux and macOS:

### Android Setup :

1.  **Install Android Studio:**
[https://developer.android.com/studio](https://developer.android.com/studio), and follow the steps further to setup an environment.

2.  Enable Debugger options and USB Debugging in your mobile phone. Instructions for the same are given below.
On Android 4.1 and lower, the Developer options screen is available by default. On Android 4.2 and higher, you must enable this screen. To enable developer options, tap the Build Number option 7 times. You can find this option in one of the following locations, depending on your Android version:

-   **Android 9 (API level 28) and higher:** Settings > About Phone > Build Number
-   **Android 8.0.0 (API level 26) and Android 8.1.0 (API level 26):** Settings > System > About Phone > Build Number
-   **Android 7.1 (API level 25) and lower:** Settings > About Phone > Build Number
    
At the top of the Developer options screen, you can toggle the options on and off. You probably want to keep this on. When off, most options are disabled except those that don't require communication between the device and your development computer.

Before you can use the debugger and other tools, you need to enable USB debugging, which allows Android Studio and other SDK tools to recognize your device when connected via USB. To enable USB debugging, toggle the USB debugging option in the Developer Options menu. You can find this option in one of the following locations, depending on your Android version:

-   **Android 9 (API level 28) and higher:** Settings > System > Advanced > Developer Options > USB debugging
-   **Android 8.0.0 (API level 26) and Android 8.1.0 (API level 26):** Settings > System > Developer Options > USB debugging
-   **Android 7.1 (API level 25) and lower:** Settings > Developer Options > USB debugging

### Download Google USB Driver (for Windows only):

1.  In Android Studio, click Tools > SDK Manager.  
2.  Click the SDK Tools tab.  
3.  Select Google USB Driver and click OK.
4.  Proceed to install the package (The link to install is given below after 4th point). When done, the driver files are downloaded into the android_sdk\extras\google\usb_driver\ directory.

Now, follow the steps given in [https://developer.android.com/studio/run/oem-usb#InstallingDriver](https://developer.android.com/studio/run/oem-usb#InstallingDriver)  according to your system.

5.  Using a USB cable, plug your phone into your computer. If prompted on your device, authorize your computer to access your device.
6.  In the terminal, run the flutter devices command to verify that Flutter recognizes your connected Android device.

> Install VS Code: Download VS Code according to your system through [https://code.visualstudio.com/download](https://code.visualstudio.com/download).

### Installing Flutter and Dart plugins:

1.  Start VS Code.
2.  Invoke View > Command Palette or Press Ctrl + Shift + P
3.  Type “install”, and select Extensions: Install Extensions.
4.  Type “flutter” in the extensions search field, select Flutter in the list, and click Install. This also installs the required Dart plugin.
  
### Validate your setup with Flutter Doctor:

1.  Invoke View > Command Palette or Press Ctrl + Shift + P
2.  Type “doctor”, and select the Flutter: Run Flutter Doctor.
3.  Review the output in the OUTPUT pane for any issues. Make sure to select Flutter from the dropdown in the different Output Options.