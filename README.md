# Sushi Auction Maker

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

The Auction Maker is a permission-less system that allows the fees (5 bp) earned by the sushiswap, to be sold for the bid token (Sushi / xSushi) which is served to the xSushi holders using the SushiBar. Anyone can start the auction for a particular token with a bid. There are two periods (minTTL and maxTTL) during which the bid can be finalized. Once, the bid is finalized, it is sent to the receiver to be served at SushiBar. The users cannot start an auction for the LP token, only underlying tokens are allowed.

## Env

```sh
cp .env.example .env
```

## Test

```sh
yarn test
```

```sh
yarn test test/Greeter.ts
```

## Coverage

```sh
yarn test:coverage
```

<https://hardhat.org/plugins/solidity-coverage.html#tasks>

## Gas

```sh
yarn test:gas
```

<https://github.com/cgewecke/hardhat-gas-reporter>

## Lint

```sh
yarn lint
```

## Watch

```sh
npx hardhat watch compile
```

## Deployment

### Local

Running the following command will start a local node and run the defined deploy script on the local node.

```sh
npx hardhat node
```

### Mainnet

```sh
yarn mainnet:deploy
```

```sh
yarn mainnet:verify
```

```sh
hardhat tenderly:verify --network mainnet ContractName=Address
```

```sh
hardhat tenderly:push --network mainnet ContractName=Address
```

### Ropsten

```sh
yarn ropsten:deploy
```

```sh
yarn ropsten:verify
```

```sh
hardhat tenderly:verify --network ropsten ContractName=Address
```
