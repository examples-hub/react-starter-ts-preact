# react-starter-ts

> simple starter boilerplate for react using typescript

# overview
- features
  - 😎️ switch between react(v17) and preact(v10) out of the box
  - simple react starter boilerplate
  - support react/preact hot reloading
  - built with react/preact + typescript + babel + webpack(v5) from scratch
    - pre-configured with code quality tools: eslint, prettier, jest, etc.

---

- css-in-js not baked in
  - css is using scss/css
- no state management library baked in
  - hooks are enough for simple apps
- no routing baked in
- codebase structure is unopinionated
  - the starter app is very simple with little code
  - no third party react component library baked in

> 🤗️ if you want to start with a batteries-included react app, you can have a look at my project prospect-garden-dashboard(WIP)

# usage

```shell
npm i

# start react app
npm run start

# start preact app
npm run start2
```

- open http://localhost:8999/
# notes
- only a few `scripts` in `package.json` work; just write your own
- if the app is started with preact env
  - .tsx/.scss hot reloading is supported
  - Preact Devtools is supported; but you need to install the [preact browser extension](https://preactjs.com/guide/v10/debugging) first
- ❌️ component testing is using `@testing-library/react` ; preact is not supported
  - it's not easy to switch from [@testing-library/react](https://github.com/testing-library/react-testing-library) to [@testing-library/preact](https://github.com/testing-library/preact-testing-library) or [jest-preset-preact](https://github.com/preactjs/jest-preset-preact) with little effort because you need to change the config and/or the apis
  - if you want to test with preact, write with your own choice
  - `jest-preset-preact` env is ready for `npm run test:preact` to help you start quickly
