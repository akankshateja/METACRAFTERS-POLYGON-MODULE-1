# METACRAFTERS-POLYGON-MODULE-1

This is my NFT Project, in which I was tasked to deploy an NFT collection on the Ethereum blockchain, Map the collection to Polygon, and Transfer assets over via the Polygon Bridge.

## Installation
To get started with the project, follow these steps:

1. clone this repository :
    `git clone https://github.com/Palakkkkkkkkkk/METACRAFTERS-POLYGON-MODULE-1.git`
   
2. Install the required dependencies :
     `npm install`

## ERC721 Contract Deployment
Before deploying, add private key to your wallet here in "PRIVATE_KEY= 'your wallet private key'". 
Run the following command to deploy the ERC721 contract to the Goerli Ethereum Testnet:

`npx hardhat run scripts/deploy.js --network goerli`


After deploying the contract, the address will be generated. So, copy that address and paste it into the batchMint.js, and approveDeposit.js file(stored in scripts folder), and contractAddress.js file(stored in metadata folder).

## Minting the NFTs
Run the following command to batch-mint NFTs using the deployed ERC721 contract:

`npx hardhat run scripts/batchMint.js --network goerli`

## Approve and Deposit NFTs to Polygon Mumbai
Run the following commands to approve and deposit the minted NFTs from Ethereum to the Polygon Mumbai network using the FxPortal Bridge:

`npx hardhat run scripts/approveDeposit.js --network goerli`

## Author
PALAK JAIN :)

## LICENSE
This project is licensed under the [MIT License](LICENSE).
