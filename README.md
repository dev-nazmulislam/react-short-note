# React Tutorial

1. [React Inastallation](https://github.com/dev-nazmulislam/react-short-note/tree/installation)
2. [React Fundamental Concepts](https://github.com/dev-nazmulislam/react-short-note/tree/react-fundamental)
3. [React Advanced concepts](https://github.com/dev-nazmulislam/react-short-note/tree/advanced)

# Advanced

### Add Firebase your project

1.  Create Firebase Project and register your app.
2.  Install SDK "npm install firebase"
3.  Initialize Firebase in your app and create a Firebase App object
4.  Initialize Firebase auth from firebase/auth. by const auth = getAuth(app)

### Use Firebase by Native providers

> Example: Email/Password, Phone, Anonymous.

### use Firebase by Additional providers

> Google, Facebook, Play Game, Game Center, Apple, Github, Microsoft, Twitter, Yahoo.

### Google Sign-in

1.  Enable Google as a sign-in method in the Firebase console.
2.  open auth section from firbase console.
3.  Create an instance of the Google provider object

```Js
import { GoogleAuthProvider } from "firebase/auth";
const provider = new GoogleAuthProvider();
```

4. To sign in with a pop-up window, call `signInWithPopup`

```Js
signInWithPopup(auth, provider)
  .then((result) => {
    const user = result.user;
  }).catch((error) => {
    console.log(error.message)
  });
```

5. To sign out a user, call `signOut`

```Js
import { getAuth, signOut } from "firebase/auth";

const auth = getAuth();
signOut(auth).then(() => {
  // Sign-out successful.
}).catch((error) => {
  // An error happened.
});
```

### GitHub Sign-in

1. In the Firebase console, open the Auth section.
2. On the Sign in method tab, enable the GitHub provider.
3. Add the Client ID and Client Secret from that provider's developer console to the provider configuration.
   - Register your app as a developer application on GitHub and get your app's OAuth 2.0 Client ID and Client Secret.
   - Make sure your Firebase OAuth redirect URI (e.g. my-app-12345.firebaseapp.com/auth/handler) is set as your Authorization callback URL in your app's settings page on your GitHub app's config.
4. Create an instance of the GitHub provider object.

```Js
import { GithubAuthProvider } from "firebase/auth";

const provider = new GithubAuthProvider();
```

5. To sign in with a pop-up window, call `signInWithPopup`

```Js
signInWithPopup(auth, provider)
  .then((result) => {
    const user = result.user;
  }).catch((error) => {
    console.log(error)
  });
```

6. To sign out a user, call `signOut`

```Js
import { getAuth, signOut } from "firebase/auth";

const auth = getAuth();
signOut(auth).then(() => {
  // Sign-out successful.
}).catch((error) => {
  // An error happened.
});
```

### Email/Password

1. On the Sign in method tab, enable the Email/password sign-in method and click Save.
2. Create a new account by passing the new user's email address and password to createUserWithEmailAndPassword

```Js
import { getAuth, createUserWithEmailAndPassword } from "firebase/auth";

const auth = getAuth();
createUserWithEmailAndPassword(auth, email, password)
  .then((result) => {
    const user = result.user;
  })
  .catch((error) => {
    consol.log(error)
  });
```

3. Sign in a user with an email address and password with `signInWithEmailAndPassword`

```Js
import { getAuth, signInWithEmailAndPassword } from "firebase/auth";

const auth = getAuth();
signInWithEmailAndPassword(auth, email, password)
  .then((result) => {
    // Signed in
    const user = result.user;
  })
  .catch((error) => {
    console.log(error)
  });
```

4. To sign out a user, call `signOut`

```Js
import { getAuth, signOut } from "firebase/auth";

const auth = getAuth();
signOut(auth).then(() => {
  // Sign-out successful.
}).catch((error) => {
  // An error happened.
});
```

### Conditional Randaring
