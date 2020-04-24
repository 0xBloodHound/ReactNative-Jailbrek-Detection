# ReactNative-Jailbrek-Detection

## Step 1 Create React Native Application and Install Modules

```bash
npx react-native init ReactNativeJailbrekDetection 

npm i jail-monkey --save
react-native link 'jail-monkey'

cd ./ios
pod install

npx react-native start
```

![](resources/Reatc%20Native%20-%20Jailbreak%20Detection.md/2020-04-24-13-22-40.png)

![](resources/Reatc%20Native%20-%20Jailbreak%20Detection.md/2020-04-24-13-23-01.png)

**Jail-Monkey**

![](resources/Reatc%20Native%20-%20Jailbreak%20Detection.md/2020-04-24-13-27-37.png)

Go to /android/build.gradle and set "minSdkVersion=19" 

![](resources/Reatc%20Native%20-%20Jailbreak%20Detection.md/2020-04-24-13-33-59.png)

## Step 2 Start Android Application

```
adb reverse tcp:8081 tcp:8081
npx react-native run-android
```

## Step 3 Start iOS Application

Open Xcode

![](resources/Reatc%20Native%20-%20Jailbreak%20Detection.md/2020-04-24-13-38-52.png)

Specific Target Version

![](resources/Reatc%20Native%20-%20Jailbreak%20Detection.md/2020-04-24-13-40-51.png)

Set Signing Certificate

![](resources/Reatc%20Native%20-%20Jailbreak%20Detection.md/2020-04-24-13-41-33.png)

Buide & Run

![](resources/Reatc%20Native%20-%20Jailbreak%20Detection.md/2020-04-24-13-44-08.png)

## Step 4 Adding Root/JailBreak Detection Code

App.js

![](resources/Reatc%20Native%20-%20Jailbreak%20Detection.md/2020-04-24-13-51-23.png)


## Step 5 Terminate the application if root/jailbreak were detected

```
npm i react-native-exit-app --save
react-native link 'react-native-exit-app'
```

![](resources/Reatc%20Native%20-%20Jailbreak%20Detection.md/2020-04-24-13-57-43.png)

![](resources/Reatc%20Native%20-%20Jailbreak%20Detection.md/2020-04-24-14-07-13.png)