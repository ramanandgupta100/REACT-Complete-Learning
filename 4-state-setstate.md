# 4 STATE setState ( )

## How to use State?

In `App.jsx`

```javascript
import './App.css';
let x = 10;

function App() {
  function updateState() {
    x = 15;
  }

  return (
    <div>
      <h1>Heading {x}</h1>
      <button onClick={updateState}>click me</button>
    </div>
  );
}
```

## useState()

`useState` is hook, it is used with functional component (utility function).

**How to know if something is hook or what?**

There will be **use…Something..** before any useState's name.

Note: We cannot use useState under if/else condition.

#### importing useState()

```javascript
import { useState } from 'react';
import React from 'react';
```

## Using useState()

We initialize our state by calling `useState` in our function component.

`useState` accepts an initial state and returns two values:

1. The current state.
2. A function that updates the state.

```javascript
function FavoriteColor() {
  const [color, setColor] = useState("");
}
```

* The first value, `color`, is our current state.
* The second value, `setColor`, is the function that is used to update our state.
* Lastly, we set the initial state to an empty string: `useState(' ')`

## A COMPLETE USE CASE

```javascript
App.jsx
import './App.css';
import {useState} from 'react';
import React from 'react';

function App(){
 const [count, setCounter] = useState()
 
   function updateCount(){
   setcounter(count+1)
    }

return(
 <div>
   <h1>Button Clicked {count} times </h1>
   <button onClick={updateCount}>Click</button>

 </div>

);
}

export default App;
```
