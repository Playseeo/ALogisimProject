# Brief Introduction
This is a personal simple logisim project supports 11 instructions of RISC-V for ysyx("一生一芯") F Stage made by playseeo with AI-verification(deepseek) based on logisim v4.0.0 and opened RISC-V Instruction set.
(The Instruction File:unpriv-isa-asciidoc.pdf)

# Supported Instruction
Here is the instruction set:
ADD,ADDI,SUB,LUI,LW,SW,LBU,SB,JALR,BNE,BEQ
(The figure is provided in InstructionSet.png,and you can find it in the mentioned pdf before.)

# Project Structure:
A PC to the Instruction-ROM to decode to RegisterFile(actually here is usable register) to ALU to Data-RAM unit(include 4RAM which is 16 BitWidth address and 32 Data bit Width) to RAMInfoDealer to writeback to RF or output in RGB video.

(For 0x20000000 to 0x20040000 is the range of RGB video region and you can change it with my two subtractors.)