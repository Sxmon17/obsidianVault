#Coding #React 

# React

## Basic concepts
### Components and Props
[[React Components]]
https://reactjs.org/docs/components-and-props.html

## Templates
### Basic Starter 
```javascript
import React from "react";
import ReactDOM from "react-dom";
import "./index.css";
class Main extends React.Component {
    render() {
        return ();
    }
}
// ========================================

const container = document.getElementById("root");
const root = ReactDOM.createRoot(container);
root.render(<Main />);
```

### Map a List
```Javascript
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
    <li>{number}</li>
);
```

### Eventhandler
```Javascript
function handleSubmit = () => {
    console.log('this is: ', this)
}
```
