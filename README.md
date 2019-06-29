# ESLint Prettier Boilerplate

Starter repository for a JS project using ESLint and Prettier recommended rules
and styles.

## Installation

Clone the Git repository.

```
git clone https://github.com/travishorn/eslint-prettier-boilerplate.git
```

Install the dependencies.

```
npm install
```

Since you are probably using this as a base for a new project, you probably also want to remove the git history.

On Linux/Mac:

```
rm -rf .git
```

On Windows:

```
rmdir /S .git
```

## Usage

Start developing.

Any files with extension `.js` can be linted against ESLint and Prettier
recommended rules.

```
npm run lint
```

You can automatically fix some problems.

```
npm run lint:fix
```

## Editor Setup

If you're using Visual Studio Code, you can install the ESLint extension, which
will automatically highlight warnings and errors using this boilerplate.

1. Press **Ctrl + Shift + X** or click the **Extensions** button
2. Search for **ESLint**
3. Click the **Install** button next to the **ESLint** search result

With this extension, you can also choose to automatically fix/format your code
when you save. Add the following to your Visual Studio Code settings.

```
"eslint.autoFixOnSave": true
```

This setting only takes effect if  `files.autoSave` is set to `off`,
`onFocusChange`, or `onWindowChange`.

## Manual Setup (without using this repository)

Initialize an npm package.

```
npm init -y
```

Install development dependencies

```
npm i -D eslint eslint-config-prettier eslint-plugin-prettier prettier
```

Create `.eslintrc.js` in project root.

```
module.exports = {
  "extends": [
    "eslint:recommended",
    "plugin:prettier/recommended"
  ],
  "env": {
    "es6": true,
    "node": true
  },
  "parserOptions": {
    "ecmaVersion": 8
  }
};
```

## License

Copyright 2019 Travis Horn

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
