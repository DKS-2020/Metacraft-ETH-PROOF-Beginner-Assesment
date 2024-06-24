# Nexus Token Smart Contract

## Overview :
A smart contract implemented in Solidity for a custom token named "Nexus" (NXS) that supports minting and burning of tokens.

## Description :
This is a Solidity smart contract in which we can mint and burn tokens. I have created my own token, known as Nexus, with the abbreviation NXS. This code allows minting any amount of tokens as per requirements and also burning tokens according to needs.It also make sure that the balance of account is greater than or equal to the amount that is supposed to be burned. It's a very basic code that can easily give you an understanding of how to mint and burn tokens in Solidity.

### Mapping Vaiable:
"balances" which Maps addresses to their respective balances.

### Mint function:
It allows new tokens to created and assigned to specific address. In this code it takes two parameters:
a) "address" : new token will assigned to this address.
b) "value"   : number of token to be created.
#### Burn function :
It allow token to destroyed from specific address. In this code it takes two parameters:
a) "address" : nthe address from which the token will be removed.
b) "value"   : number of token to be destroyed.

## Author:
Deepak Kumar Singh(chandigarh University)
https://github.com/DKS-2020

## License:
This project is licensed under the MIT License - see the LICENSE.md file for details

