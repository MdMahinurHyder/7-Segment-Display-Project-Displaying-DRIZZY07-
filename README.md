=====================================================
      7-SEGMENT ALPHANUMERIC DISPLAY: "drIZZY07"
=====================================================

Project Overview:
This project involves designing a combinational logic circuit 
that sequences through the characters "d", "r", "I", "Z", "Z", 
"Y", "0", and "7" on a common-anode/cathode 7-segment display 
based on 3-bit binary inputs (X, Y, Z).

-----------------------------------------------------
1. OBJECTIVES
-----------------------------------------------------
- Construct a Truth Table for the sequence "drIZZY07".
- Derive simplified logic equations using:
    * Sum of Minterms (SOM)
    * Product of Maxterms (POM)
    * Sum of Products (SOP) via K-Maps
- Perform cost analysis for hardware implementation.
- Design the circuit in Logisim.

-----------------------------------------------------
2. HARDWARE / COMPONENTS REQUIRED
-----------------------------------------------------
- 7-Segment Display
- IC 74LS138 (3 to 8 Line Decoder)
- IC 74LS153 (4 to 1 Multiplexer)
- IC 74LS04 (Hex Inverter/NOT Gate)
- IC 74LS08 (2-Input AND Gate)
- IC 74LS32 (2-Input OR Gate)
- IC 74LS10/11 (3-Input NAND/AND Gates)
- Breadboard & Jumper Wires
- Resistors (330 ohms)

-----------------------------------------------------
3. LOGIC SUMMARY
-----------------------------------------------------
The sequence is mapped to 3-bit inputs (000 to 111):
000 -> d | 001 -> r | 010 -> I | 011 -> Z
100 -> Z | 101 -> Y | 110 -> 0 | 111 -> 7

Key Equations (Sample SOP):
- A = yz + x(not z)
- B = X + Y + (not z)
- G = (not Y) + (not X)z

-----------------------------------------------------
4. COST ANALYSIS
-----------------------------------------------------
The project includes a detailed breakdown of costs for 
different implementation methods:
- SOM Implementation: ~280.48 TK
- POM Implementation: ~180.36 TK
- SOP Implementation: ~160.32 TK

-----------------------------------------------------
5. AUTHOR
-----------------------------------------------------
Md. Mahinur Hyder Antor
ID: 2412755642
