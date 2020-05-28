# nand2tetris

Working my way through the [Nand to Tetris Course](https://www.nand2tetris.org/)

- Download the latest `nand2tetris.zip` from the book website, and overwrite everything in the `projects` and `tools` directory.
- Remember to run `chmod +X tools/*.sh` if you're on \*nix.

## [Project 1: Boolean Logic](https://www.nand2tetris.org/project01)

Build order as per the website. Cost for each gate in NAND in brackets.

- [x] `Nand` (primitive)
- [x] `Not` (1)
- [x] `Or` (3)
- [x] `Xor` (6, Can be improved)
- [x] `And` (2)
- [x] `Mux` (8, Took me ages. Can be improved)
- [x] `DMux` (5, Super Fun)
- [x] `Not16` (16)
- [x] `And16` (32)
- [x] `Or16` (48)
- [x] `Mux16` (113)
- [x] `Or8Way` (21)
- [x] `Mux4Way16` (339)
- [x] `Mux8Way16` (791)
- [x] `DMux4Way` (37, Fun)
- [x] `DMux8Way` (101)

## [Project 2: Boolean Arithmetic](https://www.nand2tetris.org/project02)

CHIPs/Gates used in brackets

- [x] `HalfAdder` (Xor+And)
- [x] `FullAdder` (2 HalfAdder, 1 Or)
- [x] `Add16` (1 HalfAdder, 15 FullAdder)
- [x] `Inc16` (1 Add16)
- [x] `ALU` (6 Mux16, 3 Not16, 1 Add16, 1 And16, 2 Or8Way, 2 Or, 1 Not)

## [Project 3: Memory](https://www.nand2tetris.org/project03)

Make sure you read through the [Hardware Simulator Tutorial][s] to understand the clock in the simulator.

- [x] `DFF` (primitive)
- [x] `Bit` (1 Mux, 1DFF)
- [x] `Register` (16 Bits)
- [x] `RAM8` (8 Registers, 1 DMux8Way, 1 Mux8Way16) = 8 registers
- [x] `RAM64` (8 RAM8, 1 DMux8Way, 1 Mux8Way16) = 64 registers
- [x] `RAM512` (8 RAM64, 1 DMux8Way, 1 Mux8Way16) = 512 registers
- [x] `RAM4K` (8 RAM512, 1 DMux8Way, 1 Mux8Way16) = 4096 registers
- [x] `RAM16K` (4 RAM4K, 1 DMux4Way, 1 Mux4Way16) = 16384 registers
- [x] `PC` (1 Register, 1 Inc16, 1 Or8Way, 1 Mux8Way16)

[s]: https://b1391bd6-da3d-477d-8c01-38cdf774495a.filesusr.com/ugd/44046b_bfd91435260748439493a60a8044ade6.pdf

## [Project 3: Machine Language Programming](https://www.nand2tetris.org/project03)

Counting number of instructions by `wc -l $file.hack`

- [x] Mult (18)
- [x] Fill (98)
