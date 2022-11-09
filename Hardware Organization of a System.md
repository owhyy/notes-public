# Hardware Organization of a System

#Programming

> How a #[[6f9l-computer]] is organized

- Buses - carry [[do9i-byte|bytes]] of information (_words_) to the other components
- I/O Devices - connect to the outer world
  - controllers are chips on the device itself
  - adapters are cards that plug into the motherboard
- Main [[ad6a-memory]] - temporarily stores data;
  - memory is a linear array of bytes
- [[37ve-processors|Processor]] - executes the instructions stored in main memory
  - the [[5tlm-registers|register]]/Program Count (PC) points at the address of some instruction in main memory
  - instruction is read -> operation is performed -> PC gets updated to point to next instruction
  - the Arithmetic Logic Unit (ALU) performs the operations

Execution of a program:

1. the characters `./hello` are read from the keyboard and stored into a register
2. when `ENTER` is pressed, the data in the `hello` executable is copied into main memory, from the disk. The data includes the `Hello, world!\n` string that will be printed
3. after they are loaded into direct memory, the instructions in the `hello`'s `main` function are executed, by copying the `Hello, world!\n` string **from direct memory to the PC**
4. the string is copied from the register to the display device
