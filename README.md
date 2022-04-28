# React Tutorial

1. [React Fundamental Concepts](https://github.com/dev-nazmulislam/react-short-note/tree/react-fundamental)
2. [React Advanced concepts](https://github.com/dev-nazmulislam/react-short-note/tree/advanced)

# Installation for client side with website link

1.  [Create React App](#creact-react-app)
2.  [Router](#react-router)
3.  [React Bootstrap](#react-bootstrap)
4.  [React tailwind](#react-taillwind)
5.  [Firebase](#firebase)
6.  [React Firebase Hooks](#react-firebase-hooks)
7.  [React hooks form](#React-hooks-form)
8.  [React Icons](react-icons)
9.  [react-hot-toast](#react-hot-toast)
10. [Rechart](#react-recharts)

# Installation for server side with website link

1. [Server setup with mongodb atlas](#server-setup-with-mongodb-atlas)
2. [Express](#express)
3. [Nodemon](#nodemon)
4. [Cors](#cors)
5. [Mongodb](#mongodb)
6. [dotenv](#dotenv)

# Herouku deploy

### One Time for your computer

1. Create Herouku account.
2. Install herouku CLI.
3. Download & install herouku app.
4. Check some task on client side.
5. herouku login.
6. herouku create.
7. git push herouku main.

### For each Projects one time.

1. herouku create.
2. Make sure your git add, git commit, git push up to date.
3. git push herouku main.
4. Go to Dashboard > Current Projects > Settings > Reveal Config Vars and add .env file.

### Update Server with new changes.

1. Make Change.
2. Make sure your git add, git commit, git push up to date.
3. git push herouku main.

### Connect server with client side & deply firebase.

1. Replace locall host with herouku link.
2. npm run build.
3. firebase deploy.

# Get Started

### [Creact React App](https://react-bootstrap.github.io/)

```Js
npx create-react-app my-app
```

### [React Router](https://reactrouter.com/docs/en/v6/getting-started/overview)

```Js
npm install react-router-dom@6
```

### [React Bootstrap](https://react-bootstrap.github.io/)

> 2 Way to install react bootstrap to your projects

1. Install bootstrap with cdn (Place bootstrap cdn link in index file.)
1. Install bootstrap with npm & place css link in your app.js or index.js.

### installation with npm command

```
npm install react-bootstrap bootstrap@5.1.3
```

### Import CSS file

```
import 'bootstrap/dist/css/bootstrap.min.css';
```

### installation with cdn

#### Import Css file

```Html
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-1BmE4kWBq78iYhFldvKuhfTAU6auU8tT94WrHftjDbrCEXSU1oBoqyl2QvZ6jIW3" crossorigin="anonymous">
```

#### Import js file

```Html
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ka7Sk0Gln4gmtz2MlQnikT1wXgYsOg+OMhuP+IlRH9sENBO0LRn5q+8nbTov4+1p" crossorigin="anonymous"></script>
```

### [React Taillwind](https://tailwindcss.com/docs/guides/create-react-app)

#### install with cdn

> Add the CDN script tag to the <head> of your HTML file, and start using Tailwind’s utility classes to style your content.

```Html
  <script src="https://cdn.tailwindcss.com"></script>
```

#### Install with CLI

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

### [Firebase](https://firebase.google.com/)

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

### [React Firebase Hooks](https://github.com/CSFrequency/react-firebase-hooks)

```Js
npm install --save react-firebase-hooks
```

### [React hooks form](https://react-hook-form.com/)

```Js
npm install react-hook-form
```

### [React Icons](https://react-icons.github.io/react-icons/)

```Js
npm install react-icons --save
```

- import react icons

```Js
import { FaBeer } from 'react-icons/fa';
```

### [react-hot-toast](https://react-hot-toast.com/)

```Js
npm install react-hot-toast
```

### [React Recharts](https://recharts.org/en-US/)

```
npm install recharts
```

### [Server setup with mongodb atlas](https://www.mongodb.com/atlas/database)

[mongodb doc](https://www.mongodb.com/docs/drivers/node/current/)

- Create folder
- npm init
- Creacte index.js file
- Add some script on pakage.json file

```Js
"start":"node index.js",
"start-dev":"nodemon index.js"
```

- Create MongoDB Atlas Account with 5 steeps

  1. sign up. with google access.
  2. create cluster.
  3. Create user & password.
  4. Network Access --> ip address: allow all.
  5. database > Connect > code copy paste in index.js

### [Express](https://expressjs.com/)

```Js
npm install express
```

### [Nodemon](https://www.npmjs.com/package/nodemon)

```Js
npm install -g nodemon
```

### [Cors](http://expressjs.com/en/resources/middleware/cors.html)

```Js
npm install cors
```

### [Mongodb](https://www.mongodb.com/docs/drivers/node/current/)

```Js
npm install mongodb
```

### [dotenv](https://www.npmjs.com/package/dotenv)

```Js
npm install dotenv --save
```
