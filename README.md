# React Tutorial

1. [React Fundamental Concepts](https://github.com/dev-nazmulislam/react-short-note/tree/react-fundamental)
2. [React Advanced concepts](https://github.com/dev-nazmulislam/react-short-note/tree/advanced)

# installation

1.  [Install React](https://reactjs.org/docs/getting-started.html)
2.  [Install react bootstrap](https://react-bootstrap.github.io/getting-started/introduction)
3.  [Install react Tailwind](https://tailwindcss.com/docs/installation)
4.  [Recharts installation](https://recharts.org/en-US/guide)

## React Bootstrap Installation

> 2 Way to install react bootstrap to your projects

1. Install bootstrap with cdn (Place bootstrap cdn link in index file.)
2. Install bootstrap with npm & place css link in your app.js or index.js.

### Bootstrap installation npm command

```
npm install react-bootstrap bootstrap@5.1.3
```

### Import CSS file

```
import 'bootstrap/dist/css/bootstrap.min.css';
```

### Bootstrap installation with cdn

#### Import Css file

```Html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">
```

#### Import js file

```Html
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p" crossorigin="anonymous"></script>
```

## React Taillwind Installation

### install with cdn

> Add the CDN script tag to the <head> of your HTML file, and start using Tailwind’s utility classes to style your content.

```Html
  <script src="https://cdn.tailwindcss.com"></script>
```

### Install with CLI

1. Install Tailwind & Tailwind configaration with npm

```
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

2. Replace content line in tailwind.config.js file

```
content: [
    "./src/**/*.{js,jsx,ts,tsx}",
  ],
```

3. Add tailwind directives to your index.css file. Then injoy & npm run start.

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

## React Recharts Installation

### NPM

```
npm install recharts
```

# Project template instalation

### Install for Client

1. React

```Js
npx create-react-app my-app
```

2. React Router

```Js
npm install react-router-dom@6
```

3. React Bootstrap

   > 2 Way to install react bootstrap to your projects

1. Install bootstrap with cdn (Place bootstrap cdn link in index file.)
1. Install bootstrap with npm & place css link in your app.js or index.js.

### Bootstrap installation npm command

```
npm install react-bootstrap bootstrap@5.1.3
```

### Import CSS file

```
import 'bootstrap/dist/css/bootstrap.min.css';
```

### Bootstrap installation with cdn

#### Import Css file

```Html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">
```

#### Import js file

```Html
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p" crossorigin="anonymous"></script>
```

4. React Taillwind

### install with cdn

> Add the CDN script tag to the <head> of your HTML file, and start using Tailwind’s utility classes to style your content.

```Html
  <script src="https://cdn.tailwindcss.com"></script>
```

### Install with CLI

1. Install Tailwind & Tailwind configaration with npm

```
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p
```

2. Replace content line in tailwind.config.js file

```
content: [
    "./src/**/*.{js,jsx,ts,tsx}",
  ],
```

3. Add tailwind directives to your index.css file. Then injoy & npm run start.

```
@tailwind base;
@tailwind components;
@tailwind utilities;
```

5. Firebase

- Create Firebase Project and register your app.
- Install SDK

```Js
npm install firebase
```

- Initialize Firebase in your app and create a Firebase App object.
- Initialize Firebase auth from firebase/auth.

```Js
import { getAuth } from "firebase/auth";
const auth = getAuth(app)
```

6. React Firebase Hooks

```Js
npm install --save react-firebase-hooks
```

7. React hooks form

```Js
npm install react-hook-form
```

8. React Icons

```Js
npm install react-icons --save
```

- import react icons

```Js
import { FaBeer } from 'react-icons/fa';
```

9. react-hot-toast

```Js
npm install react-hot-toast
```
