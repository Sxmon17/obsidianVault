#Coding #React

# Components and Props
https://reactjs.org/docs/components-and-props.html

## Summary
Mit Components kannst du dein UI in unabhängige, wiederverwendbare Teile trennen und isolieren.

Components sind im Prinzip JS Funktionen, nur dass sie props akzeptieren und sie returnen React Elemente, welche beschreiben was auf dem Bildschirm erscheint.

## Templates
### Class Component
```Javascript
class Main extends React.Component {
    constructor(props) {
        super(props);
        this.state = {};
    }
    render() {
        return ();
    }
}
```

### Function
```Javascript
function App() {
    return (
        <div></div>
    );
}
```