# Product Factory Contract

This folder contains examples on how to compile/deploy/use custom transaction protocols to forge powered blockchain.

## Getting started

- Write a protocol in protocols sub folder
- Export `FORGE_MODERATOR_SK` variable, that is used to deploy protocol to ABT Node
- Run `forge protocol:compile ./protocol` to compile the protocol
- Run `forge protocol:deploy .compiled/create_product/elixir/create_product/create_product.itx.json` to deploy the protocol
- Run `node demo.js` to test with the example
