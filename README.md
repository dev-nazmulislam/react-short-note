## [React Advanced](https://github.com/dev-nazmulislam/react-short-note/tree/react-advanced)

## [React installation](https://github.com/dev-nazmulislam/react-short-note/tree/react-installation)

# React Fundamental

[What is react?](#what-is-react)

[Why we use React?](#why-we-use-react)

[Benefits of single page aplications.](#benefits-of-single-page-aplications)

[What is component?](#what-is-component)

[What is JSX?](#what-is-jsx)

[What is react props?](#what-is-react-props)

[What is react state?](#what-is-react-state)

[What is event in react?](#what-is-event-in-react)

[add css in react jsx](#add-css-in-react-jsx)

### What is react?

> React is a flexible, efficient, open-sourse JavaScript library for building user interfaces.

### Why we use React?

> React allows developers to create large web applications that can change data, without reloading the page. The main purpose of React is to be fast, scalable, and simple. It works only on user interfaces in the application.

### Benefits of single page aplications.

1. Quick Loading Time.
2. Seamless User Experience.
3. Ease in Building Feature-rich Apps.
4. Uses Less Bandwidth.

### What is component?

> Components are independent and reusable bits of code. They serve the same purpose as JavaScript functions, but work in isolation and return HTML. Components come in two types, Class components and Function components.

#### Functional component

```Js
import React from 'react';

export default function UserProfile() {
  return (
      <div className="UserProfile">
        <div>Hello</div>
        <div>World</div>
     </div>
  );
}
```

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

### What is JSX?

> JSX stands for JavaScript XML. JSX allows us to write HTML in React. JSX makes it easier to write and add HTML in React. Return a single element (only one parent element)

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

### What is react props?

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

### What is react state?

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

> React Router is a standard library for routing in React. It enables the navigation among views of various components in a React Application, allows changing the browser URL, and keeps the UI in sync with the URL.

### What is event in react?

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

### add css in react jsx
