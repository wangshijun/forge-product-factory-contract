# Product Factory Contract

> Contract that defines the type need when your want to create a vending machine on your chain.

## What the use case of this blocklet?

You want to create an `AssetFactory` in your dApp, so that users can send `AcquireAssetTx` later, you should look at this contract.

## What are the requirements to use this blocklet?

- Install latest `@arcblock/forge-cli`
- Your machine should be able to run `elixir escript`

## How to use this blocklet?

- Write a protocol in protocols sub folder
- Export `FORGE_MODERATOR_SK` variable, that is used to deploy protocol to ABT Node
- Run `forge protocol:compile ./protocol` to compile the protocol
- Run `forge protocol:deploy .compiled/create_product/elixir/create_product/create_product.itx.json` to deploy the protocol
- Run `node demo.js` to test with the example
