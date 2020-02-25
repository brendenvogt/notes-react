
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
