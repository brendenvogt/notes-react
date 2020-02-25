# Text Inputs
[Docs](https://reactnative.dev/docs/textinput)

## Goal
- Create a Text component, and a Text Input component.
- Update the Text component whenever the TextInput component text changes.

Start with this.
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

Use what we know from our `useState` tutorial to create a piece of state.
``` javascript
// 1. Import useState
import React, { useState } from 'react';
import { StyleSheet, Text, View } from 'react-native';

export default function App() {
    // 2. Make a piece of state
    const [name, setName] = useState("");

    // 4. Use the piece of state
    return (
        <View style={styles.container}>
            <Text>My name is: {name}</Text>
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

That should've gotten us close. Now lets get our input field.
``` javascript
import React, { useState } from 'react';
// 1. Import TextInput from react-native
import { StyleSheet, Text, View, TextInput } from 'react-native';

export default function App() {
    const [name, setName] = useState("");

    // 2. Add a TextInput (which is self closing)
    // Add a placeholder text and an onChangeText event
    return (
        <View style={styles.container}>
            <Text>My name is: {name}</Text>
            <TextInput 
                style={styles.input}
                placeholder='e.g. John Doe' 
                onChangeText={(val)=> setName(val)}/>
        </View>
    );
}

// 3. Adding a style as well
const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#fff',
    alignItems: 'center',
    justifyContent: 'center'
  },
  input {
      borderWidth: 1,
      borderColor: '#777',
      padding: 8, 
      margin: 10,
      width: 200
  }
});
```

### Other Attributes for TextInput
- 

# Recap
- Import TextInput
``` javascript
import { TextInput } from 'react-native';
```
- Add the TextInput component
``` javascript
<TextInput 
    style={styles.input}
    placeholder='e.g. John Doe' 
    onChangeText={(val)=> setName(val)}/>
```
