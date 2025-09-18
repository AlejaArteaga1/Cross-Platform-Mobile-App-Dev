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
First I installed node.js version v20.17.0 after that I checked the npm version to see if it is compatible with the program i will run with the commands `node --version` and `npm--version`. Then we install react native CLI with the following commands: `npm install -g react-native-cli` and `npm install -g @react-native-community/cli`. In the third step we install Android studio with the default settings and we configured it with some require additionals tools that configure the screen, the images and some details. Following that we set the enviroment variables in my case for windows and finally we create our android virtual device with Pixel 4, API 33. We continue to create our project in visual studio code (which was already set up and I just added some useful extentions) however in this step I had to type a different command `npx @react-native-community/cli@latest init NewProject` which is used to create a new React Native project with the name that we desire sing the latest version of the React Native Community CLI.Then we start the emulator to create our enviroment.
## Any deviations from the lab instructions
Yes, I needed to install `npm install react-native-safe-area-context` in the moment that i was going to run my application with the EnviromentTest App created because the console throws an error saying that the project did not have a Native Safe Area and was required to initialize the app in the correct way and in that way be able to see my aplication in the home screen. So with `react-native-safe-area-context` it helps to ensure that the app's content is visible and not hidden by the elemets that are not system UI elements like notches, status bars, navigation bars, or home indicators.
## Time taken for each major step
To install the required softwares:  Apporximately 30 minutes waiting for the components to download, setup...


