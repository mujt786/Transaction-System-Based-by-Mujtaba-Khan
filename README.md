# Transaction System (Transaction Validation)

This project is a dynamic **Transaction System** model that leverages formal methods and the Z3 theorem prover to ensure system correctness. It includes features for adding and removing transactions, validating system constraints, and maintaining transaction history while preventing invalid states.

## Project Overview

The Transaction System validates transactions while adhering to the following constraints:

- **No Overdraft**: The account balance must never be negative.
- **Unique Transaction IDs**: All transactions must have unique identifiers.
- **Positive Transaction Amounts**: Only positive transaction amounts are allowed.
- **Dynamic Constraints**: The system dynamically updates and verifies constraints after each modification.

This implementation demonstrates the importance of formal verification in preventing errors and ensuring system reliability.

## Features

- Add transactions dynamically.
- Remove transactions by ID.
- Validate constraints in real-time using Z3.
- Prevent invalid states, such as:
  - Duplicate transaction IDs.
  - Negative transaction amounts.
  - Overdrafts.

## System Requirements

- Python 3.7 or above
- Z3 Theorem Prover (`z3-solver` package)
