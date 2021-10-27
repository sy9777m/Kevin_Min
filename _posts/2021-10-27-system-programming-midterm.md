---
toc: true
layout: post
description: Soongsil University 2-2 System Programming midterm.
categories: [markdown]
title: System Programming midterm
---
# System Programming midterm

## Abstraction is good but don't forget reality

Abstraction have limits

-   Especially in the presence of bugs
-   Need to understand details of underlying implementations

Useful outcomes from taking system programming

-   Able to find and eliminate bugs efficiently
-   Able to understand and tune for program performance

## Ints are not integers, Floats are not reals

![image-20211027041921386](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027041921386.png)

![image-20211027041925730](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027041925730.png)

## Computer arithmetic

Does not generate random values

Cannot assume all usual mathematical properties

-   Due to finiteness of representations
-   Integer operations satisfy 'ring' properties
    -   Commutativity, associativity, distributivity
-   Floating point operations satisfy 'ordering' properties
    -   Monotonicity, values of signs

Important issues for compiler writers and serious application programmers.

## You've got to know assembly

Understanding assembly is key to machine-level execution model

-   Behavior of programs in presence of bugs
    -   High-level language models break down
-   Tuning program performance
    -   Understand optimizations done / not done by the compiler
    -   Understanding sources of program inefficiency
-   Implementing system software
    -   Compiler has machine code as target
    -   Operating systems must manage process state

## Memory matters - Random Access Memory is an unphysical abstraction

Memory is not unbounded

-   It must be allocated and managed
-   Many applications are memory dominated

Memory referencing bugs especially pernicious

-   Effects are distant in both time and space

Memory performance is not uniform

-   Cache and virtual memory effects can greatly affect program performance
-   Adapting program to characteristics of memory system can lead to major speed improvements

![image-20211027042541071](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027042541071.png)

![image-20211027042551119](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027042551119.png)

## Memory referencing errors

-   C and C++ do not provide any memory protection
    -   out of bounds array refences
    -   Invalid pointer values
    -   Abuses of malloc / free
-   Can lead to nasty bugs
    -   Whether or not bug has any affect depends on system and compiler
    -   Action at a distance
        -   Corrupted object logically unrelated to one being accessed
        -   Effect of bug may be first observed long after it is generated

## There's more to performance than asymptotic complexity

Constant factors matter too

And even exact op count does not predict performance

-   Easily see 10:1 performance range depending on how code written
-   Must optimize at multiple levels - algorithm, data representations, procedures, and loops

Must understand system to optimize performance

-   how programs compiled and executed
-   how to measure program performance and identify bottlenecks
-   how to improve performance without destroying code modularity and generality

![image-20211027042938550](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027042938550.png)

Hierarchical memory organization

Performance depends on access patterns

-   Including how step through multi-dimensional array

## Computers do more than execute programs

They need to get data in and out

-   I/O system critical to program reliability and performance

They communicate with each other over networks

-   Many system-level issues arise in presence of network
    -   Concurrent operations by autonomous processes
    -   Coping with unreliable media
    -   Cross platform compatibility
    -   Complex performance issues

## Everything is bits

Each bits is 0 or 1

By encoding / interpreting sets of bits in various ways

Why bits? - Electronic implementation

-   Easy to store with bistable elements
-   Reliability transmitted on noisy and inaccurate wires

## Encoding byte values

Byte = 8 bits

### Example data representations

![image-20211027043303747](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027043303747.png)

## Boolean algebra

Algebraic representation of logic

-   Encode true as 1 and false as 0

![image-20211027043347856](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027043347856.png)

### General boolean algebras

Operate on bit vectors

-   Operations applied bitwise

![image-20211027043430808](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027043430808.png)

All of the properties of boolean algebra apply

![image-20211027043452466](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027043452466.png)

![image-20211027044238795](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027044238795.png)

## Bit-level operations in C

![image-20211027044259735](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027044259735.png)

![image-20211027044309599](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027044309599.png)

## Contrast: Logic operations in C

![image-20211027044328800](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027044328800.png)

![image-20211027044336152](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027044336152.png)

## Shift operations

![image-20211027044421381](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027044421381.png)

## Integers

### Encoding integers

![image-20211027044701071](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027044701071.png)

![image-20211027044716057](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027044716057.png)

![image-20211027044757931](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027044757931.png)

### Numeric ranges

![image-20211027044826093](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027044826093.png)

### Values for different word sizes

![image-20211027044913286](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027044913286.png)

### Unsigned & signed numeric values

Equivalence

-   same encodings for nonnegative values

Uniqueness

-   Every bit pattern represents unique integer value
-   Each representable integer has unique bit encoding

Can inverting mappings

![image-20211027045039055](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027045039055.png)

![image-20211027045044999](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027045044999.png)

## Mapping between signed & unsigned

![image-20211027045107523](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027045107523.png)

Mappings between unsigned and two's complement numbers: Keep bit representations and reinterpret

![image-20211027045221125](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027045221125.png)

![image-20211027045230990](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027045230990.png)

### Relation between signed & unsigned

![image-20211027045250508](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027045250508.png)

![image-20211027045308052](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027045308052.png)

### Signed vs. unsigned in C

Constants

-   By default are considered to be signed integers
-   Unsigned if have "U" as suffix
-   ![image-20211027045337350](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027045337350.png)

Casting

-   Explicit casting between signed & unsigned same as U2T and T2U

![image-20211027045359829](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027045359829.png)

-   Implicit casting also occurs via assignment and procedure calls

![image-20211027045429660](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027045429660.png)

### Casting surprises

Expression evaluation

-   If there is a mix of unsigned and signed in single expression, signed values implicitly cast to unsigned
-   Including comparison operations

![image-20211027045512058](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027045512058.png)

### Casting signed <-> unsigned: basic rules

-   Bit pattern is maintained
-   but reinterpreted
-   can have unexpected effects: adding or subtracting $2^{w}$
-   Expression containing signed and unsigned int
    -   `int` is cast to `unsigned`!!

### Sign extension

Task

-   Given w-bit signed integer x
-   Convert it to w + k-bit integer with same value

![image-20211027045810403](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027045810403.png)

![image-20211027045831561](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027045831561.png)

-   Converting from smaller to larger integer data type
-   C automatically performs sign extension

#### Expanding (short int to int)

-   Unsigned: zeros added
-   Signed: sign extension
-   Both yield expected result

#### Truncating (unsigned to unsigned short)

-   Unsigned / signed: bits are truncated
-   Result reinterpreted
-   Unsigned: mod operation
-   Signed: similar to mod
-   For small numbers yield expected behavior

### Unsigned addition

![image-20211027050155034](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050155034.png)

Standard addition function

-   ignores carry output

Implementations modular arithmetic

![image-20211027050240445](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050240445.png)

![image-20211027050335775](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050335775.png)

![image-20211027050350882](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050350882.png)

### Two-complement addition

![image-20211027050417014](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050417014.png)

![image-20211027050425030](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050425030.png)

![image-20211027050435241](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050435241.png)

![image-20211027050459580](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050459580.png)

### Multiplication

![image-20211027050529807](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050529807.png)

Maintaining exact results

-   would need to keep expanding word size with each product computed
-   is done in software, if needed

![image-20211027050615217](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050615217.png)

![image-20211027050623133](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050623133.png)

![image-20211027050636927](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050636927.png)

![image-20211027050645206](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050645206.png)

### Power-of-2 multiply with shift

![image-20211027050706187](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050706187.png)

![image-20211027050710469](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050710469.png)

![image-20211027050743532](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050743532.png)

![image-20211027050810877](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027050810877.png)

### Arithmetic: Basic rules

#### Addition:

-   Unsigned / signed: normal addition followed by truncate, same operation on bit level
-   Unsigned - addition mode $2^{w}$
    -   Mathematical addition + possible subtraction of $2^{w}$
-   Signed - modified addition mode $2^{w}$ (result in proper range)
    -   Mathematical addition + possible addition or subtraction of $2^{w}$

#### Multiplication:

-   Unsigned / signed: normal multiplication followed by truncate, same operation on bit level
-   Unsigned - multiplication mod $2^{w}$
-   Signed - modified multiplication mod $2^{w}$ (result in proper range)

### Why should I use unsigned?

![image-20211027051210460](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027051210460.png)

![image-20211027051241526](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027051241526.png)

![image-20211027051258484](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027051258484.png)

## Representations in memory, pointers, strings

### Byte-oriented memory organization

![image-20211027051332281](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027051332281.png)

Programs refer to data by address

-   Conceptually, envision it as a very large array of bytes
-   An address is like an index into that array
    -   and, a pointer variable stores an address

System provides private address spaces to each 'process'

-   Think of a process as a program being executed
-   So, a program can clobber its own data, but not that of others

### Machine words

Any given computer has a 'word size'

-   Nominal size of integer-valued data and of addresses
-   Until recently, most machines used 32 bits (4 bytes) as word size
    -   Limits addresses to 4GB
-   Increasingly, machines have 64-bit word size
    -   Potentially, could have 18EB (exabytes) of addressable memory
-   Machines still support multiple data formats
    -   Fractions or multiples of word size
    -   Always integral number of bytes

### Word-oriented memory organization

![image-20211027065818406](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027065818406.png)

Addresses specify byte locations

-   Address of first byte in word
-   Addresses of successive words differ by 4 (32-bit) or 8 (64-bit)

![image-20211027065857259](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027065857259.png)

### Byte ordering

Conventions

![image-20211027065913492](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027065913492.png)

![image-20211027065921688](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027065921688.png)

![image-20211027065953283](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027065953283.png)

![image-20211027070043111](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027070043111.png)

![image-20211027070050642](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027070050642.png)

![image-20211027070102449](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027070102449.png)

### Representing Strings

Strings in C

-   Represented by array of characters
-   Each character encoded in ASCII format
    -   Standard 7-bit encoding of character set
-   String should be null-terminated
    -   Final character = 0

Compatibility

-   Byte ordering not an issue

![image-20211027070247413](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027070247413.png)

## Floating point

### Fractional binary numbers

![image-20211027070611400](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027070611400.png)

![image-20211027070656701](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027070656701.png)

### Representable numbers

![image-20211027070714526](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027070714526.png)

### IEEE Floating point

IEEE Standard 754

Driven by numerical concerns

-   Nice standards for rounding, overflow, underflow
-   Hard to make fast in hardware
    -   Numerical analysts predominated over hardware designers in defining standard

### Floating point representation

![image-20211027070845517](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027070845517.png)

![image-20211027070927661](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027070927661.png)

![image-20211027070937032](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027070937032.png)

### Normalized values

![image-20211027071101884](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027071101884.png)

![image-20211027072122233](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027072122233.png)

bias = 127

127을 기준으로 0과 255만 제외하고, 소수점 1칸을 움직이고 싶으면 Exp = 128, E = 128 - 172 = 1로 계산

### Denormalized values

![image-20211027072608278](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027072608278.png)

### Special values

![image-20211027072733402](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027072733402.png)

![image-20211027072953531](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027072953531.png)

### Distribution of values

![image-20211027073027716](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027073027716.png)

![image-20211027073048133](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027073048133.png)

### Special properties of the IEEE encoding

FP zero same as Integer zero

-   all bits = 0

Can (almost) use unsigned integer comparison

-   Must first compare sign bits
-   Must consider -0 = 0
-   NaNs problematic
-   -   Will be greater than any other values
    -   What should comparison yield?
-   Otherwise OK
    -   Denorm vs. normalized
    -   Normalized vs. infinity

### Floating point operations: basic idea

![image-20211027073309010](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027073309010.png)

Basic idea

-   First compute exact result
-   Make it fit into desired precision
    -   Possibly overflow if exponent too large
    -   Possibly round to fit into `frac`

### Rounding

![image-20211027073355639](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027073355639.png)

### Closer look at round-to-even

Default rounding mode

-   hard to get any other kind without dropping into assembly
-   All other are statistically biased
    -   Sum of set of positive numbers will consistently be over- or under-estimated

![image-20211027073540219](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027073540219.png)

### Rounding binary numbers

![image-20211027073643032](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027073643032.png)

### FP multiplication

![image-20211027073655642](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027073655642.png)

Fixing

-   If $M \geq 2$, shift M right, increment E
-   If E out of range, overflow
-   Round M to fit `frac` precision

Implementation

-   Biggest chore is multiplying significands

### Floating point addition

![image-20211027073824957](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027073824957.png)

![image-20211027073911945](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027073911945.png)

### Mathematical properties of FP add

![image-20211027073929110](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027073929110.png)

### Mathematical properties of FP mult

![image-20211027074040391](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027074040391.png)

### Abelian group

![image-20211027074127882](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027074127882.png)

### Floating point in C

`float` - single precision

`double` - double precision

Conversions / casting

-   Casting between `int, float`, and `double` changes bit representation.
-   `double / float` -> int
    -   Truncates fractional part
    -   like rounding toward zero
    -   not defined when out of range or NaN
-   `int -> double`
    -   exact conversion, as long as `int` has $\leq 53$ bit word size
-   `int -> float`
    -   will round according to rounding mode

### Floating point puzzles

![image-20211027074403219](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027074403219.png)

### Dynamic range (positive-only)

![image-20211027074710910](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027074710910.png)

## Intel x86 processors

Complex instruction set computer (CISC)

-   Many different instructions with many different formats
    -   but, only small subset encountered with Linux programs
-   Hard to match performance of Reduced Instruction Set Computers (RISC)
-   In terms of speed. Less so for low power.

Added features

-   Instructions to support multimedia operations
-   Instructions to enable more efficient conditional operations
-   Transition from 32 bits to 64 bits
-   More cores

## x86 clones: Advanced Micro Devices (AMD)

-   a little bit slow, a lot cheaper
-   Developed x86-64, their own extension to 64 bits

## Definitions

Architecture - (also ISA: Instruction Set Architecture) The parts of a processor design that one needs to understand or write assembly / machine code.

Microarchitecture - Implementation of the architecture

Code forms

-   Machine code - The byte-level programs that a processor executes
-   Assembly code - A text representation of machine code

## Assembly  / Machine code view

![image-20211027075257754](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027075257754.png)

Programmer-visible state

-   PC - Program counter
    -   address of next instruction
    -   called 'RIP'
-   Register file
    -   heavily used program data
-   Condition codes
    -   store status information about most recent arithmetic or logical operation
    -   used for conditional branching

Memory

-   Byte addressable array
-   Code and user data
-   Stack to support procedures

## Turning C into Object code

![image-20211027075420009](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027075420009.png)

### Compiling into assembly

![image-20211027075451716](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027075451716.png)

## Assembly characteristics: data types

'Integer' data of 1, 2, 4, or 8 bytes

-   Data values
-   Addresses (untyped pointers)

Floating point data of 4, 8, or 10 bytes

Code - byte sequences encoding series of instructions

No aggregate types such as arrays or structures

-   just contiguously allocated bytes in memory

## Assembly characteristics: Operations

perform arithmetic function on register or memory data

Transfer data between memory and register

-   Load data from memory into register
-   Store register data into memory

Transfer control

-   Unconditional jumps to / from procedures
-   conditional branches

## Object code

![image-20211027075819838](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027075819838.png)

## Machine instruction example

![image-20211027075907340](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027075907340.png)

## Disassembling object code

![image-20211027075952304](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027075952304.png)

Disassembler

`objdump -d sum`

-   useful tool for examining object code
-   Analyzes bit pattern of series of instructions
-   Produces approximate rendition of assembly code
-   Can be run on either a.out (complete executable) or .o file

### What can be disassembled?

![image-20211027080055315](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027080055315.png)

Anything that can be interpreted as executable code

Disassembler examines bytes and reconstructs assembly source

## x86-64 Integer Registers

![image-20211027080134896](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027080134896.png)

### Some history: IA32 registers

![image-20211027080157590](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027080157590.png)

## Moving data

`movq Source, Dest`

![image-20211027080222603](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027080222603.png)

### `movq` operand combinations

![image-20211027080309631](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027080309631.png)

## Simple memory addressing modes

![image-20211027080353954](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027080353954.png)

![image-20211027080408919](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027080408919.png)

![image-20211027080425212](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027080425212.png)

![image-20211027080602119](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027080602119.png)

![image-20211027080610058](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027080610058.png)

![image-20211027080617652](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027080617652.png)

![image-20211027080625400](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027080625400.png)

![image-20211027080630845](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027080630845.png)

## Complete memory addressing modes

![image-20211027080653122](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027080653122.png)

![image-20211027094428952](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027094428952.png)

## Address computation instruction

`leaq Src, Dst`

-   `Src` is address mode expression
-   Set `Dst` to address denoted by expression

Use

-   Computing addresses without a memory reference
-   Computing arithmetic expressions of the from $x + k * y$

![image-20211027094541160](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027094541160.png)

## Some arithmetic operations

![image-20211027094629212](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027094629212.png)

![image-20211027094634269](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027094634269.png)

![image-20211027094704377](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027094704377.png)

![image-20211027094735037](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027094735037.png)

## Processor State (x86-64, Partial)

![image-20211027094916448](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027094916448.png)

## Condition codes (implicit setting)

![image-20211027094954382](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027094954382.png)

![image-20211027095002281](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027095002281.png)

Not set by `leaq` instruction

### Explicit setting: Compare

![image-20211027095056556](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027095056556.png)

### Explicit setting: test

![image-20211027095130320](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027095130320.png)

## Reading condition codes

SetX Instructions

-   Set low-order bytes of destination to 0 or 1 based on combinations of condition codes
-   Does not alter remaining 7 bytes

![image-20211027095226154](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027095226154.png)

![image-20211027095236908](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027095236908.png)

SetX Instructions - set single byte based on combination of condition codes

One of addressable byte registers

-   Does not alter remaining bytes
-   Typically use `movzbl` to finish job
    -   32-bit instructions also set upper 32 bits to 0

![image-20211027095339037](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027095339037.png)

## Jumping

jX instructions - Jump to different part of code depending on condition codes

![image-20211027095421739](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027095421739.png)

## Conditional branch example (old style)

![image-20211027095444228](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027095444228.png)

## Expressing with Goto code

![image-20211027100123443](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027100123443.png)

## General conditional expression translation (using branches)

![image-20211027100213983](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027100213983.png)

## Using conditional moves

![image-20211027100234307](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027100234307.png)

Conditional move instructions

-   Instruction supports: `if (Test) Dest <- Src`
-   Supported in post-1995 x86 processors
-   GCC tries to use them
    -   But, only when known to be safe

Why?

-   Branches are very disruptive instruction flow through pipelines
-   Conditional moves do not require control transfer

## Conditional move example

![image-20211027100428875](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027100428875.png)

## Bad cases for conditional move

### Expensive computations

`val  = Test(x) ? Hardl(x) : Hard2(x);`

-   both values get computed
-   Only makes sense when computations are very simple

### Risky computations

`val = p ? *p : 0;`

-   Both values get computed
-   May have undesirable effects

### Computations with side effects

`val = x > 0 ? x *= 7 : x += 3`

-   Both values get computed
-   Must be side-effect free

## Do-while loop example

![image-20211027100719400](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027100719400.png)

## Do-while loop compilation

![image-20211027100753177](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027100753177.png)

## General do-while translation

![image-20211027100829385](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027100829385.png)

### General while translation #1

![image-20211027100846135](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027100846135.png)

## While loop example

![image-20211027100917193](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027100917193.png)

![image-20211027100933135](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027100933135.png)

![image-20211027100942738](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027100942738.png)

## For loop form

![image-20211027101053616](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027101053616.png)

## For loop -> while loop

![image-20211027101110082](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027101110082.png)

## For-while conversion

![image-20211027101123580](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027101123580.png)

## For loop do-while conversion

![image-20211027101136420](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027101136420.png)

## Switch statement example

![image-20211027101209574](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027101209574.png)

## Jump table structure

![image-20211027101222818](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027101222818.png)

## Switch statement example

![image-20211027101241191](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027101241191.png)

![image-20211027101324338](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027101324338.png)

## Assembly setup explanation

Table structure

-   each target requires 8 bytes
-   base address at `.L4`

Jumping

-   Direct: `jmp .L8`
-   Jump target is denoted by label `.L8`
-   Indirect: `jmp *.L4(, %rdi, 8)`
-   Start of jump table: `.L4`
-   Must scale by factor of 8 (addresses are 8 bytes)
-   Fetch target from effective address `.L4 + x * 8`
    -   only for $0 \leq x \leq 6$

## Jump table

![image-20211027101557124](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027101557124.png)

### Code blocks (`x == 1`)

![image-20211027101656175](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027101656175.png)

### handling fall-through

![image-20211027101728790](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027101728790.png)

### Code blocks (`x == 2, x == 3`)

![image-20211027101744257](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027101744257.png)

### Code blocks (`x == 5, x == 6, default`)

![image-20211027101831338](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027101831338.png)

## Mechanisms in procedures

passing control

-   To beginning of procedure code
-   back to return point

Passing data

-   Procedure arguments
-   return value

Memory management

-   allocate during procedure execution
-   deallocate upon return

Mechanisms all implemented with machine instructions

x86-64 implementation of a procedure uses only those mechanisms required

## x86-64 stack

![image-20211027103417450](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027103417450.png)

region of memory managed with stack discipline

grows toward lower addresses

register `%rsp` constains lowest stack address

-   address of 'top' element

### x86-64 stack: push

`pushq src`

-   Fetch operand at src
-   Decrement `%rsp` by 8
-   Write operand address given by `%rsp`

![image-20211027103538821](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027103538821.png)

### x86-64 stack: pop

`popq dest`

-   Read value at address given by `%rsp`
-   increment `%rsp` by 8
-   store value at dest (must be register)

![image-20211027103627936](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027103627936.png)

## Code example

![image-20211027103644808](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027103644808.png)

## Procedure control flow

use stack to support procedure call and return

procedure call: `call label`

-   push return address on stack
-   jump to label

return address:

-   address of the next instruction right after call
-   example from disassembly

Procedure return: `ret`

-   pop address from stack
-   jump to address

![image-20211027103755978](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027103755978.png)

![image-20211027103818672](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027103818672.png)

![image-20211027103905789](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027103905789.png)

![image-20211027103916325](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027103916325.png)

## Procedure data flow

![image-20211027103941719](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027103941719.png)

### data flow examples

![image-20211027104001697](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104001697.png)

## Stack-based languages

languages that support recursion

-   code must be 'reentrant'
    -   multiple simultaneous instantiations of single procedure
-   need some place to store state of each instantiation
    -   arguments
    -   local variables
    -   return pointer

stack discipline

-   state for given procedure needed for limited time
    -   from when called to when return
-   callee returns before caller does

stack allocated in frames

-   state for single procedure instantiation

## call chain example

![image-20211027104207381](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104207381.png)

## Stack frame

contents

-   return information
-   local storage (if needed)
-   temporary space (if needed)

management

-   space allocated when enter procedure
    -   set-up code
    -   includes push by `call` instruction
-   deallocated when return
    -   finish code
    -   includes pop by `ret` instruction

![image-20211027104310318](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104310318.png)

### Example

![image-20211027104326446](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104326446.png)

![image-20211027104338914](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104338914.png)

![image-20211027104347201](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104347201.png)

![image-20211027104353955](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104353955.png)

![image-20211027104402833](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104402833.png)

![image-20211027104411997](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104411997.png)

![image-20211027104418160](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104418160.png)

![image-20211027104426472](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104426472.png)

![image-20211027104433206](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104433206.png)

![image-20211027104439712](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104439712.png)

![image-20211027104445710](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104445710.png)

## x86-64 / Linux stack frame

![image-20211027104501895](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104501895.png)

Current stack frame ('top' to bottom)

-   'argument build': parameters for function about to call
-   local variables if can't keep in registers
-   saved register context
-   old frame pointer (optional)

Caller stack frame

-   return address
    -   pushed by `call` instruction
-   arguments for this call

## Example: `incr`

![image-20211027104623434](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027104623434.png)

![image-20211027110105442](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110105442.png)

![image-20211027110122509](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110122509.png)

![image-20211027110132835](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110132835.png)

![image-20211027110152468](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110152468.png)

![image-20211027110204358](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110204358.png)

## Register saving conventions

when procedure `yoo` calls `who`:

-   `yoo` is the caller
-   `who` is the callee

Can register be used for temporary storage?

![image-20211027110246294](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110246294.png)

Conventions

-   'caller saved'
    -   caller saves temporary values in its frame before the call
-   'callee saved'
    -   callee saved temporary values in its frame before using
    -   callee restores them before returning to caller

## x86-64 Linux register usage

![image-20211027110355861](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110355861.png)

![image-20211027110528349](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110528349.png)

## Callee-saved example

![image-20211027110556071](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110556071.png)

![image-20211027110607046](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110607046.png)

## Recursion function

![image-20211027110622761](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110622761.png)

![image-20211027110734013](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110734013.png)

![image-20211027110745359](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110745359.png)

![image-20211027110755966](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110755966.png)

![image-20211027110804783](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110804783.png)

![image-20211027110812682](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110812682.png)

![image-20211027110825578](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027110825578.png)

## Observations about recursion

Handled without special consideration

-   stack frames mean that each function call has private storage

    -   saved registers & local variables
    -   saved return pointer

-   Register saving conventions prevent one function call from corrupting another's data

    -   Unless the C code explicitly does so - buffer overflow

-   Stack discipline follows call / return pattern

    -   If P calls Q, then Q returns before P
    -   Last-In, First-Out

    Also works for mutual recursion

    -   P calls Q; Q calls P

## x86-64 Procedure summary

![image-20211027111057784](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027111057784.png)

## Array allocation

Basic principle

`T A[L];`

-   array of data type T and length L
-   contiguously allocated region of L * `sizeof(T)` bytes in memory

![image-20211027111236807](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027111236807.png)

## Array access

![image-20211027111258042](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027111258042.png)

## Array example

![image-20211027111335888](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027111335888.png)

![image-20211027111354692](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027111354692.png)

![image-20211027111434013](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027111434013.png)

## Multidimensional (nested) arrays

![image-20211027111455485](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027111455485.png)

### Nested array example

![image-20211027111514213](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027111514213.png)

![image-20211027111536834](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027111536834.png)

![image-20211027111549363](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027111549363.png)

![image-20211027111731205](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027111731205.png)

![image-20211027111806092](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027111806092.png)

![image-20211027111924809](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027111924809.png)

![image-20211027111945470](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027111945470.png)

![image-20211027112047282](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027112047282.png)

## N * N Matrix code

![image-20211027112137346](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027112137346.png)

### 16 * 16 matrix access

![image-20211027113556133](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027113556133.png)

### n * n matrix access

![image-20211027113609441](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027113609441.png)

## Structure representation

![image-20211027113624871](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027113624871.png)

Structure represented as block of memory

-   big enough to hold all of the fields

Fields ordered according to declaration

-   Even if another ordering could yield a more compact representation

Compiler determines over size + positions of fields

-   Machine-level program has no understanding of the structures in the source code

## Generating pointer to structure member

![image-20211027113744195](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027113744195.png)

## Flowwing linked list

![image-20211027113801438](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027113801438.png)

## Structures & alignment

![image-20211027113814816](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027113814816.png)

## Alignment priciples

Aligned data

-   primitive data type requires K bytes
-   Addres must be multiple of k
-   required on some machines; advised on x86-64

Motivtaion for aligning data

-   memory accessed by (alinged) chunks of 4 or 8 bytes (system dependent)
    -   inefficient to load or store datum that spans quad word boundaries
    -   virtual memory trickier when datum spans 2 pages

Compiler

-   inserts gaps in structure to ensure correct alignment of fields

## Specific cases of alignment (x86-64)

![image-20211027114001119](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114001119.png)

## Satisfying alignment with structures

![image-20211027114045668](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114045668.png)

## Meeting overall alignment requirement

![image-20211027114106542](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114106542.png)

## arrays of structures

![image-20211027114123050](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114123050.png)

## Accessing array elements

![image-20211027114141994](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114141994.png)

## Saving space

![image-20211027114318223](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114318223.png)

## x86-64 Linux Memory layout

![image-20211027114335708](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114335708.png)

### x86-64 example addresses

![image-20211027114406947](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114406947.png)

![image-20211027114414171](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114414171.png)

## Memory referencing bug example

![image-20211027114458228](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114458228.png)

![image-20211027114508272](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114508272.png)

## Such problems are a BIG deal

generally called a 'buffer overflow'

-   When exceeding the memory size allocated for an array

Why a big deal?

-   It's the #1 technical cause of security vulnerabilities
    -   #1 overall cause is social enginerring / user ignorance

Most common form

-   Unchecked lengths on string inputs
-   Particularly for bounded character arrays on the stack
    -   sometimes referred to as stack smashing

## String library code

![image-20211027114642824](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114642824.png)

## Vulnerable buffer code

![image-20211027114659698](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114659698.png)

## Buffer overflow disassembly

![image-20211027114714186](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114714186.png)

## Buffer overflow stack

![image-20211027114727477](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114727477.png)

![image-20211027114738072](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114738072.png)

![image-20211027114749245](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114749245.png)

![image-20211027114800681](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114800681.png)

![image-20211027114815004](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027114815004.png)

![image-20211027115817640](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027115817640.png)

## Code injection attacks

![image-20211027115849482](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027115849482.png)

## Exploits based on buffer overflows

Buffer overflow bug can allow remote machines to execute arbitrary code on victim machines

Distressingly common in real programs

## What to do about buffer overflow attacks

-   avoid overflow vulnerabilities
-   employ system-level protections
-   have compiler use 'stack canaries'

### Avoid overflow vulnerabilities in code

![image-20211027120039759](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027120039759.png)

![image-20211027120046526](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027120046526.png)

### System-level protections can help

![image-20211027120103535](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027120103535.png)

![image-20211027120129353](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027120129353.png)

## Stack canaries can help

![image-20211027120251913](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027120251913.png)

## Protected buffer disassembly

![image-20211027120327882](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027120327882.png)

## Setting up canary

![image-20211027120342746](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027120342746.png)

## Checking canary

![image-20211027120357226](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027120357226.png)

## Return-oriented programming attacks

Challenge (for hackers)

-   stack randomization makes it hard to predict buffer location
-   marking stack nonexecutable makes it hard to insert binary code

Alternative strategy

-   use existing code
-   string together fragments to achieve oeverall desired outcome
-   does not overcome stack canaries

Construct program from gadgets

-   sequence of instructions ending in `ret`
    -   Encoded by single byte `0xc3`
-   code positions fixed from run to run
-   code is executable

### Gadget example

![image-20211027120609710](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027120609710.png)

![image-20211027120623663](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027120623663.png)

## ROP execution

![image-20211027120726700](/Kevin_Min/images/2021-10-27-system-programming-midterm/image-20211027120726700.png)

