# Two-stage Assembler Project in ANSI-C

This project is a two-stage assembler written in ANSI-C. It translates assembly language source code into machine code.

## Overview

The assembler works in two stages:

1. **First Stage**: The first stage scans the input file and performs initial processing. This involves identifying labels, opcodes, and operands in the assembly language source code. It also handles directives such as data allocation and defines the symbol table.

2. **Second Stage**: The second stage uses the information gathered in the first stage to generate the machine code. It resolves addresses of labels and translates opcodes and operands into their binary form.

## Files in the Project

- **`assembler.c`**: This is the main entry point of the program. It orchestrates the two stages of the assembly process.

- **`firstStage.c` and `secondStage.c`**: These files implement the logic for the first and second stages of the assembler, respectively.

- **`tableMgmt.c`**: This file contains functions for managing the symbol table and other tables used in the assembly process.

- **`utils.c`**: This file contains utility functions used throughout the project.

- **`system.h`, `stages.h`, and `structs.h`**: These header files contain declarations for system-specific settings, stage-specific functions, and data structures used in the project, respectively.

## How to Run the Project

The project can be compiled using the `make` command. The executable file is named `assembler`. It can be run using the following command:

```bash
./assembler <input_file> <output_file>
```


Grade: 94