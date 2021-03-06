# Installing Dependencies for React with Webpack Projects

Now that we have an empty Webpack Configuration file (`webpack.config.js`) and a freshly made Package file (`package.json`), we need to install some dependencies. Installing dependencies automatically adds some data to our `package.json`.

This project will depend on React, ReactDOM, Webpack, and Webpack Dev Server. It will also depend on a number of Babel packages, because we are going to be writing code using ES6, and [Babel is an ES6 transpiler](https://babeljs.io/).

##

The dependencies we require in detail:

| Package | Reason |
| --- | --- |
| [React](https://www.npmjs.com/package/react) | 'An npm package to get you immediate access to React, without also requiring the JSX transformer.' |
| [React DOM](https://www.npmjs.com/package/react-dom) | 'This package serves as the entry point of the DOM-related rendering paths. It is intended to be paired with the isomorphic React, which will be shipped as react to npm.' |
| [Webpack](https://www.npmjs.com/package/webpack) | 'Allows to split your codebase into multiple bundles, which can be loaded on demand.' |
| [Webpack Dev Server](https://www.npmjs.com/package/webpack-dev-server) | 'Serves a webpack app. Updates the browser on changes.' |
| [Babel Loader](https://www.npmjs.com/package/babel-loader) | 'Babel module loader for Webpack.' |
| Babel Core | Required for Babel Loader. |
| Babel Preset: ES2015 | Required for Babel Loader. |
| Babel Preset: React | Required for Babel Loader. |

We can go ahead and install all these modules with a single command:

```
npm install --save-dev react react-dom webpack webpack-dev-server babel-loader babel-core babel-preset-es2015 babel-preset-react
```

If we look at our `package.json` file now, we will notice that our `devDependencies` has become a list of the Node packages we just installed. This is important because it means we can install these again if we need to using `npm install`.

- [Help: More about `dependencies` and `devDependencies`](http://stackoverflow.com/a/22004559/4637110)
