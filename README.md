# 512-Bit-SRAM
Design of an 512-Bit SRAM using Cadence

## Requirement

The SRAM architecture is shown below,

<img src="Images/Architecture.PNG" width="500">

The SRAM had two main components.  
1. Sense Amplifier  

<img src="Images/Sense.PNG" width="200">

2. Write data path  

<img src="Images/write.PNG" width="200">  

One bit SRAM,

<img src="Images/ibsram.PNG" width="500">

PIN specification

<img src="Images/Specification.PNG" width="300">

---

## Approach
To achieve this, we started out by designing the smaller parts using metal 1. Metal 2 was used when designing the 128-bit SRAM cell.
To achieve the 512-bit design, we then connected four 128-bit SRAM cell using metal 3 to achieve the complete design.

## Layouts

Here are some of the important layouts of the design

1. Sense Amplifier

a. Cell  
<img src="Images/senseampcell_lay.JPG" width="500">

b. Unit

<img src="Images/senseamp_full_lay.JPG" width="500">

2. Write Circuit

a. Cell

<img src="Images/writeckt_lay.JPG" width="500">  

b. Unit  
<img src="Images/writeckt_full_lay.JPG" width="500">

3. Pre-charge circuit

<img src="Images/pre_ckt_cell_lay.JPG" width="500">

4. 6 transistor design of SRAM

<img src="Images/6T_layout.JPG" width="500">

5. Row decoder

<img src="Images/rowdecoder_lay.JPG" width="500">

6. Write multiplexer

<img src="Images/writemux_cell_layout.JPG" width="500">

7. Read Multiplexer

<img src="Images/readmuxcell_lay.JPG" width="500">

8. Register Bank select

<img src="Images/banksel_lay.JPG" width="500">

9. 512-Bit SRAM

a. Schematic

<img src="Images/sram_512kb_schem_with components.jpg" width="500">

b. Layout

<img src="Images/sram_bank_layout.JPG" width="500">

----

## Files

The files attached here contain a vector file with HSPICE code to simulate the design. Individual schematics of each cell and unit have 
also been attached. They can be found in the "Images" folder.
