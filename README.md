## 1 - Create React Native App & Setup  
1. npm and node version check:  
```
node -v
npm -v
```
2. use the latest npm version to install the app:  
```
source ~/.bash_profile 
nvm use node
Now using node v14.14.0 (npm v6.14.8)
```
3. install the create-react-native-app package 
```
npm install -g create-react-native-app
```
##  2.create a app template:  
1.Expo CLI  
```
npm install -g expo-cli
expo init tipCalc 
cd tipCalc 
yarn start 
```

Main Reference:   
[React Native For Everyone #1 - Create React Native App & Setup](https://www.youtube.com/watch?v=3Pm5_Cf7pQI&ab_channel=LevelUpTuts)  
[Setting up the development environment](https://reactnative.dev/docs/environment-setup)   
[UnhandledPromiseRejectionWarning: Error: Cannot find module '/MyProject/node_modules/react-native-scripts/build/scripts/init.js'](https://stackoverflow.com/questions/52472876/unhandledpromiserejectionwarning-error-cannot-find-module-myproject-node-mod)  
[expo/create-react-native-app](https://github.com/expo/create-react-native-app)   
[React Native UnhandledPromiseRejectionWarning: Error: Cannot find module […]\init.js](https://www.superglobals.net/react-native-unhandledpromiserejectionwarning-error-cannot-find-module-init-js/)   

2.React Native CLI:  
```
brew install node
brew install watchman
```
[Setting up the development environment](https://reactnative.dev/docs/environment-setup)   

## 3. iOS Setup & Simulator  

### 1.Expo (iOS)
1.To run this projec  in the iOS app via expo, you need to go to the webconsole of the React native;  
2.then shift to the send link with the email to send the project address to your email;  
3.at this moment, you need to make sure that your mobile device and pc both under the same internet or wifi;   
4.Go back to the terminal or vs code terminal, input your user-name and password to log in the expo;
5.Then your email will receive the project link;  
6.open this project link in the Expo project, then you will see the project running on the mobile expo app.  
[Run Expo on your own device (iOS)](https://medium.com/@webcore1/how-run-expo-for-react-native-on-your-ios-device-and-first-impressions-49882c38763d)  
[Run the local React Native project on the iOS and Android:](http://glennou.cn/2020/08/22/create-an-app-with-Reac-Native/)  

### 2.Xcode:  

[React Native For Everyone #2 - iOS Setup & Simulator](https://www.youtube.com/watch?v=K0y2tc38l2s&ab_channel=LevelUpTuts)  

## Resource
1.[LCRN EP3 - Trip Booking App (React Native)](https://www.youtube.com/watch?v=iVT7DRw2e7g&list=LL&index=2&t=101s&ab_channel=ByProgrammers)   
2.Source Code:  [byprogrammers/lets-code-react-native](https://github.com/byprogrammers/lets-code-react-native)   
3.[React Native For Everyone #1 - Create React Native App & Setup](https://www.youtube.com/watch?v=3Pm5_Cf7pQI&ab_channel=LevelUpTuts)  
4.[React Native For Everyone #2 - iOS Setup & Simulator](https://www.youtube.com/watch?v=K0y2tc38l2s&ab_channel=LevelUpTuts)   
5.[create an app with Reac Native](http://glennou.cn/2020/08/22/create-an-app-with-Reac-Native/)  
6.[ReactNativeNews/React-Native-Apps](https://github.com/ReactNativeNews/React-Native-Apps)   
7.[Installing & Deploying React Native on OS X - iOS/Android](https://www.youtube.com/watch?v=RBZL6PO2ytc&ab_channel=ReactNativeTutorial)   
8.[facebook/react-native](https://github.com/facebook/react-native#-building-your-first-react-native-app)   