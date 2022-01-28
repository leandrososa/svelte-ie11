# Svelte v3 + Tailwind 1.9 + Fetch support in IE11

![image](https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00) ![image](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white
)

Svelte JS Rollup Config for IE11 Support via `rollup-plugin-babel ` and Tailwind 1.9 purged with postcss & postcss-cli.
Also allow support for Async/Await Syntax. Usefuell if your App needs to run on some sort of embeded Systems.

## How to use

```js
  // Clone boilerplate with degit
  npx degit https://github.com/leandrososa/svelte-tailwind-ie11 your-project-name

  // Git init & npm install
  git init
  npm i
```

## Project info
#### Fetch Support

```js
// src/main.js
import App from './App.svelte'
import 'whatwg-fetch' // fetch polyfill for IE 11

export default new App({
  target: document.body,
})
```

#### Config

You can disable IE11 Support via ``rollup.config.js`

```js
...
const legacySupport = true // enable for IE11 Support
...
```

#### Dependencies

```
  "devDependencies": {
    "@rollup/plugin-commonjs": "^21.0.1",
    "@rollup/plugin-node-resolve": "^13.0.6",
    "concurrently": "^7.0.0",
    "postcss": "^8.4.5",
    "postcss-cli": "^9.1.0",
    "prettier": "^2.5.1",
    "prettier-plugin-svelte": "^2.6.0",
    "rollup": "^2.60.0",
    "rollup-plugin-css-only": "^3.1.0",
    "rollup-plugin-livereload": "^2.0.5",
    "rollup-plugin-svelte": "^7.1.0",
    "rollup-plugin-terser": "^7.0.2",
    "svelte": "^3.44.2",
    "tailwindcss": "^1.9.6"
  },
  "dependencies": {
    "@babel/core": "^7.16.0",
    "@babel/plugin-syntax-dynamic-import": "^7.8.3",
    "@babel/plugin-transform-runtime": "^7.16.4",
    "@babel/preset-env": "^7.16.4",
    "@babel/runtime": "^7.16.3",
    "@fullhuman/postcss-purgecss": "^4.1.3",
    "@rollup/plugin-babel": "^5.3.0",
    "core-js": "3",
    "history": "^5.2.0",
    "rollup-plugin-babel": "^4.3.3",
    "sirv-cli": "^1.0.14",
    "svelte-navigator": "^3.1.5",
    "svelte-preprocess": "^4.10.2",
    "vconsole": "^3.11.2",
    "whatwg-fetch": "^3.6.2"
  }
```
