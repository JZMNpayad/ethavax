# ethavax

DegenToken is an ERC-20 token that includes functionalities for managing allowances, tracking inventory, and buying items from a virtual merchant.

## Table of Contents

- [Overview](#overview)
- [Functionalities](#functionalities)
- [Usage](#usage)

## Overview

DegenToken is an ERC-20 token built on the Ethereum blockchain. It extends the functionality of the OpenZeppelin ERC20 and Ownable contracts to include a virtual merchant where users can buy items using the token.

## Functionalities

### ERC-20 Token

DegenToken follows the ERC-20 standard, allowing for basic token functionalities such as transfers, allowances, and balance tracking.

### Ownable

The contract inherits from Ownable, ensuring that certain functions can only be executed by the owner of the contract.

### Virtual Merchant

The contract includes a virtual merchant with items that users can buy using the token. Each item has a name and a price, and users can purchase items from the merchant by burning the required amount of tokens.

## Usage

1. **Minting Tokens:** The owner can mint new tokens using the `mint` function.

2. **Burning Tokens:** Users can burn their own tokens using the `burn` function.

3. **Transferring Tokens:** Users can transfer tokens to other addresses using the standard ERC-20 `transfer` function.

4. **Buying from Merchant:** Users can buy items from the virtual merchant using the `buyFromMerchant` function. Each item has a unique index, and users need to have a sufficient balance to make a purchase.

5. **Checking Inventory:** Users can check the number of items available in the virtual merchant using the `InventoryItemCount` function.

