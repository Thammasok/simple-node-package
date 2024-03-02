# Simple Node Package

Example of node package tutorial

<https://www.freecodecamp.org/news/how-to-create-and-publish-your-first-npm-package>

---

## How to Test Your NPM Package

Testing ensures that your NPM package works as expected. There are many ways to test your package. In this tutorial, you will learn one of the simplest ways of testing.

First, navigate to the root of your package project. Then, run the following command:

```bash
npm link
```

This will make your package available globally. And you can require the package in a different project to test it out.

Create a example folder. And inside that test folder, add a index.js file.

In the example above, the example folder contains only the index.js file. It does not yet contain the package. To add the package you created to your example folder, run the command below:

```bash
npm link <name-of-package>
```

In the case of the example folder for this tutorial, I will run the following command:

```bash
npm simple-node-package
```

In the example/index.js file, you can now require your package and use it for the test.

```js
const helloNpm = require('simple-node-package')

console.log(helloNpm())
```

test run index.js

```bash
node example/index.js
```

---
