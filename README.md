React
# React Native Tutorial
- from `React Native Tutorial #1 - Introduction` by `The Net Ninja`

## Lessons
- [Github Lessons](https://www.github.com/iamshaunjp/react-native-tutorial)
- Different stopping points are available in branches

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

```sh
expo init <your-project-name>
# asks for a project template (choose blank)
# asks for a name for the project
# follow the prompt
```
```sh
cd <your-project-name>
npm start
```