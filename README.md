# BasicMath
The BasicMath Solidity contract provides basic arithmetic functions to add, subtract, multiply, and divide two unsigned integers (uint256). It is a simple utility contract designed to demonstrate fundamental mathematical operations in Solidity.

## Description
The BasicMath contract includes four pure functions to perform basic arithmetic:

add(uint256 a, uint256 b): Adds two unsigned integers and returns the result.
subtract(uint256 a, uint256 b): Subtracts one unsigned integer from another and returns the result.
multiply(uint256 a, uint256 b): Multiplies two unsigned integers and returns the result.
divide(uint256 a, uint256 b): Divides one unsigned integer by another, ensuring the divisor is non-zero. If the divisor is zero, the function will revert with an error message "Cannot divide by zero."
##Getting Started
### Installing
To use this contract, you can compile and deploy it using an Ethereum development environment like Remix.

Open the Remix IDE.
Create a new file with a .sol extension (e.g., BasicMath.sol).
Copy and paste the following code into the file:
solidity
Copy code
    
    // SPDX-License-Identifier: MIT
    pragma solidity ^0.8.26;

    contract BasicMath {
    
    // Add two numbers
    function add(uint256 a, uint256 b) public pure returns (uint256) {
        return a + b;
    }
    
    // Subtract two numbers
    function subtract(uint256 a, uint256 b) public pure returns (uint256) {
        return a - b;
    }

    // Multiply two numbers
    function multiply(uint256 a, uint256 b) public pure returns (uint256) {
        return a * b;
    }

    // Divide two numbers
    function divide(uint256 a, uint256 b) public pure returns (uint256) {
        require(b != 0, "Cannot divide by zero");
        return a / b;
    }
    }
## Executing Program

Compile the contract using the Solidity compiler in Remix. Ensure the compiler version is set to 0.8.26 or a compatible version.
Deploy the contract using the "Deploy & Run Transactions" tab.
After deploying, you can interact with the following functions:
add(uint256 a, uint256 b): Adds a and b and returns the result.
subtract(uint256 a, uint256 b): Subtracts b from a and returns the result.
multiply(uint256 a, uint256 b): Multiplies a and b and returns the result.
divide(uint256 a, uint256 b): Divides a by b, ensuring b is non-zero.
## Help
Make sure that when using the divide function, the second parameter (b) is not zero, as it will result in an error.
Ensure you're using the correct Solidity compiler version 0.8.26 or a compatible one.
## Authors
Aakash Raj
Email: akashraj2708@gmail.com
## License
This project is licensed under the MIT License - see the LICENSE.md file for details.
