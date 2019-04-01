[![banner](https://raw.githubusercontent.com/oceanprotocol/art/master/github/repo-banner%402x.png)](https://oceanprotocol.com)

<h1 align="center">commons-marketplace</h1>

> Marketplace front-end and backend server to explore, download, and publish open data sets.

[![Build Status](https://travis-ci.com/oceanprotocol/commons-marketplace.svg?token=3psqw6c8KMDqfdGQ2x6d&branch=master)](https://travis-ci.com/oceanprotocol/commons-marketplace)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-7b1173.svg?style=flat-square)](https://github.com/prettier/prettier)
[![js oceanprotocol](https://img.shields.io/badge/js-oceanprotocol-7b1173.svg)](https://github.com/oceanprotocol/eslint-config-oceanprotocol)
[![css bigchaindb](https://img.shields.io/badge/css-bigchaindb-39BA91.svg)](https://github.com/bigchaindb/stylelint-config-bigchaindb)

- [Prerequisites](#prerequisites)
- [Get Started](#get-started)
- [Production](#production)
- [Testing](#testing)
- [Code Style](#code-style)
- [License](#license)

<img alt="screen shot 2019-02-08 at 16 53 57" src="https://user-images.githubusercontent.com/90316/52489283-27080e80-2bc2-11e9-8ec0-508c21eb86f7.png">

## Prerequisites

To make use of all the functionality, you need to connect to the Ocean network.

For local development, you can spin up [`barge`](https://github.com/oceanprotocol/barge) to use a local network:

```bash
git clone git@github.com:oceanprotocol/barge.git
cd barge

./start_ocean.sh --latest --no-pleuston --local-spree-node
```

The default configuration of the client & server is to connect to this local network. Modify `./client/src/config.ts`, and `./server/src/config/config.ts` to change that.

## Get Started

To spin up both, the client and the server in a watch mode for local development, execute:

```bash
npm install
npm start
```

This will run both, client and server in development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view the client in the browser.

The page will reload if you make edits to files in either `./client` or `./server`.

## Production

To create a production build of both, the client and the server:

```bash
npm run build
```

Builds the client for production to the `./client/build` folder, and the server into the `./server/dist` folder.

## Testing

```bash
npm test
```

Launches the test runner in the interactive watch mode.<br>
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

## Code Style

For linting and auto-formatting you can use:

```bash
# auto format all ts & css with eslint & stylelint
npm run lint

# auto format all ts & css with prettier, taking all configs into account
npm run format
```

## License

```text
Copyright 2018 Ocean Protocol Foundation Ltd.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```