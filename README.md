# React Tutorial

1. [React Inastallation](https://github.com/dev-nazmulislam/react-short-note/tree/installation)
2. [React Fundamental Concepts](https://github.com/dev-nazmulislam/react-short-note/tree/react-fundamental)
3. [React Advanced concepts](https://github.com/dev-nazmulislam/react-short-note/tree/advanced)

# React Fundamental

[What is react?](#what-is-react)

[Why we use React?](#why-we-use-react)

[Benefits of single page aplications.](#benefits-of-single-page-aplications)

[React JSX](#what-is-jsx)

[React Component](#what-is-component)

[React properties](#what-is-react-properties)

[React Hooks](#what-is-react-hooks)

[React state](#what-is-react-state)

[Event in react](#what-is-event-in-react)

[Add css in react jsx](#add-css-in-react-jsx)

### What is react?

<small><a href="#react-tutorial">Top</a></small>
<small><a href="#why-we-use-react">Next</a></small>

> React is a flexible, efficient, open-sourse JavaScript library for building user interfaces.

### Why we use React?

<small><a href="#react-tutorial">Top</a></small>
<small><a href="#benefits-of-single-page-aplications">Next</a></small>

> React allows developers to create large web applications that can change data, without reloading the page. The main purpose of React is to be fast, scalable, and simple. It works only on user interfaces in the application.

### Benefits of single page aplications.

<small><a href="#react-tutorial">Top</a></small>
<small><a href="#what-is-jsx">Next</a></small>

1. Quick Loading Time.
2. Seamless User Experience.
3. Ease in Building Feature-rich Apps.
4. Uses Less Bandwidth.

### What is JSX?

<small><a href="#react-tutorial">Top</a></small>
<small><a href="#what-is-component">Next</a></small>

> JSX stands for JavaScript XML. JSX allows us to write HTML in React. JSX makes it easier to write and add HTML in React. Return a single element (only one parent element)

[JSX Element](#jsx-element) | [JavaScript in JSX](#javascript-in-jsx) | [JSX Expressions](#jsx-expressions) | [JSX attributes](#jsx-attributes) | [JSX Functions](#jsx-functions) | [JSX Conditional rendering](#jsx-conditional-rendering).

#### JSX Element

```Js
let element = <h1>Hello, world!</h1>;
let emptyHeading = <h1 />;
```

#### JSX Expressions

```Js
let name = 'Josh Perez';
let element = <h1>Hello, {name}</h1>;

function fullName(firstName, lastName) {
  return firstName + ' ' + lastName;
}
let element = <h1>Hello, {fullName('Julie', 'Johnson')}</h1>
```

#### JSX attributes

```Js
const element = <img src={user.avatarUrl} />;
const element = <button className="btn">Click me</button>;
```

#### JSX Functions

```Js
name() {
  return "Julie";
}

return (
  <h1>
    Hi {name()}!
  </h1>
)
```

#### JSX Conditional rendering

```Js
import React from "react";
export default function Weather(props) {
  if (props.temperature >= 20) {
    return (
      <p>
        It is {props.temperature}°C (Warm) in {props.city}
      </p>
    );
  } else {
    return (
      <p>
        It is {props.temperature}°C in {props.city}
      </p>
    );
  }
}

```

#### Javascript in JSX

```Js
function App(){
    const name = 'Mike'
    return (
      <>
          <h1>Hello {name}</h1>
          <p>{name === 'Mike' ? '(admin)': '(user)'}</p>
      </>
    )
}
```

### What is component?

<small><a href="#react-tutorial">Top</a></small>
<small><a href="#what-is-react-properties">Next</a></small>

> Components are independent and reusable bits of code. They serve the same purpose as JavaScript functions, but work in isolation and return HTML. Components come in two types, Class components and Function components.

#### Class Components

> Class components can define functions that will execute during the component's lifecycle.

#### Creating a class component

```Js
// MyComponent.js
import React, { Component } from 'react';

class MyComponent extends Component {
  render() {
    return (
      <div>This is my component.</div>
    );
  }
}
export default MyComponent;
```

#### Functional component

> A functional component is basically a JavaScript/ES6 function that returns a React element (JSX). According to React's official docs.

#### Creating a Functional component

```Js
import React from 'react';

function UserProfile() {
  return (
      <div className="UserProfile">
        <div>Hello</div>
        <div>World</div>
     </div>
  );
}
export default UserProfile;
```

#### Making an Interactive Component

#### Embed an internal component

```Js
import React from 'react';
import UserAvatar from "./UserAvatar";

export default function UserProfile() {
  return (
      <div className="UserProfile">
        <UserAvatar />
        <UserAvatar />
      </div>
  );
}
```

#### Embed an external component

```Js
import React from 'react';
import ComponentName from 'component-name';

export default function UserProfile() {
  return (
      <div className="UserProfile">
        <ComponentName />
      </div>
  );
}
```

#### Nested Components

### What is react properties?

<small><a href="#react-tutorial">Top</a></small>
<small><a href="#what-is-react-hooks">Next</a></small>

> It is an object which stores the value of attributes of a tag and work similar to the HTML attributes. It gives a way to pass data from one component to other components. It is similar to function arguments. Props are passed to the component in the same way as arguments passed in a function.

#### Passing properties to a component

```Js
<Student firstName="Julie" lastName="Johnson" age={23} pro={true} />
```

#### Accessing the properties from a component

```Js
import React from "react";

export default function Student(props) {
  return (
    <h1>
      {props.firstName} {props.lastName} is {props.age}.
    </h1>
  )
}
```

#### Default Props value

```Js
const Person = ({name, age, children}) => {
    return (
        <h1>Name: {name} Age: {age}</h1>
        <p>{children}</p>
    )
}

Person.defaultProps = {
    name: 'No name',
    age: 0,
}
```

#### Props object destructuring

### What is react hooks?

<small><a href="#react-tutorial">Top</a></small>
<small><a href="#what-is-react-state">Next</a></small>

[useState](#usestate) | [useEffect](#useeffect) | [useRef](#useref) | [useCallback](#usecallback) | [useMemo](#usememo) | [useContext](#usecontext) | [useReducer](#usereducer) | [Custom Hooks](#custom-hooks)

#### useState

#### useEffect

#### useRef

#### useCallback

#### useMemo

#### useContext

#### useReducer

#### Custom Hooks

### What is react state?

<small><a href="#react-tutorial">Top</a></small>
<small><a href="what-is-react-routing">Next</a></small>

> State is a plain JavaScript object used by React to represent an information about the component's current situation. It's managed in the component (just like any variable declared in a function).

#### React state

```Js
import React, { useState } from "react";

export default function Hello(props) {
  let [name, setName] = useState("Julie");
  function updateName() {
    let newName = prompt("What is your name?");
    setName(newName);
  }

  return (
    <h1>
      {name}
    </h1>
    <button onClick={updateName}>
      Update name
    </button>
  );
}
```

### What is react routing?

<small><a href="#react-tutorial">Top</a></small>
<small><a href="#what-is-event-in-react">Next</a></small>

> React Router is a standard library for routing in React. It enables the navigation among views of various components in a React Application, allows changing the browser URL, and keeps the UI in sync with the URL.

### What is event in react?

<small><a href="#react-tutorial">Top</a></small>
<small><a href="#add-css-in-react-jsx">Next</a></small>

> An event is an action that could be triggered as a result of the user action or system generated event.

#### Event listener

```Js
import React from "react";

export default function Hello() {
  function handleClick(event) {
    event.preventDefault();
    alert("Hello World");
  }

  return (
    <a href="/" onClick={handleClick}>
      Say Hi
    </a>
  );
}
```

### Add css in react jsx

<small><a href="#react-tutorial">Top</a></small>
