# 🧙 Ethereum ERC 20 Wizard 🧙
<p align="left">
<img alt="npm version" src="https://img.shields.io/npm/v/erc20-wizard.svg">
<img alt="NPM" src="https://img.shields.io/npm/l/erc20-wizard.svg">
</p>
CLI for creating and deploying ERC20 tokens on Ethereum network.

## Install
```
$ npm install -g erc20-wizard
```

## Configuration
First go and get your infura project id at https://infura.io/.
```
$ erc20-wizard --config=yourInfuraProjectId
```

## Usage
Deploy to `main` net:
```
$ erc20-wizard --main
```

Deploy to `ropsten` testnet:
```
$ erc20-wizard --ropsten
```

Deploy to `rinkeby` testnet:
```
$ erc20-wizard --rinkeby
```

You will be asked to provide informations about ERC20 token:
1. Private key which will be used to sign the transaction. **Private key is not stored in the process**. Make sure you have some funds on your account since deploying a token costs ether.
2. Token information like name, symbol, decimal places and total supply

```
prompt: Please enter your private key. This will be used to sign contract transaction.:
prompt: Token name:  MyAwesomeToken
prompt: Token symbol:  MAT
prompt: Token decimal places:  18
prompt: Token total supply:  100000000
✅ MyAwesomeToken successfuly deployed from 0x0Dca93a693b9695B9fFf96E3c60d062B6F152250 to 0xD565eDF2319B6F6c0d1c32Dce532AAd1Bf2C0F99
```
