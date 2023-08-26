# Anime NFT Smart Contract

## Introduction

This repository contains a Solidity smart contract for creating Anime-themed NFTs. The contract is built on the ERC-721 standard and extends the functionality with enumeration and ownership features. It allows users to mint new NFTs, manage metadata, and customize contract settings.

## Smart Contract Details

- **Name:** Anime
- **Symbol:** ANK

### Functionalities

1. **Minting:** Users can mint new Anime NFTs in specified quantities.
2. **Metadata:** The contract supports base URI for metadata of NFTs.
3. **Owner Privileges:** The contract owner can set base URI, prompt, and token attributes.
4. **Total Supply:** Provides the total number of minted NFTs.
5. **Token Attributes:** Stores additional attributes for each NFT token.
6. **Withdraw:** Allows the owner to withdraw the contract balance.

## Deployment

1. Install dependencies:

   ```bash
   npm install
   ```

2. Configure your environment variables in a `.env` file:

   ```plaintext
   MNEMONIC=<your_mnemonic_phrase>
   INFURA_PROJECT_ID=<your_infura_project_id>
   ```

3. Deploy the contract:

   ```bash
   npx hardhat run scripts/deploy.js --network <network_name>
   ```

   Replace `<network_name>` with the desired network (e.g., `mumbai` or `sepolia`).

## Interacting with the Contract

- To mint NFTs, call the `mint` function, specifying the quantity to mint.

- Use the owner's account to set the base URI, prompt, and token attributes using appropriate functions.

- View token attributes using the `getTokenAttributes` function.

- Withdraw contract balance using the `withdraw` function.

## Hardhat Configuration

- Edit the `hardhat.config.js` file to include your networks, accounts, and Solidity version.

- Use the appropriate network name for deploying the contract.

## License

This project is licensed under the MIT License. 
