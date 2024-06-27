# ETH-AVAX-Assessment1

This project demonstrates the usage of require(), assert(), and revert() statements in a Solidity smart contract. The ProjectContract is a basic Ethereum smart contract written in Solidity. It allows users to deposit (stake) Ether into the contract and allows the shopkeeper (the contract deployer) to withdraw Ether from the contract. This contract demonstrates basic functionalities such as asserting contract balance and forcing reverts.

## Description

This Solidity smart contract is designed for reveiwing purpose to illustrate basic error handling and conditional checks in Solidity.

## Getting Started

### Installing

* Clone the repository to your local machine: https://github.com/Lavisha13/ETH-AVAX-Assessment1/edit/main/README.md
* Navigate to the project directory: ETH-AVAX Assessment1.

### Executing program

* Deploy the Contract:

Use Remix to deploy the contract to an Ethereum network.

* Interact with the Contract:

1. Use the deposit function to send Ether to the contract:
```
// In Remix or your chosen environment, call the deposit function and send some Ether
projectContract.deposit({ value: web3.utils.toWei('2', 'ether') });
```
2.Use the withdraw function to withdraw Ether (only the owner can call this function):
```
// Ensure you are the owner and call the withdraw function
projectContract.withdraw(web3.utils.toWei('0.3', 'ether'));
```
3.Use the checkBalance function to verify that the balance is non-negative:
```
// Call the checkBalance function
projectContract.checkBalance();
```
4.Use the causeRevert function to intentionally trigger a revert:
```
// Call the causeRevert function
projectContract.Revert();
```

## Help

If you encounter any issues:

Ensure that you have a valid Ethereum account with sufficient funds.

Make sure you are using a compatible Solidity version (^0.8.0).

Check the Remix console or your development environment's logs for detailed error messages.

## Authors

* Lavisha 
* Mail: lavishab.0096@gmail.com

## License

This project is licensed under the MIT License - see the LICENSE.md file for details.
