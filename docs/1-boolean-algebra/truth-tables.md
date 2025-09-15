---
layout: default
title: Truth Tables
nav_order: 2
parent: Boolean Algebra
---

# Truth Tables

[&laquo; Return to Boolean Algebra Chapter](index.md)

Truth tables are systematic ways to represent all possible combinations of input values and their corresponding output values for Boolean expressions. They provide a complete and unambiguous way to define logical functions and verify Boolean identities.

## What is a Truth Table?

A truth table lists all possible combinations of input variables and shows the resulting output for each combination. For n input variables, there are 2^n possible combinations.

## Basic Truth Tables

### NOT Gate Truth Table

| A | NOT A |
|---|-------|
| 0 |   1   |
| 1 |   0   |

### AND Gate Truth Table

| A | B | A AND B |
|---|---|---------|
| 0 | 0 |    0    |
| 0 | 1 |    0    |
| 1 | 0 |    0    |
| 1 | 1 |    1    |

### OR Gate Truth Table

| A | B | A OR B |
|---|---|--------|
| 0 | 0 |   0    |
| 0 | 1 |   1    |
| 1 | 0 |   1    |
| 1 | 1 |   1    |

## Constructing Truth Tables

### Step-by-Step Process

1. **Count Variables**: Determine the number of input variables (n)
2. **Calculate Rows**: Create 2^n rows for all possible combinations
3. **List Combinations**: Write all possible binary combinations
4. **Evaluate Expression**: Calculate the output for each combination
5. **Fill Table**: Complete the truth table with results

### Example: Three-Variable Expression

Let's create a truth table for: F = AB + C

| A | B | C | AB | AB + C |
|---|---|---|----|--------|
| 0 | 0 | 0 |  0 |    0   |
| 0 | 0 | 1 |  0 |    1   |
| 0 | 1 | 0 |  0 |    0   |
| 0 | 1 | 1 |  0 |    1   |
| 1 | 0 | 0 |  0 |    0   |
| 1 | 0 | 1 |  0 |    1   |
| 1 | 1 | 0 |  1 |    1   |
| 1 | 1 | 1 |  1 |    1   |

## Using Truth Tables for Verification

### Verifying Boolean Identities

Truth tables can prove that two Boolean expressions are equivalent by showing they produce identical outputs for all input combinations.

**Example**: Prove that A + AB = A

| A | B | AB | A + AB | A |
|---|---|----|--------|---|
| 0 | 0 |  0 |    0   | 0 |
| 0 | 1 |  0 |    0   | 0 |
| 1 | 0 |  0 |    1   | 1 |
| 1 | 1 |  1 |    1   | 1 |

Since the columns for "A + AB" and "A" are identical, the expressions are equivalent.

### Verifying De Morgan's Laws

**First Law**: A + B̄ = ĀB̄

| A | B | A+B | A + B̄ | Ā | B̄ | ĀB̄ |
|---|---|-----|-------|----|----|----|
| 0 | 0 |  0  |   1   | 1  | 1  |  1  |
| 0 | 1 |  1  |   0   | 1  | 0  |  0  |
| 1 | 0 |  1  |   0   | 0  | 1  |  0  |
| 1 | 1 |  1  |   0   | 0  | 0  |  0  |

The columns for "A + B̄" and "ĀB̄" are identical, proving the law.

## Common Truth Table Patterns

### XOR (Exclusive OR) Gate

| A | B | A XOR B |
|---|---|---------|
| 0 | 0 |    0    |
| 0 | 1 |    1    |
| 1 | 0 |    1    |
| 1 | 1 |    0    |

**Note**: XOR returns 1 when inputs are different, 0 when they're the same.

### NAND Gate

| A | B | A NAND B |
|---|---|----------|
| 0 | 0 |    1     |
| 0 | 1 |    1     |
| 1 | 0 |    1     |
| 1 | 1 |    0     |

**Note**: NAND is the complement of AND.

### NOR Gate

| A | B | A NOR B |
|---|---|---------|
| 0 | 0 |    1    |
| 0 | 1 |    0    |
| 1 | 0 |    0    |
| 1 | 1 |    0    |

**Note**: NOR is the complement of OR.

## Tips for Working with Truth Tables

1. **Systematic Approach**: Always list input combinations in binary order (000, 001, 010, 011, etc.)
2. **Intermediate Steps**: Show intermediate calculations for complex expressions
3. **Double-Check**: Verify your work by checking a few rows manually
4. **Use for Simplification**: Truth tables can help identify patterns for simplification
5. **Complete Coverage**: Ensure all 2^n combinations are included

## Applications

Truth tables are used in:
- **Digital Circuit Design**: Specifying circuit behavior
- **Boolean Expression Simplification**: Finding equivalent simpler forms
- **Logic Verification**: Proving logical equivalences
- **Programming**: Understanding conditional logic
- **Database Queries**: Understanding SQL logical operations

## Next Steps

Now that you understand truth tables, you're ready to learn about logic gates, which are the physical implementations of these Boolean operations in digital circuits.

**[Continue to Logic Gates →](logic-gates.md)**
