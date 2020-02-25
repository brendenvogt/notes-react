React
# React Native Tutorial
- from `React Native Tutorial #1 - Introduction` by `The Net Ninja`

## Lessons
- Github
  - [Github Lessons](https://www.github.com/iamshaunjp/react-native-tutorial)
  - Different stopping points are available in branches
- Expo.io
  - [Expo.io](https://expo.io) and the [tutorial](https://expo.io/learn)
  - Flow
    - Fall in Love by using Snack
    - Download NodeJS
    - Get the command line tool
    - Create your first project
    - Preview your project
      - `expo start` will produce a QR code which you can use to preview your app on your phone
    - Start coding
    - Further Learning
      - Routing and Navigation
      - Up & Running
      - Debugging
## Things to learn 
- React Hooks
  - `useState` hook
- React Context
### Extra things 
- Flutter

## How React Works
- Construct various components
- Chain together components in the form of a tree structure
- Pass data between components by using props or other means
- Example
  - App Component can have two sub components
    - Header Component
    - Content Component (Which has two components)
      - Text Component (receives data from props)
      - Text Component (receives data from props)


# Install
## One Time Install
- Install Node on Computer (we need npm the `Node Package Manager`)
- Android Studio (for android development)
- XCode (for iOS development)
- VSCode (for our development IDE)
  - Packages: 
    - ES7 React/Redux/GraphQL/React-Native snippets

- ReactNative Tools
  - ExpoCLI (very helpful in creating a base standard React Application)
    - install expo
```sh
# Install expo globally
npm install expo-cli --global
```

## New Project
### initialize new project  
```sh
expo init <your-project-name>
# asks for a project template (choose blank)
# asks for a name for the project
# follow the prompt
```
### change directory into the directory
```sh
cd <your-project-name>
```
### optional open vscode
```sh
code .
```
### start your application
```sh
# open vscode using code .
npm start
# This runs `expo start` under the hood
```
### Navigate to `localhost:19002`

## View App on iPhone Expo Client
- `Expo Client` by `Nametag`
- Scan the QR code created by `expo start`

## View App on Android using Android Studio Virtual Devices 
- Install Android Studio
- Navigate to AVD Manager (Android Virtual Device Manager)
  - Create a virtual device of a certain device and API firmware
  - Name the device and finish
  - Start the device
- Keep the emulator open
- Go to the Expo window
- Click on `Run on android device or emulator`
- The emulator is going to ask to install Expo
- if prompted, you will need to go back and click `Run on android device or emulator` again.

# Development
## Files and Directory Overview
- Assets
- node_modules