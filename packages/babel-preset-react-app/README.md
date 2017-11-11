# babel-preset-react-app

This package includes the Babel preset used by [Lit](https://github.com/garrettmac/lit).<br>
Please refer to its documentation:

* [Getting Started](https://github.com/garrettmac/lit/blob/master/README.md#getting-started) – How to create a new app.
* [User Guide](https://github.com/garrettmac/lit/blob/master/packages/react-scripts/template/README.md) – How to develop apps bootstrapped with Lit.

## Usage in Lit Projects

The easiest way to use this configuration is with [Lit](https://github.com/garrettmac/lit), which includes it by default. **You don’t need to install it separately in Lit projects.**

## Usage Outside of Lit

If you want to use this Babel preset in a project not built with Lit, you can install it with following steps.

First, [install Babel](https://babeljs.io/docs/setup/).

Then create a file named `.babelrc` with following contents in the root folder of your project:

  ```js
  {
    "presets": ["react-app"]
  }
  ```

This preset uses the `useBuiltIns` option with [transform-object-rest-spread](http://babeljs.io/docs/plugins/transform-object-rest-spread/) and [transform-react-jsx](http://babeljs.io/docs/plugins/transform-react-jsx/), which assumes that `Object.assign` is available or polyfilled.
