# Rural Bank Account Management System (RBAMS)

## Overview
A console-based Java application to manage savings and current accounts for rural customers like Sita Devi from Myagdi, Nepal.

## Features
- Deposit & Withdraw operations
- Interest addition for Savings Account
- Overdraft handling in Current Account
- Custom exception handling (`InsufficientBalanceException`)
- Object-Oriented Programming: Abstraction, Encapsulation, Inheritance, Polymorphism

## Class Design

### `BankAccount` (Abstract Class)
- Attributes: `accountHolderName`, `accountNumber`, `balance`
- Methods: `deposit()`, `withdraw()`, `displayDetails()`

### `SavingsAccount` (Extends `BankAccount`)
- Adds: Interest application

### `CurrentAccount` (Extends `BankAccount`)
- Adds: Overdraft limit handling

### `Customer`
- Holds multiple `BankAccount` objects

### `InsufficientBalanceException`
- Custom exception thrown for withdrawal errors

## Screenshots

### Operation
![Screenshot](Bank.png)


## How to Compile & Run
```bash
javac RBAMS.java
java RBAMS
