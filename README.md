## POLY_PROOF_MODULE_1_PROJECT

For this project, you will deploy an NFT collection on the Ethereum blockchain, Map the collection to Polygon, and Transfer assets over via the Polygon Bridge.
. Approve the NFTs to be transferred.
. Deposit the NFTs to the Bridge.
. Test balanceOf on Mumbai.
Deploy an ERC721 to the Goerli Ethereum Testnet.

## Getting Started

### Executing program

Download the codes by downloading the entire repository which will give you access to other contents of the repository. 

```shell

 npm install

```

After installing the dependencies, run the test file by using the following command:

```shell
npx hardhat test
```

### Deploying the ERC721 Contract

Before deploying, make sure t0 provide your wallet private key where required i.e. "PRIVATE_KEY= 'your wallet private key'". Run the following command to deploy the ERC721 contract to the Goerli Ethereum Testnet:

``` shell
npx hardhat run scripts/deploy.js --network goerli 
```
## NOTE:
After deploying the address will generate. So, copy that address into `contarctAddress.js`(stored in metadata folder) and also in `batchMint.js`(stored in scripts folder)

 
### Batch Mint NFTs

Run the following command to batch-mint NFTs using the deployed ERC721 contract:

``` shell
npx hardhat run scripts/batchMint.js --network goerli
```

### Approve and Deposit NFTs to Polygon Mumbai

Run the following commands to approve and deposit the minted NFTs from Ethereum to the Polygon Mumbai network using the FxPortal Bridge:

```shell
npx hardhat run scripts/approvedDeposit.js --network goerli
```



## Author
ABHISEK BAG
https://www.linkedin.com/in/abhisek-bag-09865421b/
21BCS9333@cuchd.in



## License

This project is licensed under the [MIT License](LICENSE).
You can make a copy of the project to use for your own purposes.
The MIT License is one of the most popular open-source licenses used for software, and it is often applied to Solidity smart contracts as well. The MIT License is a permissive license that allows users to freely use, modify, distribute, and sublicense the code, as long as they include the original copyright notice and disclaimer
