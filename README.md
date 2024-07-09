# ProjectMod1

## Description

The ProjectMod1 contract demonstrates the use of require(), assert(), and revert() statements to enforce certain conditions and ensure contract integrity.

## Functions

### setValue(uint256 _value): 
Sets the state variable value to the given _value.
This function allows users to set the value for the contract.

### checkValue(uint256 _value):
A pure function that takes an input _value and performs checks on it.
Uses require() to ensure the input value is between 10 and 20 (inclusive).

If the condition fails, it reverts the transaction with the message: "The inputted value must be between 10 and 20".

Uses revert() to explicitly fail if the input value is not exactly 10.
If _value is not 10, it reverts the transaction with the message: "The value must be exactly 10".

### asserting()
A view function that uses assert() to check an internal condition.
Ensures that the state variable value is greater than 5.

If the condition fails, it indicates a critical bug in the contract logic, and the transaction is reverted, consuming all gas.

## Executing program

To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension. Copy and paste the following code into the file:

To compile the code, click on the "Solidity Compiler" tab in the left-hand sidebar. Make sure the "Compiler" option is set to "0.8.0" (or another compatible version), and then click on the "Compile ProhectMod1.sol" button.

Once the code is compiled, you can deploy the contract by clicking on the "Deploy & Run Transactions" tab in the left-hand sidebar. Select the "ProhectMod1" contract from the dropdown menu, and then click on the "Deploy" button.

Once the contract is deployed, you can interact with it by calling the different functions. Click on the "ProhectMod1" contract in the left-hand sidebar, and then click on the one of the functions. Finally, click on the functions button to execute the function and retrieve the value and/or error message.

## Authors

syvillacruz
