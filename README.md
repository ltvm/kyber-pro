# Kyber FPR Node Implementation

This is a reference implementation for Kyber's FPR javascript SDK. By default, it connects to Ropsten testnet, but you can easily point it to mainnet when you are ready to deploy. 

We recommend reviewing the Kyber FPR tutorials to get a good understanding of the various functions involved.

1. Basics: Deployment, Adding Token Pairs and Setting Base Rates
2. Control  [WIP]
3. Optimization and Sanity [WIP]

## Getting Started

To get started, clone this repo into a local directory. After that, run `npm install` to install the SDK and related libraries.

```
npm install
```

Add your enviroment variables to a new .env file. 

```shell
# Sample .env
ROPSTEN_NODE_URL = https://ropsten.infura.io/v3/XXX
TESTNET_PRIVATE_KEY = 8C9CFCEE9048E0D6B481E58F6E874368682B5FD01DD6HF867E71...
```

Make sure you have ETH in your Ropsten testnet account. You can get Ropsten ETH [here](https://faucet.ropsten.be/).

After that, run the deployment script. This will set up the corresponding smart contracts 

```shell
node deploy.js
```

Replace the default reserve addresses in `addresses.json` with the addresses that show up in the deployment script.
