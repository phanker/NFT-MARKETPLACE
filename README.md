# NFT-MARKETPLACE

Nft Marketplace is a market place for selling nfts.It contains 3 parts.
The first is for selling nfts,you can list your nfts and sell them.
The second is for cancelling,you can cancel your listed items.
The third is for buying,you can buy the nfts anothers listed.


## Features
* Frontend server build by Next.js, Backend server build by Java  ,Contracts build by Solidity.
* Log in Nft marketplace with digital wallet using Walletconnect.
* All transactions are managed and send by Wagmi.
* Used Stream hooks of Moralis to listen to the events of transaction and callback the Backend server.
* Fecth the metadatas of nft using NFT'S API from Moralis.
* Integracted with the Mongodb to store events data that from Stream hooks of Moralis.
* Test and deploy contracts with Hardhat.

## Quick Start

# Step1:Start Backend server
  We need to run the Backend server at first.We need fill the apikey of Moralis in the application.properties(https://github.com/phanker/NFT-MARKETPLACE/blob/main/nft-market-backend/src/main/resources/application.properties) of Backend server instead example value of MORALIS_API_KEY.Please access to Moralis(https://admin.moralis.io/) then regirster if you don't have the apikey.after that.Like this we can run with the Backend server.

# Step2:Complie the contracts for Apis of contract
  For Apis of contract,We can use Remix to complie the contracts.

# Step3:Create the Stream hook
  To process this step we should login in the Moralis. creating the Stream hook is for listening to events of contract.(Of course you can create the Stream hook via coding,but here we directly create on the website).click the Stream tab then create new Stream,this the creation page you need fill the address and abi of NftMarketplace 
and choose the all events needing to listen to.You can refer the video below.

# Step4:Run with the frontend server


