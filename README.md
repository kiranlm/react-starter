# react-boilerplate

React 16.5.2 + babel 7 + jest + webpack 4 + flow + eslint + esdoc + live editing boilerplate.

[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)
[![coverage statements](./coverage/badge-statements.svg)](https://github.com/pamepeixinho/jest-coverage-badges)
[![coverage lines](./coverage/badge-lines.svg)](https://github.com/pamepeixinho/jest-coverage-badges)
[![coverage functions](./coverage/badge-functions.svg)](https://github.com/pamepeixinho/jest-coverage-badges)
[![dependencies](https://david-dm.org/Ziv-Barber/react-boilerplate.svg?style&#x3D;flat-square)](https://david-dm.org/Ziv-Barber/react-boilerplate)
[![devDependencies](https://david-dm.org/Ziv-Barber/react-boilerplate/dev-status.svg?style&#x3D;flat-square)](https://david-dm.org/Ziv-Barber/react-boilerplate#info&#x3D;devDependencies)
[![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg)](https://github.com/semantic-release/semantic-release)
[![build status](https://travis-ci.org/Ziv-Barber/react-boilerplate.svg?branch&#x3D;master)](https://travis-ci.org/Ziv-Barber/react-boilerplate)

![react-boilerplate logo](https://cdn-images-1.medium.com/max/1500/1*LQbS9RgHy93y9JH8ltejuQ.jpeg)

- [Getting Started](#getstart)
- [Features](#features)
- [Installation](#inst)
- [The source code](#code)
- [Variations](#other)
- [Credit](#credit)

<a name="getstart"></a>
## Getting Started: ##

This boilerplate including a basic code to start creating a web app using React.

Start with cloning the project:

```bash
$ git clone --depth=1 git://github.com/Ziv-Barber/react-boilerplate.git your-project-name
```

- Remove the .git directory (rm -rf your-project-name/.git).
- Edit package.json and change the name of the project to your project name.

Now, create a new github project and do:
	
```bash
$ git init
$ git remote add origin https://github.com/your-name/your-project-name.git
$ git add -A
$ npm run commit
$ git push origin master
```

This project is using [semantic-release](https://github.com/semantic-release/semantic-release) to automatic handling of the version of your web app. To be able to automatic release a new version you must configure Travis-CI to your new project:

- Go to [https://travis-ci.org/](https://travis-ci.org/) and either signup or signin.
- Select your new project and click setting.
- You MUST configure a token or [semantic-release](https://github.com/semantic-release/semantic-release) will not be able to commit changes:
  - Create a new token (see [here](https://help.github.com/articles/creating-a-personal-access-token-for-the-command-line/) how to do it).
  - Permissions needed in the github token:
    - repo:
      - repo:status
      - repo_deployment
      - public_repo
    - admin:org:
      - read:org
    - admin:repo_hook:
      - write:repo_hook
    - user:
      - user:email
  - In your Travis-CI project setting, go to the environment settings section and add a new environment variable with the name 'GH_TOKEN' and the generated token as the data.
- To test everything just push something into github and it should update everything automatic!

<a name="features"></a>
## Features: ##

This project is using the following awesome libraries/utilities/services:

- [jest](https://jestjs.io/)
- [babel 7](https://babeljs.io/)
- [commitizen](http://commitizen.github.io/cz-cli)
- [esdoc](https://esdoc.org/)
- [ESLint](https://eslint.org/)
- [flow](https://flow.org/)
- [better-npm-run](https://github.com/benoror/better-npm-run)
- [npm-run-all](https://github.com/mysticatea/npm-run-all)
- [react](https://reactjs.org/)
- [redux](https://redux.js.org/)
- [semantic-release](https://github.com/semantic-release/semantic-release)
- [redux-thunk](https://github.com/reduxjs/redux-thunk)
- [webpack](https://webpack.js.org/)

<a name="inst"></a>
## Installation: ##

via Git:

```bash
$ git clone git://github.com/{{authorGit}}/{{name}}.git
```

<a name="code"></a>
## :coffee: The source code: ##

### The project structure: ###

- react-boilerplate/src/ - All the sources should be here.
- react-boilerplate/src/types/ - All the flow type declarations.
- react-boilerplate/src/components/containers/ - All the React containers.
- react-boilerplate/src/components/presentational/ - All the React presentational components without a state.
- react-boilerplate/src/store/ - The redux store.
- react-boilerplate/__tests__/ - All the unit tests.
- webpack.config.js - The configuration for [webpack](https://webpack.js.org/).
- .editorconfig - The [coding style settings](editorconfig.org) for this project.

### Npm scripts: ###

When using with **yarn** then use the following syntax:

```bash
$ yarn name params
```

Or with just **npm**:

```bash
$ npm name params
```

- **start** - Run the code in development mode.
- **build** - Build the production mode.
- **lint** - Lint :cop: using [ESLint](https://eslint.org/).
- **flow** - [Flow](https://flow.org/) checks.

<a name="other"></a>
## Variations: ##

- [library-boilerplate](https://github.com/Ziv-Barber/library-boilerplate) - Rollup based javascript library boilerplate + babel 7, eslint, flow, jest, esdoc and live editing.
- [library-boilerplate-mocha](https://github.com/Ziv-Barber/library-boilerplate-mocha) - Rollup based javascript library boilerplate + babel 7, eslint, flow, mocha, esdoc and live editing.
- react-boilerplate (this project) - React 16.5.2 + babel 7 + jest + webpack 4 + flow + eslint + esdoc + live editing boilerplate.
- [react-boilerplate-mocha](https://github.com/Ziv-Barber/react-boilerplate-mocha) - React 16.5.2 + babel 7 + mocha + webpack 4 + flow + eslint + esdoc + live editing boilerplate.

<a name="credits"></a>
## Credit: ##

- Created by Ziv Barber.
