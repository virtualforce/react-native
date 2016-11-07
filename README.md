# React Native
React Native is the javascript framework specialized in mobile application which is build on top of react.js, a framework for web.It've been quickly popular due to its ability to translate javascript code into native platform code. It is currently supporting 3 major platform android, window and iphone and is expected to support 10 major mobile platform in near future.

## React vs React Native
ReactJs has been build to target web platform, react native is for mobile application it share most of the common functionality from web but some component is replace by mobile platforms
For Example 
`<div>,<span> translated to <view> in mobile applications`

## Setup
Instructions are written on there official docs. it's easy for windows linux and mac
https://facebook.github.io/react-native/docs/getting-started.html

## ES5 vs ES6
ES5 uses React.createClass which is old way of writing componenets while ES6 uses class extends React.Component
Both syntax are highly in used but later one is preferable because ES6 used much simpler syntax with great performance improvements
for more detail read 
https://toddmotto.com/react-create-class-versus-component/
https://babeljs.io/blog/2015/06/07/react-on-es6-plus

## Android Emulator
Genymotion is the emulator that provide handle button to reload automatically and hot reloading.
install it from here
https://www.genymotion.com/

## IOS Simulator 
it is simulator provide with XCode.

## Three command to create and run project
```
   react-native init AwesomeProject
   cd AwesomeProject
   For Android => react-native run-ios 
   For IOS => react-native run-android 
   
   Note: Emulator/Simulator Emulator must be running and set to your ip address and port 8081
   
   => use this one to set automatically "adb reverse tcp:8081 tcp:8081"
   =>  To Set manually https://facebook.github.io/react-native/docs/running-on-device-android.html#using-adb-reverse

   => Go to dev settings 
      -> debugging 
      -> set localhost:8081 OR IP_ADDRESS:8081 for devices

```

That's it! 

# Compnenets
  project structure is as follows
```
Project root directory
 -> android
 -> ios
 -> node_modules
 -> index.android.js
 -> index.ios.js
 
 index.android.js and index.ios.js are entry point to write code for android and ios respectively
```

## Navigator
```
This is the offical library used for all navigation
other popular Navigator is https://github.com/exponentjs/ex-navigator
```
# Flux
  Flux is the application architecture that Facebook uses for building client-side web applications.
  Flux is basically a pattren. it uses to persist states between different components and it follows uni-directional data     flow unlink other framework which support two way dataflow or binding like angularjs
  
  There exist many implementations for flux most common
  * Flux officially supported by facebook
  * Alt.js an imporved version flux
  * Redux most popular repositroy on facebook and even has more star as compared to flux
  There are many more for more detail take a look into https://github.com/voronianski/flux-comparison
  
## Production Setup
 * cd android && ./gradlew assembleRelease
 * react-native run-android --variant=release
 There are some pre-requisite to run these command which is written here
 https://facebook.github.io/react-native/docs/signed-apk-android.html
 
## Debugging
use `debugger` to put breakpoint and use chrome inspect element to check

## logs
see command line as well as red screen in case of error appears

Then:
Enjoy



