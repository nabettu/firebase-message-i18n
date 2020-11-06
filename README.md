# firebase-message-i18n

## Installation

Using npm

```
$ npm i firebase-message-i18n
```

Using yarn

```
$ yarn add firebase-message-i18n
```

## Usage

```js
import firebase from "firebase";
import firebaseMessage from "firebase-message-i18n/ja-jp.json";

firebase
  .auth()
  .signInWithEmailAndPassword("email", "password")
  .catch(e => {
    const errorText = firebaseMessage[e.code] || e.message;
    alert(errorText);
  });
```

## Contribution

Please make a pull request.

## License

[MIT](https://opensource.org/licenses/MIT)
