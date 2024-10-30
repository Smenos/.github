
# Anlytical Psychology Quantized and Supercharged 🔥🔥🔥

This enterprise introduces an algebraic model named **Tektōn** aswell as a family of tools based on our framework which we call _Reaper_ for computational psychology, where personality and cognition are represented as functional elements using specific mathematical operations and relationships. Here we provides a sample overview of the syntax, rules, and operations for manipulating these elements within the model.

---

## Table of Contents
- [Introduction](#introduction)
- [Definitions](#definitions)
- [Algebraic Rules](#algebraic-rules)
  - [Basic Syntax](#basic-syntax)
  - [Operators](#operators)
  - [Priority Rules](#priority-rules)
- [Usage Examples](#usage-examples)
- [Contributors](#contributors)

---


## Definitions

| Symbol      | Name           | Density                             |
|-----------------|------------------|---------------------------------------|
| `Si`     | Introverted Sensing        | `Very Dense`      |
| `Ni`     | Introverted Intuition       | `Very Dense`   |
| `Ne`     | Extraverted Intuition    | `Dense`      |
| `Fi`     | Introverted Feeling       | `Dense` |
| `Te`     | Extraverted Thinking        |  `Somewhat Light`  |
| `Fe`     | Extraverted Feeling| `Somewhat light`  |
| `Ti`     | Introverted Thinking        | `Light`       |
| `Se`    | Extraverted Sensing       | ` Very Light`       |


## Introduction
This model aims to describe elements of personality and cognition using algebraic rules. Functions representing dimensions of personality and cognitive processes can interact, combine, and influence each other through defined operations. These operations and rules simulate complex psychological dynamics and provide insights into cognitive processes and personality traits through mathematical notation.

## Algebraic Rules

### Basic Syntax
- **Terms** are grouped by parentheses, e.g., `(Se ~ Ti)`.
- **Operators**:
  - `+` combines terms.
  - `i` represents a negative charge, and `e` a positive charge.
- **Dimensions**:
  - N (Ne, Ni)
  - F (Fe, Fi)
  - T (Te, Ti)
  - S (Se, Si)
- **Coefficients**:
  - Coefficients adjacent to functions describe mass.
  - Coefficients outside of parentheses describe acceleration and do not affect internal mass coefficients.

**Example**: 
`2(Se ~ Ti)` – here `2` denotes acceleration.

### Operators
- **Orbital (`~`)**: Describes a relationship where a T or F function orbits an S or P function. No coefficient exchange occurs.
- **Drag (`→`)**: Represents a function pulling an opposite-charge and opposite-domain function. Not equivalent to voltage.
- **Opposition (`oo`)**: Subtracts functions of the same domain with different charges, producing a drag.
  - Example: `Fe oo Fi`, `Ne oo Ni`
- **Non-interaction (`|`)**: Indicates that two terms cannot interact due to a lack of rules for reaction.
- **Subtraction with drag rule**:
  - If the drag coefficient is larger, it "carries" the difference. 
  - Example: `7Se oo 5Si = 2Se → Ni`

### Priority Rules
1. **Addition of Same Functions**: Functions of the same type (e.g., `Se`) add their coefficients.
   - Example: `(2Se) + (2Se) = (4Se)`
2. **Order of Operations**: Always solve for subtraction (`oo`) before other operations, as this can produce new drag reactions.
3. **Single Drag Reactions**: Within a single term, drag reactions within the same domain accumulate until only one remains.

### Drag Rules
Refer to the drag rule table for specific rules based on different function interactions.

### Drag Rules Table

The following table lists outcomes for specific drag reactions using the opposition operator (`oo`). In each case, the function with the higher coefficient "carries" the drag to the opposite dimension and charge.

| Expression      | Result           | Reasoning                             |
|-----------------|------------------|---------------------------------------|
| `2Se oo Si`     | `Se → Ni`        | `Se` is higher, carries the drag      |
| `2Si oo Se`     | `Si → Ne`        | `Si` is higher, becomes the carrier   |
| `2Ne oo Ni`     | `Ne → Si`        | `Ne` is higher, carries the drag      |
| `2Ni oo Ne`     | `Ni → Se`        | `Ni` is higher, becomes the carrier   |
| `2Te oo Ti`     | `Te → Fi`        | `Te` is higher, carries the drag      |
| `2Ti oo Te`     | `Ti → Fe`        | `Ti` is higher, becomes the carrier   |
| `2Fe oo Fi`     | `Fe → Ti`        | `Fe` is higher, carries the drag      |
| `3Fi oo 2Fe`    | `Fi → Te`        | `Fi` is higher, carries the drag      |

Each drag reaction creates a directional force based on the opposing domain and charge, simplifying complex expressions by reducing redundant reactions.


---

## Usage Examples

### Example 1: Solving a Complex Reactor
```text
Reactor = 40(5Se ~ 3Ti) + 9(8Ni → 3Se ) + 10( 2Se ~ 2Se oo 3Si)

Step-by-Step Solution:
1. Sum all instances of `Se` as it's the most common.
   Result: `51(10Se ~ 3Ti → 8Ni) + 8(2Ne → Si)`

2. Carry `Ni` by the largest `Se` function, adjusting acceleration.
   Result: `59(10Se ~ 3Ti → 8Ni oo 2Ne → Si)`

3. Prioritize subtraction (`oo`) to create a drag.
   Result: `59(10Se ~ 3Ti → 6Ni → 2Se oo Si)`

4. Final result after reduction:
   Result: `59(11Se ~ 3Ti → 9Ni)`
```

### Example 2: Solving a Complex Reactor
```text
2(Te ~ Si) | 4(Fe ~ Ni) + (2Ne oo Ni) + 4(Se)

Solution Steps:
1. Solve reduction (`oo`).
2. Convert reductions and remove the `|` operator.
   Result: `2(Te ~ Si) + 4(Fe ~ 4Se → Ni)`

3. Complete reduction with final adjustment:
   Result: `6(Te ~ Si oo 4Se → Ni)`

Final simplified expression:
   `6(Te ~ 3Se → 2Ni)`
```

![image](https://github.com/user-attachments/assets/84c216e4-737b-458e-a0e2-9445c0299f59)


### We strongly believe in descentralization - Reaper is entirely self-hosted and able to run locally.
