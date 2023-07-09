# metaCrafters-ETH Beginner
# MyToken Contract

This is a Solidity smart contract that implements a basic token called MyToken. 
The contract allows for the minting and burning of tokens. 

## License

This code is licensed under the MIT License.

## Prerequisites

- Solidity version 0.8.18 or higher is required.

### Variables

- `tokenName`: A public string variable representing the name of the token. In this contract, it is set to "ALPHA".
- `tokenAbbrv`: A public string variable representing the abbreviation of the token. In this contract, it is set to "ALH".
- `totalSupply`: A public unsigned integer variable representing the total supply of tokens. Initially, it is set to 0.

### Mapping

- `balances`: A mapping that associates addresses with their respective token balances. The mapping is public, allowing external parties to view token balances for specific addresses.

### Functions

- `mint(address _address, uint _value)`: A public function used to mint new tokens. It takes an address `_address` and a uint `_value` as parameters.
                                         The function increases the total supply by `_value` and adds the same amount to the token balance of the specified `_address`.
  
- `burn(address _address, uint _value)`: A public function used to burn existing tokens. It takes an address `_address` and a uint `_value` as parameters.
                                         The function decreases the total supply by `_value` and reduces the token balance of the specified `_address` by the same amount, if the balance is sufficient.

## Usage

To use this contract, you need to deploy it on a compatible Ethereum Virtual Machine (EVM) blockchain network, such as Ethereum. Once deployed, you can interact with the contract using the provided functions.

1. Minting Tokens:
   - Call the `mint` function and provide the address to which the tokens should be minted (`_address`) and the amount of tokens to mint (`_value`).
   - This will increase the total supply and add the minted tokens to the balance of the specified address.

2. Burning Tokens:
   - Call the `burn` function and provide the address from which the tokens should be burned (`_address`) and the amount of tokens to burn (`_value`).
   - This will decrease the total supply and subtract the burned tokens from the balance of the specified address if the balance is sufficient.

## License
   This project is licensed under the MIT License - see the LICENSE.md file for details
