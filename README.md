# EthProof_Assessment:
---

# MyToken Smart Contract

This smart contract implements a basic ERC-20 token with minting and burning functionality. The contract is written in Solidity for the Ethereum blockchain.

## Contract Details

### Public Variables

- `tokenName` (string): The name of the token. 
- `abbr` (string): The abbreviation for the token.
- `totalSupply` (uint): The total supply of the token.

### Mapping

- `balances` (mapping): A mapping of addresses to their token balances.

## Functions

### mint

```solidity
function mint(address _address, uint _value) public
```

- **Parameters:**
  - `_address` (address): The address to which the tokens will be minted.
  - `_value` (uint): The number of tokens to mint.

- **Description:** Increases the `totalSupply` by `_value` and adds the same amount to the balance of `_address`.

### burn

```solidity
function burn(address _address, uint _value) public
```

- **Parameters:**
  - `_address` (address): The address from which the tokens will be burned.
  - `_value` (uint): The number of tokens to burn.

- **Description:** Decreases the `totalSupply` by `_value` and subtracts the same amount from the balance of `_address`. Ensures that the balance of `_address` is greater than or equal to `_value` before burning.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

This README provides an overview of the MyToken smart contract, including its public variables, mappings, and functions. The contract includes basic minting and burning functionalities necessary for managing a simple token on the Ethereum blockchain.
