---
layout: default
title: Logic Gates
nav_order: 3
parent: Boolean Algebra
---

# Logic Gates

[&laquo; Return to Boolean Algebra Chapter](index.md)

Logic gates are physical devices that implement Boolean operations in digital circuits. They are the building blocks of all digital systems, from simple calculators to complex computers. Each logic gate performs a specific Boolean function and can be combined to create more complex circuits.

## What are Logic Gates?

Logic gates are electronic circuits that take one or more binary inputs and produce a single binary output based on the Boolean operation they implement. They are typically implemented using transistors and form the foundation of digital electronics.

## Basic Logic Gates

### 1. NOT Gate (Inverter)

**Symbol**: 
```
    A ──┐
        │○── NOT A
        └─
```

**Function**: Inverts the input
- Input: A
- Output: NOT A (Ā)

**Truth Table**:
| A | NOT A |
|---|-------|
| 0 |   1   |
| 1 |   0   |

**Characteristics**:
- Single input, single output
- Also called an inverter
- Fundamental building block for other gates

### 2. AND Gate

**Symbol**:
```
    A ──┐
        │&── A AND B
    B ──┘
```

**Function**: Output is 1 only when all inputs are 1
- Inputs: A, B
- Output: A AND B (AB)

**Truth Table**:
| A | B | A AND B |
|---|---|---------|
| 0 | 0 |    0    |
| 0 | 1 |    0    |
| 1 | 0 |    0    |
| 1 | 1 |    1    |

**Characteristics**:
- Multiple inputs possible (2, 3, 4, etc.)
- Output is 1 only when ALL inputs are 1
- Used for enabling/disabling signals

### 3. OR Gate

**Symbol**:
```
    A ──┐
        │≥1── A OR B
    B ──┘
```

**Function**: Output is 1 when any input is 1
- Inputs: A, B
- Output: A OR B (A + B)

**Truth Table**:
| A | B | A OR B |
|---|---|--------|
| 0 | 0 |   0    |
| 0 | 1 |   1    |
| 1 | 0 |   1    |
| 1 | 1 |   1    |

**Characteristics**:
- Multiple inputs possible
- Output is 1 when ANY input is 1
- Used for combining signals

## Universal Gates

### NAND Gate (NOT AND)

**Symbol**:
```
    A ──┐
        │&○── A NAND B
    B ──┘
```

**Function**: Complement of AND operation
- Output: AB̄

**Truth Table**:
| A | B | A NAND B |
|---|---|----------|
| 0 | 0 |    1     |
| 0 | 1 |    1     |
| 1 | 0 |    1     |
| 1 | 1 |    0     |

**Why Universal**: Can implement any Boolean function
- NOT A = A NAND A
- A AND B = (A NAND B) NAND (A NAND B)
- A OR B = (A NAND A) NAND (B NAND B)

### NOR Gate (NOT OR)

**Symbol**:
```
    A ──┐
        │≥1○── A NOR B
    B ──┘
```

**Function**: Complement of OR operation
- Output: A + B̄

**Truth Table**:
| A | B | A NOR B |
|---|---|---------|
| 0 | 0 |    1    |
| 0 | 1 |    0    |
| 1 | 0 |    0    |
| 1 | 1 |    0    |

**Why Universal**: Can implement any Boolean function
- NOT A = A NOR A
- A OR B = (A NOR B) NOR (A NOR B)
- A AND B = (A NOR A) NOR (B NOR B)

## Specialized Gates

### XOR Gate (Exclusive OR)

**Symbol**:
```
    A ──┐
        │=1── A XOR B
    B ──┘
```

**Function**: Output is 1 when inputs are different
- Output: A ⊕ B

**Truth Table**:
| A | B | A XOR B |
|---|---|---------|
| 0 | 0 |    0    |
| 0 | 1 |    1    |
| 1 | 0 |    1    |
| 1 | 1 |    0    |

**Applications**:
- Binary addition (sum bit)
- Parity checking
- Encryption algorithms

### XNOR Gate (Exclusive NOR)

**Symbol**:
```
    A ──┐
        │=1○── A XNOR B
    B ──┘
```

**Function**: Complement of XOR
- Output: A ⊕ B̄

**Truth Table**:
| A | B | A XNOR B |
|---|---|----------|
| 0 | 0 |    1     |
| 0 | 1 |    0     |
| 1 | 0 |    0     |
| 1 | 1 |    1     |

## Gate Combinations

### Building Complex Circuits

Logic gates can be combined to create more complex functions:

**Example**: Half Adder
- Inputs: A, B (two bits to add)
- Outputs: Sum (A ⊕ B), Carry (AB)

**Circuit**:
```
    A ──┐
        │=1── Sum
    B ──┘
    
    A ──┐
        │&── Carry
    B ──┘
```

### Gate Delays and Timing

**Propagation Delay**: Time for output to change after input changes
- NOT: ~1ns
- AND/OR: ~2-3ns
- Complex gates: Longer delays

**Timing Considerations**:
- Critical for high-speed circuits
- Affects maximum clock frequency
- Important for synchronous design

## Practical Applications

### Digital Systems
- **Processors**: ALU operations, control logic
- **Memory**: Address decoding, read/write control
- **I/O**: Interface circuits, protocol handling

### Everyday Electronics
- **Calculators**: Arithmetic operations
- **Remote Controls**: Signal encoding
- **Digital Clocks**: Time display logic

### Computer Architecture
- **CPU Design**: Instruction decoding, data paths
- **Cache Systems**: Hit/miss detection
- **Bus Controllers**: Data routing

## Gate Implementation Technologies

### TTL (Transistor-Transistor Logic)
- Bipolar transistors
- 5V power supply
- Fast switching
- Higher power consumption

### CMOS (Complementary Metal-Oxide-Semiconductor)
- MOSFET transistors
- Low power consumption
- Wide voltage range
- Most common in modern ICs

### ECL (Emitter-Coupled Logic)
- Very high speed
- High power consumption
- Used in high-frequency applications

## Key Concepts to Remember

1. **Basic Gates**: NOT, AND, OR are fundamental
2. **Universal Gates**: NAND and NOR can implement any function
3. **Symbols**: Standard symbols represent each gate type
4. **Truth Tables**: Define gate behavior completely
5. **Combinations**: Gates can be combined for complex functions
6. **Timing**: Propagation delays affect circuit performance
7. **Technology**: Different implementation technologies have trade-offs

## Next Steps

You've now completed the Boolean Algebra chapter! You understand:
- The mathematical foundation (Boolean algebra basics)
- Systematic representation (truth tables)
- Physical implementation (logic gates)

These concepts form the foundation for understanding digital circuits, computer architecture, and many aspects of computer science.

**[Return to Boolean Algebra Chapter →](index.md)**
