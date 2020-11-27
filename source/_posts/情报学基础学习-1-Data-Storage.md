---
title: 情报学基础学习-1.Data Storage
date: 2020-11-25 15:57:31
tags: [CS, 一般入试, EN, ZN]
categories: 勉強力
index_img: /img/index/CS.png
---
# 1.1 Bits and Their Storage
**Bits**: 0s and 1s
## Boolean Operation 
There are 3 kinds of boolean operations.
- AND: A AND B is True, A is True and B is True
- OR: A OR B is True, At least one of A and B is True
- XOR: A XOR B is True, either A or B but not both

## Gates and Flip-Flop
### Gates:
- AND:
- OR:
- XOR:
- NOT:

### Flip-flop 
A device to store a bit, constructed of gates.
## Hexadecimal Notation 十六进制记数法
Stream：A long string of bits (0s and 1s)
Hard to read and comprehend. So we need a new shorthand notation to simplify the representation of the string, which is ***Hexadecimal Notation***.
- Takes advantage of the fact that bit patterns within a machine tend to have lengths in multiples of four.
- Represent Table 
    - TODO:

# 1.2 Main Memory
A computer store a large number collection of ***circuits***(such as flip-flops), each storing a **single bit** .This bit reservoir is known as the machine’s ***main memory***.
## Memory Organization
### Cells
Main memory is organized in manageable units called cells. A typical cell size being **eight bits** which is one **byte**.
- **high-order end**, or the most significant bit is the **left** end of the row (which is a memory cell).
    如果这个cell被表示为数字，则这个MSB代表了这个cell最重要的内容，数字的正负，1代表正，0代表负。
- **low-order end**,  or the least significant bit is the **right** end of the row (which is a memory cell).
    如果这个cell被表示为数字，则这个LSB代表了这个cell最不重要的内容，指示数字很小的变化。

### Address
A unique “name" assign to a cell. The Address system not only gives us a way of uniquely **identifying** each cell but also associates **an order** to the cells. Which means there are "the next cell" and "the previous cell".
- which means you can store bit patterns that may be longer than the length of a single cell. 
    For example, we can still store a string of 16 bits merely by using two consecutive memory cells.
- Read operation: get data from the memory by asking for the content of the address.
- Write operation: record information in the memory by requesting that a certain bit pattern be placed in the cell at a particular address.

### RAM (Random Access Memory)
The main memory has the ability to access cells in any order.
Constructed using **not** flip-flop, but more complex technologies that provide greater miniaturization and faster response time. 
- **DRAM**: dynamic memory.
- **SDRAM**: synchronous DRAM, decrease the time needed to retrieve the contents from its memory cells.

## Measuring Memory Capacity
进位1024: bit, KB, MB, GB, TB.

# 1.3 Mass Memory
Additional memory devices including magnetic disks, CDs, DVDs, magnetic tapes, flash drives, and solid-state disks(SSD).
- **Pros**: less volatility, large storage capacities, low cost, and in many cases, the ability to remove the storage medium from the machine for archival purposes.
- **Cons**: require mechanical motion and therefore require significantly more time to store and retrieve data than a machine’s main memory. Storage systems with moving parts are more prone to mechanical failures than solid state systems.

## Magnetic Systems
TODO
## Optical Systems
TODO
## Flash Drives
TODO

# 1.4 Representing Information as Bit Patterns
## Representing Text
TODO:

## Representing Numeric Values
TODO:

## Representing Images
TODO:

## Representing Sound
TODO:

# 1.5 The Binary System
## Binary Notation
TODO:

## Binary Addition
TODO:

## Fractions in Binary
TODO: