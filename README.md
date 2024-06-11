# Project Title

**Create a Token**
# Description
This project is all about creating a token on Ethereum blockchain using solidity.It includes concept of creating, minting and burning of tokens
# Requirements
1.Declare public string and unsigned variables.  
2.Require a mapping of addresses to balances.  
3.A mint function is required for increasing the total supply and balance of address by a specified amount.    
4.A burn function is also required for burning existing tokens and decresing the totalsupply and balance amount.
# Installation
No official installation is requred.  
There is online compilier for this project.  
Visit: [Remix IDE](https://remix.ethereum.org/#lang=en&optimize=false&runs=200&evmVersion=null&version=soljson-v0.8.18+commit.87f61d96.js)
# Acknowledgements
I would like to acknowledge the professors of whole Meta team which help me so that I completed my project successfully.
# EXECUTION
1.Open Remix IDE adn create a new file and copy paste the following code: 

    pragma solidity 0.8.18;
    
    contract MyToken {
    
    string public tokenname="keshav";
    string public tokenAbbrv="singla";
    uint public totalsupply=0;

    mapping (address=> uint) public balances;
    function mint(address _address, uint _value) public{
        totalsupply += _value;
        balances[_address] += _value;
    }
        function burn(address _address, uint _value) public{
            if(balances[_address] >= _value){
            totalsupply += _value;
            balances[_address] -= _value;
     }
        } }

2.Use Solidity compiler section and deploy and run transaction section for compiling and deploying.
# Authors
[@abcd150](https://github.com/abcd150)
# License 
This project is licensed under the MIT License - see the LICENSE.md file for details.


 

