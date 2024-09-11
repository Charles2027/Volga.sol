# Volga.sol
A simple ERC20 Token contract 

## Getting Started
- Go to Remix ide ([Remix ide](https://remix.ethereum.org/))
- create a new file naming DogToken.sol
- paste the contract from the repo  ,compile and deploy
- you can use hardhat or other chains to deploy and test 
- go to the deployed contracts tab and test functionality .

## Contract Overview

- **Token Name:** Volga
- **Token Symbol:** VLGA

## Features

1. **Minting:** Only the owner can mint new tokens.
2. **Burning:** Any token holder can burn their own tokens.
3. **Transfer** Transfer tokens 

## Contract Components

### Imports

- **ERC20:** Provides standard ERC20 token functionality.
- **Ownable:** Ensures that only the owner can perform certain actions.

### Variables

- `address public owner;` - The address of the contract owner.

### Constructor

- `constructor(string memory name, string memory symbol)` - Initializes the contract, setting the token name and symbol, and assigns the owner to deployer address.

### Modifiers

- `onlyOwner` - Restricts function access to the owner.

### Functions

- `function mint(address to, uint256 amount) public onlyOwner` - Mints new tokens to a specified address. Only callable by the owner.
- `function burn(uint256 amount) public` - Burns a specified amount of tokens from the caller's balance.
- `function customTransferr(address recipient, uint256 amount) public returns (bool)` - transfer token to address from your account if you have enough balance you want to send .

# Author
- Charles Finni

# license
- This is free and unencumbered software released into the public domain.



