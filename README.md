# ETHproofproject.sol

Project title: Create a Token On this project we are going to use solidity which is a programming language designed for coding contracts on a blockchain. The purpose of this project is to test students how much they know and how does the transactions work on the blockchain.

Description The project will have a token name and amount of value that can be minted or burned and also have a condition where the burn function cannot exceed the amount remaining on the account of the token.

Getting Started: How/where to download your program// Any modifications needed to be made to files/folders//

Executing program To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., myToken.sol). Copy and paste the following code into the file: /////

pragma solidity 0.8.18;

contract MyToken {

string public tokenName = "Francheez";
string public tokenAbbrv = "FRNCHZ";
uint public totalSupply = 0;
mapping(address => uint) public balances;

function mint (address _address, uint _value) public { totalSupply += _value; balances [_address] += _value; }

function burn (address _address, uint _value) public { if(balances[_address] >= _value) { totalSupply -= _value; balances [_address] -= _value;

  }
}   
}

/////// to test if the code is working, click the icon under the "search in files", check the "auto compile checkbox.

under the "advance configurations" click the "compile [NAME OF THE FILE].sol and "compile and run.

after that, click the "deploy and run transactions where we can see an account

click the "copy" icon on the account and then click "deploy"

we can test the functionality of the code under the dropdown of the "deployed contracts"

paste the copied account on the "_address" textbox, in the mint where we can put an amount we want then just click "transact"

when you click "totalSupply" we should see the ammount that we entered in the "_value"

on the burn section, the _value that you will put in here will be deducted

we can check the balance of our account when we paste the copied account on the address text box

we can also check the token name by clicking tokenName

we should also see the balance of account is greater than or equal to the amount that is supposed to be burned.

Authors

Metacrafters Franciz

61801244@ntc.edu.ph

Metacrafter Chris

@metacraftersio

License This project is licensed under the MIT License - see the LICENSE.md file for details
