---
layout: default
title: Math Notation Test
nav_order: 999
---

# Mathematical Notation Test

This page demonstrates the KaTeX integration for Boolean algebra notation.

## Inline Math Examples

- The complement of A: $\overline{A}$
- AND operation: $AB$
- OR operation: $A + B$
- De Morgan's Law: $\overline{AB} = \overline{A} + \overline{B}$

## Block Math Examples

### Boolean Laws

$$
\begin{align}
A + \overline{A} &= 1 \\
A \cdot \overline{A} &= 0 \\
\overline{\overline{A}} &= A
\end{align}
$$

### Truth Table

$$
\begin{array}{c|c|c|c}
A & B & AB & A + B \\
\hline
0 & 0 & 0 & 0 \\
0 & 1 & 0 & 1 \\
1 & 0 & 0 & 1 \\
1 & 1 & 1 & 1 \\
\end{array}
$$

### De Morgan's Laws

$$
\begin{align}
\overline{A + B} &= \overline{A} \cdot \overline{B} \\
\overline{AB} &= \overline{A} + \overline{B}
\end{align}
$$

## Complex Boolean Expression

$$
F = \overline{AB} + C\overline{D} + \overline{A}BC
$$

