# 3 COMPONENTS The Core Part of React

### In `package.json`

There are `dependencies`, `scripts`, and `versions`.

There are `react` and `react-dom` dependencies, which successfully run our React code.

```
package.json

src/
  app.js
  index.css
  index.js

public/
  index.html

node_modules
```

Whenever a page loads, `index.js` is first loaded.

`index.css` is nothing; it just provides class and id for `index.js`.

JSX is JavaScript XML.

`app.js` or `app.jsx` is for the app component, where all the codes will be sent for rendering (for showing).

!\[]\[image2]

!\[]\[image3]

## Component creation in `Item.jsx`

Go and create `components` folder.\
Add `Item.jsx` and `Item.css`.

To import/add any file:

```js
import './Item.css';
```

### Function creation

After creating function, we also need to put `export` below it.

```javascript
function SomeThing(){  
  return(  
 <div>  
 <p>Hello Buddy</p>  
 </div>  
  );  
}

export default Something;
```

Note: `<p className="okaa">hey</p>` — when writing class for adding CSS, we have to write `className`.

## Component using in `App.jsx`

### For importing component

Okay, so to import a component:

```js
import Item from './components/Item.jsx';
```

### Calling the component

Go in `App.jsx` and insert `<> </>` with its name:

```js
return(  
  <div>  
<Item></Item>  
	……………..  
	……………..  
	……………..  
  </div>  
);
```

## How to reuse component???

Passing Props
