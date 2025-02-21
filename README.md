# todo-react-vite
Sample todo app built with the React and Vite. For the accompanying documentation, see MDN article
[Understanding client-side JavaScript frameworks : React tutorials](https://wiki.developer.mozilla.org/en-US/docs/Learn/Tools_and_testing/Client-side_JavaScript_frameworks#React_tutorials).

[![Nightwatch Tests](https://github.com/nightwatchjs-community/todo-react/actions/workflows/node.js.yml/badge.svg?branch=main)](https://github.com/nightwatchjs-community/todo-react/actions/workflows/node.js.yml)
[![Netlify Status](https://api.netlify.com/api/v1/badges/fc4d39f7-69c2-421d-b95b-ac1873dfed9e/deploy-status)](https://app.netlify.com/sites/todo-react-vite/deploys)

## Project setup
```
npm install
```

### Run locally
```
npm run dev
```

### Compiles and minifies for production
```
npm run build
```

### Customize configuration
See [Configuration Reference](https://vitejs.dev/config/).

## Preview
You can see this project deployed live at: https://todo-react-vite.netlify.app

## Run tests
Tests are written using [Nightwatch 2](https://nightwatchjs.org/) and cover both component testing and end-to-end testing.

For component testing, the new [vite-plugin-nightwatch](https://www.npmjs.com/package/vite-plugin-nightwatch) plugin is used.

Before running the tests, make sure the `Vite` dev server is running and that the localhost url matches that which is set in the `.env` file. By default it is set to `http://localhost:3000`.

### Start the Vite dev server:

```
npm run dev
```

### Run component tests
This will run a sample component test for the `src/components/Form.jsx` component in Chrome:

```
npm test
```

To run it in headless mode:
```
npm test -- --headless
```

### Run end-to-end tests
This will run the end-to-end tests in Chrome:

```
npm run test-e2e
```

To run it in headless mode:
```
npm run test-e2e -- --headless
```
