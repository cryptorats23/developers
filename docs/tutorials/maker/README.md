# Market Maker

## Overview

Now that we've learned about Makers and Takers and how they interact with one another using dApps and APIs you may be interested in putting together these concepts in order to provide liquidity on the AirSwap marketplace. Over the course of this tutorial, you'll learn how to:

* Authenticate with the AirSwap Websocket
* Create Intents
* Receive getOrder requests
* Craft, sign and send orders

## Requirements

* NodeJS 10.15 or higher.
* Yarn (`npm install yarn`).
* An Ethereum key pair. You can use Metamask to create a new wallet and export the private key.
* Rinkeby Ethereum. Get some instantly using the [Rinkeby faucet](https://faucet.rinkeby.io/).
* At least 250 Rinkeby AST to use on the Rinkeby network. You can buy some using Rinkeby Ethereum here: [AirSwap Sandbox](https://sandbox.airswap.io).

## Getting Started

First, we'll want to install AirSwap.js

`yarn add airswap.js`

Next, open a JavaScript file for our maker and import ethers.js and AirSwap.js

```
const ethers = require('ethers')
const airswap = require('airswap.js')
```

We'll use ethers.js to import a private key using the wallet API.

`const wallet = new ethers.myWallet(pk)`

Next, we'll instantiate a simple message signer that signs any data.

`const messageSigner = data => wallet.signMessage(data)`

## Authenticate with the Router

We'll instantiate params and connect to the Router.

```const routerParams = { messageSigner: messageSigner, address: address, keyspace: false }

const router = new Router(routerParams)
```

Next create a main() function that connects to the router.

`await router.connect()`

## 