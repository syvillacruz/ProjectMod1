# Simple Token

This Solidity program is a simple program that utilizes the require(), assert() and revert() statements.

## Description

This program is a simple contract written in Solidity, a programming language used for developing smart contracts on the Ethereum blockchain. The contract has a single function that returns the string "Hello World!". This program serves as a simple and straightforward introduction to Solidity programming, and can be used as a stepping stone for more complex projects in the future.

## Getting Started

The SimpleToken contract is a basic implementation of a token on the Ethereum blockchain using Solidity. Here are its key components:

### State Variables:

#### balances: A mapping that tracks the balance of tokens for each address.

#### totalSupply: Represents the total supply of tokens in the contract.

#### Constructor: Initializes the contract with an initial supply of tokens (_initialSupply) and assigns the entire supply to the address deploying the contract (msg.sender).

#### Functions: 

transfer(address _to, uint256 _value): Allows msg.sender to transfer tokens to another address _to. It checks if the sender has sufficient balance before transferring tokens.
burn(uint256 _value): Allows msg.sender to burn (destroy) tokens from their own balance. It checks if the sender has sufficient balance and includes a custom revert condition if tokens burned exceed the total supply.

#### Modifiers and Requirements:

The transfer and burn functions use the require statement to enforce conditions such as sufficient balance. The assert statement ensures that operations maintain the integrity of the total supply.
    
SPDX-License-Identifier: Indicates the open-source license under which the contract is released.

### Executing program

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension. Copy and paste the following code into the file:

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.0" (or another compatible version), and then click on the "Compile SimpleToken.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "SimpleToken" contract from the dropdown menu, and then click on the "Deploy" button.

Once the contract is deployed, you can interact with it by calling the different functions. Click on the "SimpleToken" contract in the left-hand sidebar, and then click on the one of the functions. Finally, click on the "transact"/"call" button to execute the function and retrieve the "Hello World!" message.

## Authors

syvillacruz
