---
layout: default
title: Basics of Boolean Algebra
nav_order: 1
parent: Boolean Algebra
---

# Basics of Boolean Algebra

[&laquo; Return to Boolean Algebra Chapter](index.md)

Boolean algebra is a branch of mathematics that deals with binary variables and logical operations. It was developed by George Boole in the 19th century and forms the mathematical foundation for digital logic and computer science.

## Binary Variables

In Boolean algebra, we work with **binary variables** that can only have two possible values:
- **0** (False, Low, Off)
- **1** (True, High, On)

These variables are typically represented by letters like A, B, C, etc.

## Basic Logical Operations

### 1. NOT Operation (Negation)

The NOT operation inverts the value of a variable:
- NOT 0 = 1
- NOT 1 = 0

**Symbols used:**
- `¬A` (logical notation)
- `$\overline{A}$` (mathematical notation)
- `!A` (programming notation)

### 2. AND Operation (Conjunction)

The AND operation returns 1 only when ALL inputs are 1:
- 0 AND 0 = 0
- 0 AND 1 = 0
- 1 AND 0 = 0
- 1 AND 1 = 1

**Symbols used:**
- `A ∧ B` (logical notation)
- `$AB$` (mathematical notation)
- `A && B` (programming notation)

### 3. OR Operation (Disjunction)

The OR operation returns 1 when ANY input is 1:
- 0 OR 0 = 0
- 0 OR 1 = 1
- 1 OR 0 = 1
- 1 OR 1 = 1

**Symbols used:**
- `A ∨ B` (logical notation)
- `$A + B$` (mathematical notation)
- `A || B` (programming notation)

## Basic Boolean Laws

### Identity Laws
- A + 0 = A
- A1 = A

### Domination Laws
- A + 1 = 1
- A0 = 0

### Idempotent Laws
- A + A = A
- AA = A

### Complement Laws
- A + Ā = 1
- AĀ = 0

### Double Negation Law
- Ā̄ = A

### Commutative Laws
- A + B = B + A
- AB = BA

### Associative Laws
- (A + B) + C = A + (B + C)
- (AB)C = A(BC)

### Distributive Laws
- A(B + C) = AB + AC
- A + BC = (A + B)(A + C)

### De Morgan's Laws
- A + B̄ = ĀB̄
- AB̄ = Ā + B̄

## Mathematical Notation

With KaTeX integration, we can now display Boolean algebra expressions with proper mathematical formatting:

$$
\begin{align}
A + \overline{A} &= 1 \\
A \cdot \overline{A} &= 0 \\
\overline{\overline{A}} &= A \\
\overline{AB} &= \overline{A} + \overline{B} \\
\overline{A + B} &= \overline{A} \cdot \overline{B}
\end{align}
$$

## Examples

### Example 1: Simple Boolean Expression
Evaluate: AB + ĀB̄

If A = 1 and B = 0:
- AB = 1 · 0 = 0
- Ā = 0, B̄ = 1
- ĀB̄ = 0 · 1 = 0
- Result: 0 + 0 = 0

### Example 2: Using Boolean Laws
Simplify: A + AB

Using the distributive law:
A + AB = A(1 + B) = A1 = A

## Key Concepts to Remember

1. **Binary System**: Boolean algebra only uses 0 and 1
2. **Three Basic Operations**: NOT, AND, OR
3. **Boolean Laws**: Mathematical properties that help simplify expressions
4. **Precedence**: NOT has highest precedence, then AND, then OR
5. **Parentheses**: Use parentheses to clarify order of operations

## Next Steps

Now that you understand the basics of Boolean algebra, you're ready to learn about truth tables, which provide a systematic way to represent and analyze Boolean expressions.

**[Continue to Truth Tables →](truth-tables.md)**
