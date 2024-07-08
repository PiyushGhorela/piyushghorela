Certainly! Here is the raw content for the README file for the `Loan.sol` contract:

```markdown
# Loan Smart Contract

## Description

This Solidity program defines a smart contract `Loan` that simulates loan eligibility checks and loan disbursement based on collateral. It includes functions to determine loan eligibility based on debt-to-income ratio and to calculate the maximum loan amount against collateral.

## Features

- **Loan Eligibility Check**: Checks if a borrower's debt-to-income ratio meets the maximum allowed threshold.
- **Loan Amount Calculation**: Calculates the maximum loan amount that can be disbursed based on collateral value.
- **Loan Disbursement**: Simulates a loan disbursement process, illustrating transaction failure handling.

## Contract Details

- **Solidity Version**: `0.8.0`
- **SPDX-License-Identifier**: MIT

## Functions

### `checkEligibility(uint income, uint currentDebt)`

- **Description**: Checks if a borrower's debt-to-income ratio is within acceptable limits.
- **Parameters**:
  - `income`: Borrower's monthly income.
  - `currentDebt`: Borrower's current total debt.
- **Behavior**:
  - Calculates the debt-to-income ratio.
  - Throws an error if the debt-to-income ratio exceeds the set maximum.

### `calculateLoanAmount(uint collateralValue)`

- **Description**: Calculates the maximum loan amount that can be disbursed based on collateral.
- **Parameters**:
  - `collateralValue`: Value of the collateral put up for the loan.
- **Returns**:
  - `uint`: Maximum loan amount that can be disbursed.
- **Behavior**:
  - Computes the loan amount as 60% of the collateral value.
  - Asserts that the loan amount is greater than zero.

### `disburseLoan()`

- **Description**: Simulates the process of loan disbursement.
- **Behavior**:
  - Reverts the transaction with a specific message, mimicking a failed loan disbursement.

## Getting Started

### Prerequisites

- Ensure you have an Ethereum development environment set up with tools like Remix or Truffle.

### Installing

1. Clone the repository:

   ```bash
   git clone <repository_url>
   ```

2. Open the contract file `Loan.sol` in your preferred Solidity development environment.

### Compiling the Contract

- Compile the `Loan.sol` contract using Solidity compiler version `0.8.0` or higher.

### Deploying the Contract

- Deploy the compiled contract on an Ethereum testnet or a local blockchain for testing.

### Testing

- Use Remix IDE or other testing frameworks to interact with deployed contracts.
- Test scenarios such as loan eligibility, loan amount calculation, and loan disbursement failure handling.

## Authors

- Metacrafter Chris ([@PiyushGhorela](https://github.com/PiyushGhorela))

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details.
```

You can save this content into a file named `README.md` and include it in your project directory alongside your `Loan.sol` contract. Adjust any URLs or specific details as necessary for your project context.
