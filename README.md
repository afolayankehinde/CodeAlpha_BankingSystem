# Banking System

A C++ console program that simulates a simple bank. It uses classes
for customers, accounts and transactions.

## What it does
- Creates customers, each with their own account number
- Refuses an account number that already exists
- Deposits and withdraws money
- Refuses withdrawals larger than the balance, and amounts of zero or less
- Transfers money between two accounts
- Keeps a transaction history for every account and shows it with the balance
- Shows a clear message when an account is not found
- Keeps showing the menu until the user chooses Exit

## How it is built
- `Transaction` stores the type and amount of each money movement
- `Account` holds the balance and the history, and does the deposits, withdrawals and transfers
- `Customer` holds a name and the account they own
- `findCustomer` looks up a customer by account number

## How to run
```
g++ bank.cpp -o bank
./bank
```
Customers are kept in memory while the program runs, so they are cleared when it exits.

Built as part of my CodeAlpha C++ Programming internship.
