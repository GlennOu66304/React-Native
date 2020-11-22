# Run RN Project from Github and ipa package & Test it on your phone
## Run RN Project from Github
 1.Git cloen Project: 
 ```
 git clone git@github.com:wwayne/react-native-nba-app.git
 ```
 2. Go to the package.json in the project folder, and open the file with sublime text, then you will see it is "react-native": "^0.17.0",
 ```
 package.json
 "dependencies": {
    "bluebird": "^3.0.5",
    "es6-enum": "^1.0.0",
    "moment-timezone": "^0.4.1",
    "react-native": "^0.17.0",
 ```
 [How to check the installed version of React-Native](https://stackoverflow.com/questions/37363560/how-to-check-the-installed-version-of-react-native)   

 3, Go to see the doc all version to locat this version of documentation:   
 [React Native Archive 0.17 Doc](https://archive.reactnative.dev/docs/0.17/getting-started)  
 [React Native Archive](https://archive.reactnative.dev/versions)   
  [Stable versions](https://reactnative.dev/versions)   

### Utilize the The React Native CLI quick start to build the enviroment:
4.install the node 8.3
```
node -v
source ~/.bash_profile 
nvm install v8.3.0
```
Wait those code rungning finish, then you are able to see the node version build.  

5.Node, Watchman, JDK
```
source ~/.bash_profile
nvm use v8.3.0  
brew install watchman 
brew tap AdoptOpenJDK/openjdk 
brew cask install adoptopenjdk8
npm install -g react-native-cli 
cd /Users/zt/react-native-nba-app  
```
6.run the Peroject: 
```
react-native start

```
7.open new shell under the project folder: 
```
npm test 
```
[使用nvm管理node与npm版本](https://juejin.im/post/6844903861157642247)  
[Node, Watchman, JDK](https://archive.reactnative.dev/docs/0.17/getting-started)  


## Utilize the node version v8.17.0 (sytem to run the peoject)
1.Node, Watchman, JDK
```
node -v
brew install watchman 
brew tap AdoptOpenJDK/openjdk 
brew cask install adoptopenjdk8
```
The React Native CLI  
```
npm install -g react-native-cli
```

2.Bug fixing:  pm ERR! EEXIST: file already exists, symlink '../lib/node_modules/react-native-cli/index.js' -> '/usr/local/bin/react-native'
npm ERR! File exists: /usr/local/bin/react-native
```
sudo npm install -g react-native-cli --force
```
3. run this project:  
```
cd /Users/zt/react-native-nba-app  
npm install 
react-native start 
```
4.open a new terminal under the peoject folder:  
```
npm test 
```

[terminal: “npm install -g react-native-cli”](https://stackoverflow.com/questions/32171221/terminal-npm-install-g-react-native-cli)   


[The React Native CLI](https://archive.reactnative.dev/docs/0.17/getting-started)   
Main reference:  
[如何运行github上react native项目](https://blog.csdn.net/shiningchen322/article/details/57881920?utm_medium=distribute.pc_relevant.none-task-blog-title-6&spm=1001.2101.3001.4242)  
Source Code:[wwayne/react-native-nba-app](https://github.com/wwayne/react-native-nba-app)  
[下载及运行Github的React Native开源项目](https://blog.csdn.net/jay100500/article/details/77073225)  
## ipa package 
### Certiface issue:  
Your Mac already has a Apple developemt certicate, then download it and put it in the key chain access, at the same time. You need to use it in the Xcode sign locatiuon.

### UDID issue
[Daily Tip: How to get your UDID number from System Profiler on Mac](https://www.imore.com/daily-tip-udid-number-system-profiler-mac)  
[MacOS Catalina UDID Copy for iPhone](https://stackoverflow.com/questions/58805519/macos-catalina-udid-copy-for-iphone)  

### Bundle building: 
1.cd to the ios directory;  
2.under the ios directory, build the bundle folder;   
3.Go back to the project Main directory run the bundle command below:  
```
react-native bundle --entry-file index.js --platform ios --dev false --bundle-output ./ios/bundle/index.ios.jsbundle --assets-dest ./ios/bundle
```
Main reference:  
[一、生成bundle文件](https://juejin.cn/post/6844903639329275912)  

### Release Dug version check:  
run choose the debug mode
Achive Choose the Release, you could check the mode image in the tutorial below to verify it.   
Main refernece:    
[react native Xcode打包app发布ipa到蒲公英](https://blog.csdn.net/sinat_33134895/article/details/81703239?utm_medium=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-2.pc_relevant_is_cache&depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-2.pc_relevant_is_cache)  

### bug fixing:xcode 11.4 build fatal error: module map file xxx/Build/Products/Debug-iphoneos/YogaKit/YogaKit.modulemap' not found
open the .xcodeworkspace file instead of the  .xcodeproj flie. to run in the Xcode;   
Main reference:   
[xcode 11.4 build fatal error: module map file xxx/Build/Products/Debug-iphoneos/YogaKit/YogaKit.modulemap' not found #28503](https://github.com/facebook/react-native/issues/28503)

Bug fixing:  
[How to: Create an .ipa file From XCode 2019](https://www.youtube.com/watch?v=Wb9yQUP04zg&ab_channel=LirsTechTips)   
[Xcode Signing certificate is invalid when build on ext device](https://stackoverflow.com/questions/45803131/xcode-signing-certificate-is-invalid-when-build-on-ext-device)  
1.[Bitcode Compile During Archive Never Finishes](https://stackoverflow.com/questions/36725314/bitcode-compile-during-archive-never-finishes)   
2.[Can not export IPA file from XCode 6.1](https://stackoverflow.com/questions/27061729/can-not-export-ipa-file-from-xcode-6-1)   
3.[Foolproof way to create AdHoc certificates](https://help.installrapp.com/ios/fool-proof-way-to-create-adhoc-certificates/)   
4.[Xcode: Archiving a project to generate .ipa but export is not an option in Organizer](https://apple.stackexchange.com/questions/369987/xcode-archiving-a-project-to-generate-ipa-but-export-is-not-an-option-in-organ)  
5.[How do I find my IOS app's archive file?](https://stackoverflow.com/questions/40274739/how-do-i-find-my-ios-apps-archive-file)  
[Xcode 8 shows error that provisioning profile doesn't include signing certificate](https://stackoverflow.com/questions/39568005/xcode-8-shows-error-that-provisioning-profile-doesnt-include-signing-certificat?page=2&tab=votes#tab-top)  
[Code signing issue in Xcode version 8](https://stackoverflow.com/questions/39565906/code-signing-issue-in-xcode-version-8/54682546#54682546)  

Main reference:   
[React Native 打包 iOS 测试 APP](https://blog.whezh.com/react-native-ios-bundle/)  
[React Native打包iOS的ipa包](https://juejin.im/post/6844903639329275912)   
[react native Xcode打包app发布ipa到蒲公英](https://blog.csdn.net/sinat_33134895/article/details/81703239?utm_medium=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-2.pc_relevant_is_cache&depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-2.pc_relevant_is_cache)   
other References:   
[iOS开发证书和生产证书](https://www.jianshu.com/p/63eca43c175e)  
[获取Xcode 中项目bundle ID 地址](https://blog.csdn.net/wangsun300/article/details/100045974)  
[Certificates, Identifiers & Profiles](https://developer.apple.com/account/resources/profiles/review/A3C6YCFF95)   
[ReactNative开发IOS环境打包ipa过程](https://blog.csdn.net/ywl570717586/article/details/102566658?utm_medium=distribute.pc_feed_404.none-task-blog-OPENSEARCH-9.nonecase&depth_1-utm_source=distribute.pc_feed_404.none-task-blog-OPENSEARCH-9.nonecas)  
[react native Xcode打包app发布ipa到蒲公英](https://blog.csdn.net/sinat_33134895/article/details/81703239?utm_medium=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-2.pc_relevant_is_cache&depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-2.pc_relevant_is_cache)   
[Create an IPA and APK From a React Native Project](https://medium.com/better-programming/create-ipa-and-apk-from-react-native-72fe53c6a8db)  
[Can't add a file to an XCode Project](https://stackoverflow.com/questions/3955655/cant-add-a-file-to-an-xcode-project)   
[xcode 11.4 build fatal error: module map file xxx/Build/Products/Debug-iphoneos/YogaKit/YogaKit.modulemap' not found#28503](https://github.com/facebook/react-native/issues/28503)  
[React Native打包iOS的ipa包](https://juejin.im/post/6844903639329275912)  
  
## apk file:  
Bug fixing:  
1.First time run the Android studio, you need to set the proxy to the auto proxy,then waiit for the process finish.
[First run of Android Studio. Unable to access Android SDK add-on list](https://stackoverflow.com/questions/29878370/first-run-of-android-studio-unable-to-access-android-sdk-add-on-list)

2.zip end header not found   
You need to use the Press Command+Shift+Dot to show the hiden file, then find the ~/.gradle file and rerun the command.  
[zip end header not found](https://github.com/facebook/react-native/issues/21130)  
[How to access hidden files on a Mac](https://setapp.com/how-to/show-hidden-files-on-mac) 

3. Bug:java.lang.NoClassDefFoundError: Could not initialize class org.codehaus.groovy.vmplugin.v7.Java
You need to go to your React Native Project and find the file: gradle-wrapper.properties, then change the distributionUrl to the code below: 
```
distributionUrl=https\://services.gradle.org/distributions/gradle-6.3-all.zip
```
Then run code below:  
```
./gradlew assembleRelease
```
[How to check Java version and JDK version on Mac](https://justinbagley.rbind.io/2020/01/05/how-to-check-java-version-on-mac/)
[services.gradle.org/ distributions/](https://services.gradle.org/distributions/)  
[Android Studio Could not initialize class org.codehaus.groovy.runtime.InvokerHelper](https://stackoverflow.com/questions/35000729/android-studio-could-not-initialize-class-org-codehaus-groovy-runtime-invokerhel)  
[java.lang.NoClassDefFoundError: Could not initialize class org.codehaus.groovy.vmplugin.v7.Ja【已解决】](https://blog.csdn.net/mp624183768/article/details/107316578)  
[What is the difference between gradlew build and gradlew assembleRelease](https://stackoverflow.com/questions/40219917/what-is-the-difference-between-gradlew-build-and-gradlew-assemblerelease)  

Bug fixing:  zsh: command not found: gradle
```
touch .bash_profile
open -e .bash_profile
source .bash_profile 
```

Bug Fixing: SDK location not found. Define location with sdk.dir in the local.properties file or with an ANDROID_HOME environment variable
```
sdk.dir = /Users/USERNAME/Library/Android/sdk
```
[SDK location not found. Define location with sdk.dir in the local.properties file or with an ANDROID_HOME environment variable](https://stackoverflow.com/questions/27620262/sdk-location-not-found-define-location-with-sdk-dir-in-the-local-properties-fil)  
Bug: React Native | Failed to install the app. Please accept all necessary SDK licenses using SDK Manager
[React Native | Failed to install the app. Please accept all necessary SDK licenses using SDK Manager](https://stackoverflow.com/questions/57124607/react-native-failed-to-install-the-app-please-accept-all-necessary-sdk-licens/59249008#:~:text=Go%20to%20Configure%3ESDK%20Manager%20in%20your%20Android%20Studio.&text=And%20accept%20the%20licenses%20you,yet%20(but%20need%20to).&text=Open%20Android%20Studio%2C%20then%20click%20the%20gear%20icon%20(Configure).&text=After%20that%2C%20make%20sure%20that,Android%20SDK%20Tools%20are%20updated.)  

Bug fixing:ERROR Android emulator gets killed
You need to leave the Mac free space for 9 GB to run the emmulater  

[ERROR Android emulator gets killed](https://stackoverflow.com/questions/36841461/error-android-emulator-gets-killed?page=1&tab=votes#tab-top)   

[gradlew: Permission Denied](https://stackoverflow.com/questions/17668265/gradlew-permission-denied/17669566)  


Main reference:  
[Mac下command not found:gradle解决方案](https://www.jianshu.com/p/239a9f964ad2)  
[Gradle Command Not Found](https://stackoverflow.com/questions/37019029/gradle-command-not-found)  
[zsh: command not found: gradle](https://www.programmersought.com/article/47065021046/)  

Main reference:  
[Generating the signed release APK of React Native Android App in 5 minutes](https://www.youtube.com/watch?v=SXFnpo-6u1U&ab_channel=CodewithRaza)  
[Publishing to Google Play Store](https://reactnative.dev/docs/signed-apk-android)  
## Test it on your phone
[蒲公英应用上传](https://www.pgyer.com/doc/view/app_upload)   
[【分享】使用免费的苹果开发者账号申请iOS证书打包测试教程](https://my.oschina.net/u/4356887/blog/3384062)  