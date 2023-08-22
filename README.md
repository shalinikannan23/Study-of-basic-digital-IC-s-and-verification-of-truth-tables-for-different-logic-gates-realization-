## EX 01 STUDY-OF-BASIC-DIGITAL-IC-S-AND-VERIFICATION-OF-TRUTH-TABLES-FOR-DIFFERENT-LOGIC-GATES-REALIZATION
### AIM:
To study about the different digital logic gates and to verify the truth table in Quartus for the basic logic gates using Verilog programming.
### Equipments Required:
Hardware – PCs, Cyclone II , USB flasher
Software – Quartus prime
Theory
## Introduction
Logic gates are the basic building blocks of any digital system. Logic gates are electronic circuits having one or more than one input and only one output. The relationship between the input and the output is based on a certain logic. Based on this, logic gates are named as
AND gate
OR gate
NOT gate
NAND gate
NOR gate
Ex-OR gate
Ex-NOR gate
1) AND gate
The AND gate is an electronic circuit that gives a high output (1) only if all its inputs are high. A dot (.) is used to show the AND operation i.e. A.B or can be written as AB
Y= A.B
2) OR gate
The OR gate is an electronic circuit that gives a high output (1) if one or more of its inputs are high. A plus (+) is used to show the OR operation.
Y= A+B
3) NOT gate
The NOT gate is an electronic circuit that produces an inverted version of the input at its output. It is also known as an inverter. If the input variable is A, the inverted output is known as NOT A. This is also shown as A' or A with a bar over the top, as shown at the outputs.
Y= A'
4) NAND gate
This is a NOT-AND gate which is equal to an AND gate followed by a NOT gate. The outputs of all NAND gates are high if any of the inputs are low. The symbol is an AND gate with a small circle on the output. The small circle represents inversion.
Y= (AB)’
5) NOR gate
This is a NOT-OR gate which is equal to an OR gate followed by a NOT gate. The outputs of all NOR gates are low if any of the inputs are high. The symbol is an OR gate with a small circle on the output. The small circle represents inversion.
Y= (A+B)’
6) Ex-OR gate
The 'Exclusive-OR' gate is a circuit which will give a high output if either, but not both of its two inputs are high. An encircled plus sign (⊕) is used to show the Ex-OR operation.
Y= A⊕B
7) Ex-NOR gate
The 'Exclusive-NOR' gate circuit does the opposite to the EX-OR gate. It will give a low output if either, but not both of its two inputs are high. The symbol is an EX-OR gate with a small circle on the output. The small circle represents inversion.
Y= A⊕B
### Procedure:
1)Create a New Project:Open Quartus and create a new project by selecting "File" > "New Project Wizard."Follow the wizard's instructions to set up your project, including specifying the project name, location, and target device (FPGA).
2)Create a New Design File:
    1. Once the project is created, right-click on the project name in the Project Navigator and select "Add New File."
    2. Choose "Verilog HDL File" or "VHDL File," depending on your chosen hardware description language.
3)Write the Combinational Logic Code:
    1. Open the newly created Verilog or VHDL file and write the code for your combinational logic.
4)Compile the Project:
    1.To compile the project, click on "Processing" > "Start Compilation" in the menu.
    2. Quartus will analyze your code, synthesize it into a netlist, and perform optimizations based on your target FPGA device.    
5)Analyze and Fix Errors:
    1. If there are any errors or warnings during the compilation process, Quartus will display them in the Messages window.
    2.Review and fix any issues in your code if necessary.
    3.View the RTL diagram.    
6)Verification:
   1. Click on "File" > "New" > "Verification/Debugging Files" > "University Program VWF".
   2.Once Waveform is created Right Click on the Input/Output Panel > " Insert Node or Bus" > Click on Node Finder > Click On "List" > Select All.
   3.Give the Input Combinations according to the Truth Table amd then simulate the Output Waveform.
### Program:
Program to verify the truth table in quartus for the basic logic gates using Verilog programming.
```
Developed by: SHALINI.K
RegisterNumber:  212222240095
module Ex1(a,b,yand,yor,ynot,yxor,ynand,ynor,yxnor);
input a,b;
output yand,yor,ynot,yxor,ynand,ynor,yxnor;
and (yand,a,b);
or (yor,a,b);
not (ynot,a);
xor (yxor,a,b);
nand (ynand,a,b);
nor (ynor,a,b);
xnor (yxnor,a,b);
endmodule
```
 ### Logic symbol & Truthtable:
 ![table](https://github.com/shalinikannan23/Study-of-basic-digital-IC-s-and-verification-of-truth-tables-for-different-logic-gates-realization-/assets/118656529/78e8b293-09fd-43e1-ad64-506ffb98802f)
![1](https://github.com/shalinikannan23/Study-of-basic-digital-IC-s-and-verification-of-truth-tables-for-different-logic-gates-realization-/assets/118656529/b8395052-5d73-48a7-bab1-cd457ee4d32b)
### Output:
![3](https://github.com/shalinikannan23/Study-of-basic-digital-IC-s-and-verification-of-truth-tables-for-different-logic-gates-realization-/assets/118656529/352598ba-dbea-4c1a-ba9b-ccdbcddb067b)
### Result:
Thus the different digital logic gates are studied and the truth table for different logic gates are verified.
