# System specifications
### Device specifications:
Processor:	13th Gen Intel(R) Core(TM) i7-13700H (2.40 GHz)

Installed RAM:	16.0 GB (15.6 GB usable)

System type:	64-bit operating system, x64-based processor

### Windows Specifications:
Edition;	Windows 11 Home

Version;	24H2

Installed on:	‎2025-‎02-‎09

OS build:	26100.6584

Experience:	Windows Feature Experience Pack 1000.26100.234.0


# Software versions installed
-npm: 11.0.0

-Node.js: v20.17.0

-React Native: 0.81.1 and React-Native-CLI: 2.0.1

-Android Studio: 21.0.7

-VS Code: 1.104.0

## Setup steps you followed
First, I installed Node.js v20.17.0 and verified the installation by running `node --version` and `npm--version`to ensure that the npm version was compatible (v8.0.0 or higher). Next, I installed the React Native CLI using: `npm install -g react-native-cli` and `npm install -g @react-native-community/cli`. After that, I installed Android Studio with the default settings and configured the required tools (Android SDK Platform 31 and 33, Build-Tools 33.0.0...). Then, I set the environment variables for Windows to allow proper communication with the Android SDK. Once the environment was ready, I created an Android Virtual Device (AVD) using Pixel 4 with API 33 as the system image. I then created my React Native project in Visual Studio Code. Although the lab instructions suggested a standard command, I had to use:`npx @react-native-community/cli@latest init NewProject` to make sure I used the latest version of the React Native Community CLI.
Finally, I launched the Android emulator, ran the project, and confirmed that the environment was set up correctly using the command `npx react-native run-android` that opens up the project.

## Any deviations from the lab instructions
Yes, there were a few deviations:

-When running the EnvironmentTest app, I encountered an error related to Native Safe Area support. To fix it, I installed react-native-safe-area-context, which ensures that the app content is displayed properly and is not hidden by UI elements such as notches, status bars, or navigation bars.

-For version control, I configured SSH keys entirely through the terminal. This was challenging because I was only familiar with using GitHub Desktop for push, pull, and commit operations. I had to learn how to generate SSH keys, add them to my GitHub account, and connect my local repository through the console. After some trial and error, I successfully set up SSH keys  and pushed my project to a remote repository, which was a valuable learning experience.

## Time taken for each major step
-Installing the required softwares:  Apporximately 15 minutes waiting for the components to download, setup... 

-Creating the android Virtual Device: Apporximately 15min

-Creating and testing the modifications: Apporximately 1 hours (mostly spent troubleshooting the react-native-safe-area-context error)

-Debbuging and Developer Tools: 15 minutes 

-Version Control Setup: 1 hour (due to SSH key setup challenges)


