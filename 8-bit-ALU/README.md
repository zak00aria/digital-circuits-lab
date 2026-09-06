# 8-Bit ALU

A simple 8-bit Arithmetic Logic Unit built and simulated using [CircuitVerse](https://circuitverse.org).

The ALU performs arithmetic, logical, and bit-shifting operations on two 8-bit binary inputs. The selected operation is determined by control signals. After each operation, the result is stored in the output register and the flags register is updated according to the result.

## Preview

![8-bit ALU demonstration](./8-bit-ALU.gif)

## Circuit Simulation

The circuit was designed and simulated in CircuitVerse. You can view how it was built and try the ALU using the link below:

[Open the 8-bit ALU simulation](https://circuitverse.org/users/25835/projects/alu-511675e2-545b-43ad-bfaf-ea58a4da9bfa)

## Supported Operations

| Operation | Description | Result |
|-----------|-------------|--------|
| `ADD` | Adds the two inputs | `a + b` |
| `SUB` | Subtracts `b` from `a` | `a - b` |
| `SHL` | Shifts `a` left by one bit | `a << 1` |
| `SHR` | Shifts `a` right by one bit | `a >> 1` |
| `AND` | Bitwise AND | `a AND b` |
| `NOT` | Bitwise NOT of `a` | `NOT a` |
| `OR` | Bitwise OR | `a OR b` |
| `XOR` | Bitwise exclusive OR | `a XOR b` |

## Inputs and Outputs

| Signal | Description |
|--------|-------------|
| `a[7:0]` | First 8-bit input |
| `b[7:0]` | Second 8-bit input |
| `ctrl` | Operation-selection control signal |
| `result[7:0]` | Result of the selected operation |
| `flags[5:0]` | Status flags generated from the latest operation |

The input `b` is not required for unary operations such as `NOT`, shift left, and shift right.
