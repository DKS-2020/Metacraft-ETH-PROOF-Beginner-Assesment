# Nexus Token Smart Contract

## Overview :
A smart contract implemented in Solidity for a custom token named "Nexus" (NXS) that supports minting and burning of tokens.

## Description :
This is a Solidity smart contract in which we can mint and burn tokens. I have created my own token, known as Nexus, with the abbreviation NXS. This code allows minting any amount of tokens as per requirements and also burning tokens according to needs.It also make sure that the balance of account is greater than or equal to the amount that is supposed to be burned. It's a very basic code that can easily give you an understanding of how to mint and burn tokens in Solidity.

### Mapping Vaiable:
"balances" which Maps addresses to their respective balances.

### Mint function:
It allows new tokens to created and assigned to specific address. In this code it takes two parameters:
1. "address" : new token will assigned to this address.
2. "value"   : number of token to be created.
#### Burn function :
It allow token to destroyed from specific address. In this code it takes two parameters:
1. "address" : nthe address from which the token will be removed.
2. "value"   : number of token to be destroyed.

## Author:
https://github.com/DKS-2020

## License:
This project is licensed under the MIT License - see the LICENSE.md file for details

## Smart Contract Code:
```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^ 0.8.18;

contract MyToken {

    // public variables here
    string public tokenName = "Nexus";
    string public tokenAbbrev = "NXS";
    uint public totalSupply = 0;

    // mapping variable here
    mapping(address => uint) public balances;

    // mint function
    function mint (address _address, uint _value) public{
      totalSupply += _value;
      balances[_address] += _value;
    }

    // burn function
    function burn (address _address, uint _value) public{
      if(balances[_address] >= _value){
      totalSupply -= _value;
      balances[_address] -= _value;
      }
    }

}

