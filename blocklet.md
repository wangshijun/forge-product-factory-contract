# Product Factory Contract

> Contract that defines the type need when your want to create a vending machine on your chain.

## Why this blocklet?

This blocklet is a minimalistic implementation of a smart contract that can be compiled and deploy to forge powered blockchain. It just contains one new `Transaction` type and message types required to compose that transaction.

## Use case of this blocklet?

If you are new to forge smart contracts, you can use this blocklet as a starting point to learn and explore it's workflow and composing guidelines.

If you want to create an `AssetFactory`, so that users can send `AcquireAssetTx` later in your dApp, you should look at this contract.

## Requirements to use this blocklet?

Software requirements are:

- Node.js runtime v10+ installed
- Latest forge cli installed with: `npm install -g @arcblock/forge-cli`
- Install `erlang` and `elixir >= 1.9.0`, and can run `elixir escript`

Knowledge requirements are:

- Basic ideas and formats around [google protocol buffers](https://developers.google.com/protocol-buffers/)
- Basic syntax and format of [yaml](https://yaml.org)
- Basic command line usage experience

## How to use this blocklet?

- Run: `forge blocklet:use forge-product-factory-contract` to get the contract files
- Run: `forge protocol:compile ./protocol` to compile the contract
- Run: `forge protocol:deploy .compiled/create_product/elixir/create_product/create_product.itx.json` to deploy the contract
- Run: `node demo.js` to test with the example
