# Project_2: Create a Token
This Solidity contract represents a basic token implementation. It allows for the minting and burning of tokens and tracks balances.

# Requirements
The contract includes public variables for token details, such as the token name, abbreviation, and total supply. It maintains a mapping of addresses to token balances. It also features functions to mint and burn tokens with necessary validations.

# Usage
# Public Variables
The following public variables are available:

tokenName: A string representing the name of the token.
tokenAbbrv: A string representing the abbreviation or symbol of the token.
totalSupply: An unsigned integer representing the total supply of the token.

# Mint Function
The mint function allows for the creation of new tokens. It takes two parameters:

_address: The address whose token balance will be increased.
_value: The amount of tokens to be minted.
The function increases the total supply by the specified value and adds the same amount to the balance of the specified address.

# Burn Function
The burn function allows for the destruction of tokens. It works in the opposite way to the mint function. It takes two parameters:

_address: The address whose token balance will be decreased.
_value: The amount of tokens to be burned.
The function checks if the balance of the specified address is greater than or equal to the amount to be burned. If it is, the total supply is decreased by the specified value, and the balance of the specified address is decreased by the same amount.

# License
This code is licensed under the MIT License. SPDX-License-Identifier: MIT
