# apy_calculator

A C++ console program that calculates the Annual Percentage Yield (APY) and projected final balance for a deposit, based on user-provided rate, term, and compounding frequency.

## Overview

**APY Calculator** is an interactive console application that helps a user understand how their money grows over time. It greets the user by name, collects their deposit amount, annual percentage rate (APR), term length, and compounding frequency, then calculates the resulting APY and the projected final balance.

The program is built to handle real-world input formatting — it accepts deposit amounts with commas (e.g., `1,000`) and APR values with or without a percent sign (e.g., `4.5%`), and it formats the final result with comma separators for readability.

## How to Use

1. Enter your first name.
2. Enter your deposit amount (commas are allowed, e.g., `2,500`).
3. Enter your APR in percent form (e.g., `4.5` or `4.5%`).
4. Enter your term length in years.
5. Enter how many times per year interest is compounded.
6. The program displays your APY and projected final balance.

### Compounding Frequency Reference

| Frequency  | Value |
| ---------- | :---: |
| Daily      | 365   |
| Weekly     | 52    |
| Bi-weekly  | 26    |
| Monthly    | 12    |
| Quarterly  | 4     |
| Bi-yearly  | 2     |
| Yearly     | 1     |

## Getting Started

### Prerequisites

A C++ compiler such as `g++` (part of GCC) or any standard C++ IDE.

### Compile

```bash
g++ apy_calculator.cpp -o apy_calculator
```

### Run

```bash
./apy_calculator
```

On Windows:

```bash
apy_calculator.exe
```

## Example

```
Welcome to the APY (Annual Percentage Yield) calculator!
What is your first name?: Abigail

Hello, Abigail!
What is your deposit amount?: $2,500

What is your Annual Percent Rate (APR) in percent form?: 4.5%

How many years is your term for?: 3

How many times a year is the interest being compounded?
(Daily = 365, Weekly = 52, Bi-weekly = 26, Monthly = 12,
Quarterly = 4, Bi-yearly = 2, Yearly = 1): 12
```

## What This Project Demonstrates

- Parsing and cleaning user input (stripping commas and percent signs)
- String and stream handling with `<sstream>` and `<string>`
- Mathematical computation using the compound-interest and APY formulas
- Number formatting with comma separators for readable output
- Modular design with dedicated helper functions

## Built With

- **C++**
- Standard Library (`<iostream>`, `<string>`, `<sstream>`, `<cmath>`, `<algorithm>`)

## Author

Abigail Norton
