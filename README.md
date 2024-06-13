# contract123
simply code making a contract in solidity language , containing functions variables mapping etc.

# SimpleToken Smart Contract

## Overview

This Solidity smart contract, `SimpleToken`, represents a basic implementation of a token on the Ethereum blockchain. It provides functionalities to mint and burn tokens. The contract keeps track of token balances associated with addresses and the total supply of tokens.

## Contract Details

### Public Variables

- `a` (string): The name of the token. Default is "SimpleToken".
- `b` (string): The abbreviation of the token. Default is "STK".
- `c` (uint): The total supply of the token. Initially set to 0.

### Mapping

- `d` (mapping): Maps addresses to their respective token balances. The mapping is defined as `mapping(address => uint)`.

### Functions

#### `mint`

This function allows the creation (minting) of new tokens. It increases the total supply of tokens (`c`) and updates the balance of the specified address in the mapping (`d`).

**Parameters:**
- `addr` (address): The address to which the minted tokens will be assigned.
- `val` (uint): The number of tokens to mint.

**Usage:**
```solidity
function mint(address addr, uint val) public;
