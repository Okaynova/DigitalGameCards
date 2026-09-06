# DigCards: NFT Marketplace dApp

## Project Overview & Features
DigCards is a decentralized marketplace for minting, listing, and trading digital game cards as Non-Fungible Tokens (NFTs). 
* **Minting:** Users can mint new NFT cards directly to their wallets.
* **Escrow Listing:** Owners can list their cards for sale, which securely locks the NFT in the smart contract.
* **Atomic Purchases:** Buyers can purchase listed cards using ETH, triggering an automatic and secure swap of funds to the seller and the NFT to the buyer.

## Tech Stack
* **Smart Contract:** Solidity (^0.8.20)
* **Libraries:** OpenZeppelin (ERC721URIStorage, ReentrancyGuard)
* **Development Environment:** Remix IDE
* **Storage:** IPFS (InterPlanetary File System) via Pinata

## Setup Instructions
1. Open Remix IDE and create a new file named `DigCards.sol`.
2. Copy the smart contract code into the file.
3. Navigate to the **Solidity Compiler** tab and compile using version `0.8.20`.
4. Go to the **Deploy & Run Transactions** tab.
5. Select **Injected Provider - MetaMask** as the environment to connect to your wallet.
6. Click **Deploy** and confirm the transaction in MetaMask.

## Testnet & Contract Address
* **Network:** Sepolia Testnet
* **Contract Address:** `[0x7b96aF9bD211cBf6BA5b0dd53aa61Dc5806b6ACe]`

## IPFS Implementation
This project utilizes IPFS to ensure decentralized storage of the NFT metadata. When a user mints a card via the `mintCard` function, they provide an IPFS URI (e.g., `ipfs://Qm.../metadata.json`). This URI points to a JSON file hosted on the IPFS network containing the card's name, description, and image hash. The smart contract permanently binds this IPFS URI to the specific Token ID on the blockchain using the `_setTokenURI` function.

## Deployed Link
link:-
https://sepolia.etherscan.io/address/0x7b96aF9bD211cBf6BA5b0dd53aa61Dc5806b6ACe

---
**Author:** Advait Kumar
