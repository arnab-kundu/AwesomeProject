# React Native
This a sample demo app on react-native. App name is AwesomeProject.

## Prerequisites software
1. [Node.js](https://nodejs.org/en/)
2. [VSCode](https://code.visualstudio.com/download)
3. [Android SDK](https://developer.android.com/studio)
4. An android emulator or Physical android device

## Installation
### 1. Node.js
To verify Node.js installation in your system type `node` in CLI and hit Enter. It will return the Node.js version.
```CLI
C:\Users\arnab>node
Welcome to Node.js v14.15.3.
```
### 2. VSCode
Installation of VSCode is pretty straight forward. Just follow the above link to download. After installation below commend should open VSCode, if not you can open it manually.
```CLI
> code .
```
### 3. Android SDK
Install Android Studio. Android SDK will automatically download along with Studio. Its also pretty straight forward. Just follow the above link to download.
### 4. Set ADB path in Environment Variable
Configure platform-tools to System environment variables....    
Add `C:\Users\<user>\AppData\Local\Android\Sdk\platform-tools` this path in System variable.
>Follow below steps to do so.   
`Control Panel` -> `System` -> `Advance System Settings` -> `Environment Variables` -> `System Variables` -> `Path` -> `Edit` -> `New` -> `Paste the path` -> `OK`  

>Now check adb commend working in CLI or not.
```CLI
> adb devices
```
https://reactnative.dev/docs/environment-setup

### Install react-native
To install react-native globally execute below commend. This is a One time operation. No need to install every time while creating a new react-native project.
```CLI
> npm install -g react-native-cli
```
### Create Project
Execute below commend to create a new react-native Project. This will take some time to download all dependency so have patience. It will consume around 125MB.
```
> npx react-native init AwesomeProject
    or  > npx react-native init AwesomeProject --version X.XX.X
    or  > npx react-native init AwesomeTSProject --template react-native-template-typescript
```
### Open Project
Execute below commend to open project in VSCode. You can open manually also.
```
> cd <your-react-native-project-name>
> code .
```
> Set SDK location Path into `local.properties` file and save it into android folder
### Run on Android
Execute below commend to run the project. Make sure an emulator is open, or a physical android device attached before running. Again it will take some time to download all dependency and build project. Once it's done it will automatically launch the app in the emulator/device.
```CLI
> react-native run-android
```
> Note: VSCode TERMINAL will open as powershell by default. Type `cmd` to change terminal into cmd and previous commends again.
### Run on iOS
```CLI
> npx react-native run-ios
```
### VS Code Plugins
* react-native-snippet

### Add node modules in project
```CLI
> npm install --save react-native-vector-icons
> react-native link react-native-vector-icons
> npm i uuidv4
```
