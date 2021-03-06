---
layout: post
title: 1) Embedded Systems
date:  2018-12-06 07:05:00 +0900
categories:
- Engineering - ARM
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---
Processor: CPU - ALU(Arithmetic and Logic Unit), CU(Control Unit), Register and Internal Bus

<center>-1. Architecture of Processor</center>

- Register The Temporal Device of memory that saves the data temporarily in processor - General Purpose Register - Control Register(Program Counter)- Status Register(Expresses the status of processor): Physically structured with the Latches and Flip-Flop
- ALU(Arithmetic and Logic Unit): Arithmetic, Logic, Compliment, and Shift Operation- Status Register or Flag Register(Expresses the status caused by the result of operation)- It also represents the results of operations (occurrence of a 'carry' and 'overflow'.
- CU(Control Unit): Controls the data flow between each devices in the processor which is needed to read and execute the command. - Instruction Register (Temporarily memorizes the instructions which was read from the position of main memory devices that is designated by the PC[Program Counter])- Instruction Decoder (Decodes the instructions recorded in the instruction register)- Control Signal Generator (Execute the instructions according to the control signal generated from the instruction decoder)

<center>-2. Kind of Processor</center>

- I386: Processor which is same to the PC used by the developers, has been used so long time because of easy construction of developing IDE(Integral Developing Environment). By this continuous usage, it has a stability.
- ARM: It's instructions are simple, and electricity consumption is very low. So, it has been used in individual portable terminal such as a cell-phone and smart-phone since the end of 1990's.
- MIPS
- PowerPC
- M68K

<center>-3. Program and Instructions</center>

- Assembly Language - Features
- Easier comprehension than machine Language
- Easier modifying the errors and preserving than machine language
- Have to figure out the internal structure of processor and hardware.
- Each Processor has different assembly language syntax.

- OP Code(Operation Code)
  - Operand Ex) SUB A, B, C



<center>-4. Process</center>

- Read the instructions of the main memory device into the processor to conduct the command. PC (Program Counter) has the memory address of instructions to be executed. First, Contents of PC would be transferred to address register to take the instructions in the main memory, which is referred by the PC. By this, the instructions in the main memory would be preserved in the IR (Instruction Register). This Process is said to 'FETCH'.
- Control Unit interprets the instructions in IR, and send the appropriate control signal into ALU, Memory, etc. This process is said to 'DECODE'.
- Execute the instructions. In this time, these actions are performed with respect to such instruction - if the instruction is
- ALU instruction, AL operation is performed in ALU and save the result into nominated register.
- Conditional Branch Instruction, change the contents in PC in condition of satisfied branch condition.
- Unconditional Branch Instruction, change the contents in PC.
- Memory Reference Instruction, Send the address of memory which needs to be referenced into the data address register. After that, read the contents of the memory into the data input register to save it the nominated register by the instruction.

<center>-5. Instructions and structure of processor</center>

- CISC(Complex Instruction Set Computer) Structure
- RISC(Reduced Instruction Set Computer) Structure

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/4.PNG)

<center>Fig. 1 - Description of Fetching, decoding and executing</center>

- Reference
  - ARM으로 배우는 임베디드 리눅스 시스템 - 한빛미디어, 개정판, 안효복 지음
