# State & React Hooks

### Import the useState Helper
``` Javascript
// 1. import useState from react
import React, { useState } from 'react';
import { StyleSheet, Text, View } from 'react-native';

export default function App() {
    // 2. declare your piece of state
    const [name, setName] = useState('bob');

    return (
        <View style={styles.container}>
            <Text></Text>
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
- Here we import useState which helps us instantiate a new state object 
- useState takes in an initial value and assigns it to the first element in the array (i.e. name) and useState assigns a setter to the second element in the array (i.e. setName)

### Use the State Object
``` Javascript
import React from 'react';
import { StyleSheet, Text, View } from 'react-native';

export default function App() {
    const [name, setName] = useState('bob');
 
    // 3. Here we use the 'name' variable inside curly brackets to use the value inside the variable
    return (
        <View style={styles.container}>
            <Text>My name is {name}</Text>
            <Text></Text>
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

### Add a Button To Set the Name
```javascript
import React from 'react';
import { StyleSheet, Text, View } from 'react-native';

export default function App() {
    const [name, setName] = useState('bob');
 
    // 6. define our click handler outside the view block
    const clickHandler = () => {
        setName('bobby');
    }

    // 4. Here we add a View Component and a Button component. 
    // Notice that a Button is a self closing component, and its title is set using the title attribute.
    return (
        <View style={styles.container}>
            <Text>My name is {name}</Text>
            <Text></Text>
            <View style={styles.buttonContainer}>
                <Button title='Update State' onPress={clickHandler}/>
            </View>
        </View>
        // 5. Styles cannot be placed on buttons directly, only a view section around the button.
    );
};

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#fff',
    alignItems: 'center',
    justifyContent: 'center'
  },
  buttonContainer: {
      marginTop: 20
  }
});
```


### Add a Button To Set the Name
```javascript
import React from 'react';
import { StyleSheet, Text, View } from 'react-native';

export default function App() {
    const [name, setName] = useState('bob');
    // 7. More state
    const [item, setItem] = useState({category: 'food', name: 'pizza'});

    const clickHandler = () => {
        setName('bobby');
        // 8. Set State. Note you must supply all the parameters
        setItem({ name: 'hotdogs', category: 'food'});
    }

    // 9. Use the variables {item.category} and {item.name}
    return (
        <View style={styles.container}>
            <Text>My name is {name}</Text>
            <Text>And my favorite {item.category} is {item.name}</Text>
            <View style={styles.buttonContainer}>
                <Button title='Update State' onPress={clickHandler}/>
            </View>
        </View>
    );
}

const styles = StyleSheet.create({
  container: {
    flex: 1,
    backgroundColor: '#fff',
    alignItems: 'center',
    justifyContent: 'center'
  },
  buttonContainer: {
      marginTop: 20
  }
});
```

# Recap
- Import `useState` 
``` javascript
import React, { useState } from 'react';
```
- Create our bit of state
``` javascript
const [name, setName] = useState("bob");
```
- Update the state using the handler
``` javascript
const clickHandler = () => {
    setName("new name");
}
    
//...
return ( 
    <View>
        <Button title="Update Name" onPress={clickHandler} />
    </View>
);
//...
```
