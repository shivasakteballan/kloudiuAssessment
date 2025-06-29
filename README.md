This is a new [**React Native**](https://reactnative.dev) project, bootstrapped using [`@react-native-community/cli`](https://github.com/react-native-community/cli).

# Getting Started

> **Note**: Make sure you have completed the [Set Up Your Environment](https://reactnative.dev/docs/set-up-your-environment) guide before proceeding.

## Step 1: Start Metro

First, you will need to run **Metro**, the JavaScript build tool for React Native.

To start the Metro dev server, run the following command from the root of your React Native project:

```sh
# Using npm
npm start

# OR using Yarn
yarn start
```

## Step 2: Build and run your app

With Metro running, open a new terminal window/pane from the root of your React Native project, and use one of the following commands to build and run your Android or iOS app:

### Android

```sh
# Using npm
npm run android

# OR using Yarn
yarn android
```

### iOS

For iOS, remember to install CocoaPods dependencies (this only needs to be run on first clone or after updating native deps).

The first time you create a new project, run the Ruby bundler to install CocoaPods itself:

```sh
bundle install
```

Then, and every time you update your native dependencies, run:

```sh
bundle exec pod install
```

For more information, please visit [CocoaPods Getting Started guide](https://guides.cocoapods.org/using/getting-started.html).

```sh
# Using npm
npm run ios

# OR using Yarn
yarn ios
```

If everything is set up correctly, you should see your new app running in the Android Emulator, iOS Simulator, or your connected device.

This is one way to run your app — you can also build it directly from Android Studio or Xcode.

## Requirements:

1. Authentication Context Setup
• Implement a AuthContext using React's Context API to manage the global (Done)
authentication state.
• The context should include:
o login: A function to log in a user. (Done)
o signup: A function to create a new user. (Done)
o logout: A function to log out the user. (Done)
o user: State to store the currently logged-in user's information. (Done)

1. Screens
2. Login Screen:
o Include input fields for:
§ Email (Done)
§ Password (Done)
o A "Login" button that triggers the login function from the AuthContext. (Done)
o Show error messages for:
§ Invalid email/password format. (Done)
§ Incorrect credentials. (Done)
o A "Go to Signup" button to navigate to the Signup screen. (Done)
1. Signup Screen:
o Include input fields for: (Done)
§ Name
§ Email
§ Password
o A "Signup" button that triggers the signup function from the AuthContext. (Done)
o Show error messages for:
§ Missing fields. (Done)
§ Invalid email format. (Done)
§ Password length less than 6 characters. (Done)
o A "Go to Login" button to navigate back to the Login screen. (Done)
1. Home Screen:
o Display the currently logged-in user's name and email. (Done)
o A "Logout" button to log out the user and return to the Login screen (Done)

1. Persist Authentication (optional)
• Use AsyncStorage to persist the authentication state so that the user remains logged in
after the app is closed and reopened. (Done)
1. Navigation
• Use React Navigation to manage navigation between:
o Login Screen (Done)
o Signup Screen (Done)
o Home Screen (Done)

1. UI Design
• Make the app visually appealing with clear layouts and intuitive navigation. (Done)
• Use appropriate styles for input fields, buttons, and error messages. (Done)

Bonus Tasks (Optional)
1. Password Visibility Toggle:
o Add an eye icon to toggle the visibility of the password field. (Done)
