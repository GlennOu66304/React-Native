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

Bug fixing:  
1.[Bitcode Compile During Archive Never Finishes](https://stackoverflow.com/questions/36725314/bitcode-compile-during-archive-never-finishes)   
2.[Can not export IPA file from XCode 6.1](https://stackoverflow.com/questions/27061729/can-not-export-ipa-file-from-xcode-6-1)   
3.[Foolproof way to create AdHoc certificates](https://help.installrapp.com/ios/fool-proof-way-to-create-adhoc-certificates/)   
4.[Xcode: Archiving a project to generate .ipa but export is not an option in Organizer](https://apple.stackexchange.com/questions/369987/xcode-archiving-a-project-to-generate-ipa-but-export-is-not-an-option-in-organ)  

[React Native 打包 iOS 测试 APP](https://blog.whezh.com/react-native-ios-bundle/)  
[iOS开发证书和生产证书](https://www.jianshu.com/p/63eca43c175e)  
[获取Xcode 中项目bundle ID 地址](https://blog.csdn.net/wangsun300/article/details/100045974)  
[Certificates, Identifiers & Profiles](https://developer.apple.com/account/resources/profiles/review/A3C6YCFF95)   
[ReactNative开发IOS环境打包ipa过程](https://blog.csdn.net/ywl570717586/article/details/102566658?utm_medium=distribute.pc_feed_404.none-task-blog-OPENSEARCH-9.nonecase&depth_1-utm_source=distribute.pc_feed_404.none-task-blog-OPENSEARCH-9.nonecas)  
[react native Xcode打包app发布ipa到蒲公英](https://blog.csdn.net/sinat_33134895/article/details/81703239?utm_medium=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-2.pc_relevant_is_cache&depth_1-utm_source=distribute.pc_relevant.none-task-blog-BlogCommendFromMachineLearnPai2-2.pc_relevant_is_cache)   
[Create an IPA and APK From a React Native Project](https://medium.com/better-programming/create-ipa-and-apk-from-react-native-72fe53c6a8db)  
[Can't add a file to an XCode Project](https://stackoverflow.com/questions/3955655/cant-add-a-file-to-an-xcode-project)   
[xcode 11.4 build fatal error: module map file xxx/Build/Products/Debug-iphoneos/YogaKit/YogaKit.modulemap' not found#28503](https://github.com/facebook/react-native/issues/28503)  
[React Native打包iOS的ipa包](https://juejin.im/post/6844903639329275912)  
  

## Test it on your phone
[蒲公英应用上传](https://www.pgyer.com/doc/view/app_upload)   
[【分享】使用免费的苹果开发者账号申请iOS证书打包测试教程](https://my.oschina.net/u/4356887/blog/3384062)  