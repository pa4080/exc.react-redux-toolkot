# Redux Toolkit with React: A Simple Exercise

The [ReduxToolkit](https://redux-toolkit.js.org/) part is based on the tutorial ["Redux - Complete Tutorial (with Redux Toolkit)" by
Cosden Solutions](https://youtu.be/5yEG6GhoJBs?si=fDYoCL9DQeE7cIIP).

Base concepts of Redux:

- Store: The state of the application
- Actions: What the store can do
- Reducers: How the state changes

Key points:

- Redux never mutate the state directly. Instead, it returns a new state based on the previous state and an action. Similar to React's setState - we need to return a new object with different memory address.
- ReduxToolkit automatically implements the same pattern under the hood.

See also:

- [Redux DevTools Chrome Extension](https://chromewebstore.google.com/detail/lmhkpmbekcpmknklioeibfkpmmfibljd?hl=en)
- [Why I Moved **from React Redux to Zustand** and Why You Should Too! by CoderOne](https://www.youtube.com/watch?v=DK-S4ZcmDcE)

## React + TypeScript + Vite + Redux Toolkit

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

In addition in this boilerplate is added support for SASS and the current latest version of TypeScript - 5.5.2.

### Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default {
  // other rules...
  parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
  },
}
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list
