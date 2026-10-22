# Bank Account Management Program

## Overview

The **Bank Account Management Program** is a JavaScript project built as part of the freeCodeCamp curriculum. It simulates basic banking operations, allowing users to deposit money, withdraw money, check their account balance, and view their transaction history.

The project demonstrates object-oriented programming concepts, class methods, transaction management, and array manipulation in JavaScript.

## Features

- **Account Initialization:** Creates a bank account with an initial balance of `$0` and an empty transaction history.
- **Deposit Money:** Deposits positive amounts, updates the account balance, and records successful transactions.
- **Withdraw Money:** Withdraws money when the amount is valid and sufficient funds are available.
- **Balance Inquiry:** Displays the current account balance.
- **Deposit History:** Lists all successful deposits.
- **Withdrawal History:** Lists all successful withdrawals.
- **Input Validation:** Rejects invalid deposits and withdrawals that exceed the available balance.
- **Transaction Records:** Stores each successful transaction as an object containing its type and amount.

## Technologies Used

- JavaScript (ES6+)
- Object-Oriented Programming
- Arrays and Objects
- Array Methods: `filter()`, `map()`, and `join()`
- Template Literals

## Project Structure

```text
bank-account-management/
└── script.js
```

The `script.js` file contains the `BankAccount` class, its methods, and an example account named `myAccount`.

## How It Works

### 1. Create a Bank Account

The `BankAccount` class uses a constructor to initialize the account balance and transaction history.

```javascript
const myAccount = new BankAccount();
```

### 2. Deposit Money

The `deposit(amount)` method adds money to the account when the amount is greater than zero.

```javascript
myAccount.deposit(200);
```

### 3. Withdraw Money

The `withdraw(amount)` method subtracts money from the account only when the withdrawal amount is valid and does not exceed the available balance.

```javascript
myAccount.withdraw(50);
```

### 4. Check the Balance

The `checkBalance()` method returns the current account balance.

```javascript
console.log(myAccount.checkBalance());
```

### 5. View Transaction History

The program provides separate methods for listing deposits and withdrawals.

```javascript
console.log(myAccount.listAllDeposits());
console.log(myAccount.listAllWithdrawals());
```

## Example Output

After performing the sample transactions, the account balance and transaction history can be displayed as follows:

```text
Current balance: $350
Deposits: 200,150,100,25
Withdrawals: 50,75
```

## Key Learning Outcomes

Through this project, I practised:

- Defining JavaScript classes and constructors.
- Creating and using class methods.
- Understanding the `this` keyword.
- Managing state through object properties.
- Storing transaction records in arrays of objects.
- Validating input and handling invalid operations.
- Filtering arrays using `.filter()`.
- Transforming data using `.map()`.
- Converting arrays into strings using `.join()`.
- Formatting output using template literals.

## How to Run

1. Clone or download this repository.
2. Open the project folder in Visual Studio Code.
3. Open the terminal in the project directory.
4. Run the program using Node.js:

```bash
node script.js
```

Alternatively, copy the code into a browser console or the freeCodeCamp editor.

## Project Status

**Completed** — built to satisfy the freeCodeCamp Bank Account Management Program user stories and tests.

## Author

**Collins Mwangi**

Software Engineering Graduate | JavaScript Learner

## Acknowledgements

- [freeCodeCamp](https://www.freecodecamp.org/) — for providing the project requirements and learning resources.
