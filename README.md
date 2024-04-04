
# Solidity Contracts README
This repository contains Solidity contracts for ERC20 token and a Vault.

# ERC20 Contract
Description
The ERC20 contract implements the ERC20 standard for a basic fungible token. It allows for functionalities such as transferring tokens, approving token transfers, and transferring tokens on behalf of another address.

# Features
Total Supply: Tracks the total supply of the token.
Balances: Maps addresses to their token balances.
Allowances: Maps owner addresses to spender addresses and their allowed token amounts.
Name, Symbol, and Decimals: Provides metadata for the token.
Transfer Function: Allows token holders to transfer tokens to other addresses.
Approve Function: Allows token holders to approve other addresses to spend tokens on their behalf.
Transfer From Function: Allows approved addresses to transfer tokens on behalf of token holders.
Mint Function: Allows minting new tokens.
Burn Function: Allows burning existing tokens.
Events
Transfer: Triggered when tokens are transferred from one address to another.
Approval: Triggered when approval is granted for one address to spend tokens on behalf of another address.
## Vault Contract
# Description
The Vault contract is designed to facilitate depositing and withdrawing ERC20 tokens in a controlled manner. It maintains a pool of tokens and issues shares to depositors, which can be redeemed for tokens upon withdrawal.
# Features
Token Interaction: Interacts with an ERC20 token contract to deposit and withdraw tokens.
Total Supply and Balances: Tracks the total supply of shares and the balance of shares for each address.
Deposit Function: Allows users to deposit ERC20 tokens into the Vault and receive shares representing their ownership.
Withdraw Function: Allows users to withdraw ERC20 tokens from the Vault by redeeming shares.
# Mathematics
The deposit and withdrawal functions use mathematical calculations to determine the number of shares to mint or burn based on the deposited or withdrawn token amount and the total supply of shares.
