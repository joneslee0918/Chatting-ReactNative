# meteor-react-native-chat-example
Simple example of live chat through a Meteor server on both iOS and Android with React Native

***
#Screenshots
**** 
## Example with iOS

<image src="https://raw.githubusercontent.com/tgoldenberg/meteor-react-native-chat-example/master/meteor-chat-1.png" width="200px"/>
## Example with Android

<image src="https://raw.githubusercontent.com/tgoldenberg/meteor-react-native-chat-example/master/meteor-chat-2.png" width="200px"/>
*** 
## Setup 
****

- first `git clone` the repository locally
- to run the Meteor app, `cd meteor-chat-mtr`, type `meteor`, and open Chrome to `localhost:3000`
- to run the iOS app, from the root directory, `cd MeteorChatRN`, then type `ios/MeteorChatRN.xcodeproj` to open the project in XCode (you must have an up-to-date version of `XCode`), then hit the `play` icon to run the app in a simulator
- to run the Android app, first make sure the iOS Node server is not running (hit `stop` in XCode), then open an Android simulator (most users find `Genymotion` to be user-friendly). In your React-native root, type `react-native run-android` to run the app on the Android simulator

*** 
## Libraries used
**** 

#### For Meteor, the following packages were used - to add them to other projects just type `meteor add` + project name in your Meteor app
  - `checks` for server-side data checks
  - `react` for using React 
  - `react-template-helper` for including React components in Blaze templates
  - `iron:router` for routing
  - `accounts-password` for Meteor's easy-to-use user account management
  
### For React Native, the following libraries were used - to add them to other projects in React Native just type `npm install ` + package + `--save`
  - `react-native-navbar` for a reusable navbar on iOS and Android - note, to enable use on Android, you must comment out references in the library code to `TabBarIOS`
  - `react-native-invertible-scroll-view` for easy to implement UI in situations where you want to focus the screen towards the bottom of the `ScrollView`; this is particularly useful for chat applications
  - `ddp-client` for establishing a DDP connection with the remote Meteor server and adding to collections server-side
  - `react-native-vector-icons` for using MaterialIcon fonts as well as other icon fonts; the installation of this package for iOS and Android is distinct, but can easily be implemented through the source project instructions

**** 
# Contributing
**** 
- Feel free to contribute to the project by forking and making a pull request, there are plenty of improvements to be made!

****
# Shoutouts
**** 

- Thanks to Spencer Carli for the `meteor-todos-react-native` repository, which provides a great way of linking Meteor to React Native
