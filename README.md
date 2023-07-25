## POLY_PROOF_MODULE_1_PROJECT

For this project, you will deploy an NFT collection on the Ethereum blockchain, Map the collection to Polygon, and Transfer assets over via the Polygon Bridge.
# Approve the NFTs to be transferred.
# Deposit the NFTs to the Bridge.
# Test balanceOf on Mumbai.
Deploy an ERC721 to the Goerli Ethereum Testnet.

## Getting Started And Compile

### Executing program

Download the codes by downloading the entire repository 

```shell

 npm install

```

### Deployment the ERC721 Contract:

``` shell
npx hardhat run scripts/deploy.js --network goerli 
```
## Main Point:
After deploying the address will generate. So, copy that address into `contarctAddress.js` and also in `batchMint.js`

 
## Run the following command to batch-mint NFTs using the deployed ERC721 contract:

``` shell
npx hardhat run scripts/batchMint.js --network goerli
```

### Approved and Deposit NFTs to Polygon Mumbai

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
