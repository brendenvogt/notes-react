
# Development Intro
## Files and Directory Overview
- `expo` - configuration and settings.
- `expo-shared` - configuration and settings.
- `assets` - contains any images or media that we want to use in our app later.
- `node_modules` - the directory where our node module dependencies will be populated.
- `.gitignore` - Standard gitignore for node-modules directory and other items.
- `App.js` - Root component of our react app.
- `app.json` - info about the project (name, supported platforms, version, supported orientations, etc.)
- `babel.config.js` - configures how babel works with this project.
  - Babel is a javascript compiler used for modern javascript.
- `package-lock.json`
- `package.json` - Our standard package.json, specifying things like our scripts, dependencies, and our app entry.

## App.js
This is our entry point
``` javascript
import React from 'react';
import { StyleSheet, Text, View } from 'react-native';

export default function App() {
  return (
    <View style={styles.container}>
      <Text> Open up App.js to start working on you app!</Text>
    </View>
  );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#fff',
    alignItems: 'center',
    justifyContent: 'center'
  }
});
```

## Components
### The `View` Component
[Docs](https://reactnative.dev/docs/view)

This component is similar to a `<div>` tag in HTML. It denotes a virtual container around other things.
``` js
(<View>
  <Text>Hello World</Text>
</View>)
```

### The `Text` Component
[Docs](https://reactnative.dev/docs/text)

This component is the simplest component for holding text. This is similar to the `<p>` tag in HTML as it is a simple container for holding text.
``` Javascript
(<Text>Hello World</Text>)
```

## Styles
[Docs](https://reactnative.dev/docs/stylesheet)

``` javascript
const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#fff',
    alignItems: 'center',
    justifyContent: 'center'
  }
});
```