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

## 2.React Native CLI:  
1.Node & Watchman   
```
brew install node
source ~/.bash_profile 
nvm use node
brew install watchman
```
2.CocoaPods
```
sudo gem install cocoapods
```
3.Creating a new application
```
npx react-native init AwesomeProject
```
4.Running your React Native application,under the project folder
```
npx react-native start
source ~/.bash_profile  
nvm use node 
```
5.Bug fixing: error Error: Command failed: yarn add react-native@latest  
```
node -v 
source ~/.bash_profile 
nvm use node
npx react-native init TripBookingApp 
```
Note If the above command is failing, you may have old version of react-native or react-native-cli installed globally on your pc. Try uninstalling the cli and run the cli using npx  
[React-native init NewProject / yarn add got an error .](https://medium.com/codespace69/react-native-init-newproject-yarn-add-got-an-error-6a5353f8469b)  
[How to uninstall react-native-cli on mac?](https://stackoverflow.com/questions/57248515/how-to-uninstall-react-native-cli-on-mac)   
Main Reference:  
[Setting up the development environment](https://reactnative.dev/docs/environment-setup)   

## 3. iOS Setup & Simulator  

### 1.Expo (iOS) with external device:
1.To run this projec  in the iOS app via expo, you need to go to the webconsole of the React native;  
2.then shift to the send link with the email to send the project address to your email;  
3.at this moment, you need to make sure that your mobile device and pc both under the same internet or wifi;   
4.Go back to the terminal or vs code terminal, input your user-name and password to log in the expo;
5.Then your email will receive the project link;  
6.open this project link in the Expo project, then you will see the project running on the mobile expo app.  
[Run Expo on your own device (iOS)](https://medium.com/@webcore1/how-run-expo-for-react-native-on-your-ios-device-and-first-impressions-49882c38763d)  
[Run the local React Native project on the iOS and Android:](http://glennou.cn/2020/08/22/create-an-app-with-Reac-Native/)  

Apologize for the cancellation, I have a full day meeting which was assigned this day, I will find another time to take your class, See you soon.

### 2. Expo Xcode on the iOS device:  
1.You need to leave 40GB to allow the system to install the Xcode
2.in the terminl to click the i to open the simulator:

Main reference:  
[iOS Simulator](https://docs.expo.io/workflow/ios-simulator/)  
[Xcode old version install](https://developer.apple.com/download/more/)  
[React Native For Everyone #2 - iOS Setup & Simulator](https://www.youtube.com/watch?v=K0y2tc38l2s&ab_channel=LevelUpTuts)  
[entering a file path into Finder or elsewhere?](https://discussions.apple.com/thread/3911493#:~:text=Answer%3A%20A%3A-,Answer%3A%20A%3A,%22%20button%20%26%20you%20are%20there.)  
[How To Recover Disk Space From Xcode](http://blog.neverthesamecolor.net/how-to-recover-disk-space-from-xcode/)   
[Xcode free space requirement](https://apple.stackexchange.com/questions/252753/xcode-free-space-requirement)  
[Xcode "There is not enough disk space available to install the product." with plenty of space.](https://developer.apple.com/forums/thread/27992)   

### 3.Expo web:  



## Resource
1.[LCRN EP3 - Trip Booking App (React Native)](https://www.youtube.com/watch?v=iVT7DRw2e7g&list=LL&index=2&t=101s&ab_channel=ByProgrammers)   
2.Source Code:  [byprogrammers/lets-code-react-native](https://github.com/byprogrammers/lets-code-react-native)   
3.[React Native For Everyone #1 - Create React Native App & Setup](https://www.youtube.com/watch?v=3Pm5_Cf7pQI&ab_channel=LevelUpTuts)  
4.[React Native For Everyone #2 - iOS Setup & Simulator](https://www.youtube.com/watch?v=K0y2tc38l2s&ab_channel=LevelUpTuts)   
5.[create an app with Reac Native](http://glennou.cn/2020/08/22/create-an-app-with-Reac-Native/)  
6.[ReactNativeNews/React-Native-Apps](https://github.com/ReactNativeNews/React-Native-Apps)   
7.[Installing & Deploying React Native on OS X - iOS/Android](https://www.youtube.com/watch?v=RBZL6PO2ytc&ab_channel=ReactNativeTutorial)   
8.[facebook/react-native](https://github.com/facebook/react-native#-building-your-first-react-native-app)   