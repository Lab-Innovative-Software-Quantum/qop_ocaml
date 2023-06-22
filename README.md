# qop_ocaml
An Ocaml library for quantum computing operations

## Operations
- Pauli-X/Y/Z
- Identity
- CNOT
- Hadamard
- Measurement

## How to use the library

### Download and include
The only dependency used by the library is [Owl](https://github.com/owlbarn/owl).

Once the dependency is installed, simply move the files to your lib directory and use `open Qop`.

### Use
Every function takes as input a single list of complex numbers (the quantum state) and one (or two, for the CNOT) integers that refer to the index of the qubit that has to be taken as the input of the operation. The output is always a list of complex numbers.

The measurement takes as input a complext list and a list of integers (the indexes of the qubit to measure) and returns a list or tuples `complex list * int * float`, with the new quantum state, the integer result of the measurement and the probability of having that result.