swisstronik-erc-20
This repository contains a setup for deploying and interacting with an ERC-20 token on the Swisstronik testnet using Hardhat. The setup includes scripts for deploying the contract, minting tokens, and transferring tokens, utilizing encrypted transactions with Swisstronik.

Prerequisites
Ensure you have the following installed:

Node.js (version 14.x or later)
npm (version 6.x or later)
Installation
Clone the repository:

git clone https://github.com/dante4rt/t2swisstronik-erc-20.git
cd t2swisstronik-erc-20
Make the erc20.sh script executable:

chmod +x erc20.sh
Usage
Run the script:

./erc20.sh
Follow the prompts to enter your private key and specify the token name and symbol.

Scripts
deploy.js
This script deploys the ERC-20 contract and saves the deployed contract address to contract.txt.

mint.js
This script mints 100 tokens using the deployed contract. It reads the contract address from contract.txt.

transfer.js
This script transfers tokens from the contract to a specified address. It reads the contract address from contract.txt.


This project demonstrates a basic Hardhat use case. It comes with a sample contract, a test for that contract, and a Hardhat Ignition module that deploys that contract.

Try running some of the following tasks:

```shell
npx hardhat help
npx hardhat test
REPORT_GAS=true npx hardhat test
npx hardhat node
npx hardhat ignition deploy ./ignition/modules/Lock.js
```
