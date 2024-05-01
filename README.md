# Solidity Vault with ERC20 Token

# Overview:
This repository contains a Solidity smart contract implementing a basic vault functionality for handling ERC20 tokens. The vault contract allows users to deposit ERC20 tokens into the contract, minting vault shares in return. These shares can then be used to withdraw the equivalent amount of ERC20 tokens. This setup ensures efficient and secure management of deposited assets.
# Contracts:
1. ERC20.sol: This contract defines a basic ERC20 token standard implementation. It includes functionalities for transferring tokens, approving token transfers, and managing allowances. Users can also mint new tokens and burn existing ones.
2. Vault.sol: The Vault contract facilitates the deposit and withdrawal of ERC20 tokens. Users can deposit tokens, which are converted into vault shares proportionally to the total supply. Likewise, users can withdraw tokens by burning vault shares and receiving the equivalent amount of tokens.

# Usage:

1. Deploying Contracts: Deploy the ERC20 contract and provide the necessary token details such as name, symbol, and decimals. Then deploy the Vault contract, passing the ERC20 token address as a constructor argument.
2. Depositing Tokens: Users can deposit ERC20 tokens into the vault contract using the deposit function. Specify the amount of tokens to deposit, and the equivalent vault shares will be minted.
3. Withdrawing Tokens: To withdraw tokens, users need to burn a specific amount of vault shares using the withdraw function. The corresponding ERC20 tokens will be transferred back to the user's account
