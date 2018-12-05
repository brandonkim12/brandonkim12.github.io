---
layout: post
title: 1) Embedded Systems
date:  2018-12-06 07:05:00 +0900
categories:
- Engineering - ARM
feature_image: https://www.facebook.com/photo.php?fbid=1893189787425704&set=a.1893187554092594&type=3&theater
---
Processor: CPU - ALU(Arithmetic and Logic Unit), CU(Control Unit), Register and Internal Bus

1. Architecture of Processor

    a. Register The Temporal Device of memory that saves the data temporarily in processor - General Purpose Register - Control Register(Program Counter)- Status Register(Expresses the status of processor): Physically structured with the Latches and Flip-Flop
    b. ALU(Arithmetic and Logic Unit): Arithmetic, Logic, Compliment, and Shift Operation- Status Register or Flag Register(Expresses the status caused by the result of operation)- It also represents the results of operations (occurrence of a 'carry' and 'overflow')
    c. CU(Control Unit): Controls the data flow between each devices in the processor which is needed to read and execute the command. - Instruction Register (Temporarily memorizes the instructions which was read from the position of main memory devices that is designated by the PC[Program Counter])- Instruction Decoder (Decodes the instructions recorded in the instruction register)- Control Signal Generator (Execute the instructions according to the control signal generated from the instruction decoder)

2. Kind of Processor
    a. I386: Processor which is same to the PC used by the developers, has been used so long time because of easy construction of developing IDE(Integral Developing Environment). By this continuous usage, it has a stability.
    b. ARM: It's instructions are simple, and electricity consumption is very low. So, it has been used in individual portable terminal such as a cell-phone and smart-phone since the end of 1990's.
    c. MIPS
    d. PowerPC
    e. M68K

3. Program and Instructions

    1. Assembly Language - Features
        1. Easier comprehension than machine Language
        2. Easier modifying the errors and preserving than machine language
        3. Have to figure out the internal structure of processor and hardware.
        4. Each Processor has different assembly language syntax.
            1. OP Code(Operation Code)
            2. Operand Ex) SUB A, B, C

4. Read the instructions of the main memory device into the processor to conduct the command. PC (Program Counter) has the memory address of instructions to be executed. First, Contents of PC would be transferred to address register to take the instructions in the main memory, which is referred by the PC. By this, the instructions in the main memory would be preserved in the IR (Instruction Register). This Process is said to 'FETCH'.

5. Control Unit interprets the instructions in IR, and send the appropriate control signal into ALU, Memory, etc. This process is said to 'DECODE'.

6. Execute the instructions. In this time, these actions are performed with respect to such instruction - if the instruction is

​    ​   1) ALU instruction, AL operation is performed in ALU and save the result into nominated register.

​       2) Conditional Branch Instruction, change the contents in PC in condition of satisfied branch condition.

​       3) Unconditional Branch Instruction, change the contents in PC.

​       4) Memory Reference Instruction, Send the address of memory which needs to be referenced into the data address register. After that, read the contents of the memory into the data input register to save it the nominated register by the instruction.

- Instructions and structure of processor
  - CISC(Complex Instruction Set Computer) Structure
  - RISC(Reduced Instruction Set Computer) Structure

![useful image](https://raw.githubusercontent.com/brandonkim12/brandonkim12.github.io/master/assets/4.PNG)

<center>Fig. 1 - Description of Fetching, decoding and executing</center>

- Reference
  - ARM으로 배우는 임베디드 리눅스 시스템 - 한빛미디어, 개정판, 안효복 지음

