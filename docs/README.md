![AirSwap Developer Tools](./assets/logo/AirSwap-Developer-Tools-Logo.png)

## What is AirSwap? {docsify-ignore-all}

[AirSwap](https://airswap.io/) is a peer-to-peer network for trading Ethereum ERC20 tokens. Peers connect to the marketplace and use the [Swap](https://swap.tech/whitepaper/) protocol to find and execute trades:

* Makers: provide liquidity in the form of quotes and signed orders
* Takers: send requests for quotes / orders and execute swaps

In general, Takers tend to use existing [dApps](dapps/widget.md) for price discovery and execution, while Makers tend to use our APIs and libraries to provide liquidity.

## Maker Quickstart

To become a maker on AirSwap, check out the [Market Maker tutorial](tutorials/market-maker/README.md), or simply follow the steps below:

1. Create a new Ethereum wallet
2. Acquire Rinkeby ETH from the [Faucet](https://faucet.rinkeby.io/)
3. Acquire Rinkeby AST from the [Sandbox](https://sandbox.airswap.io/)
4. `git clone git@github.com:airswap/developers.git`
5. `cd developers/docs/tutorials/market-maker`
5. `export PRIVATE_KEY=<your private key, prefixed with 0x>`
6. `export ENV=sandbox`
7. `yarn && yarn run start`

!> The following APIs are in use in production on the AirSwap network. We are sharing these APIs and code samples publicly with our community to build and iterate on them. By connecting to and using the AirSwap services you accept the [AirSwap Terms of Use](https://swap.tech/airswap-terms-of-use.pdf). Please also be sure to review the [LICENSE](LICENSE.md).

## Join the Conversation

Be sure to join the AirSwap Developers Telegram group at https://t.me/airswapdevs or the AirSwap Community at https://t.me/airswap.
