************************************************************************************************
					4 - bit ALS UNIT
************************************************************************************************
Inputs:
-------

A	- The first operand to perform the operation
B	- The second operand "	"	"	"
S3S2S1S0- Select bits to select operation to be performed (refer to the table given below)

Outputs:
--------

Output	- The standard output generated on performing the operation [Note: For shift operations,
	  arithmetic increment/decrement operations and logical NOT operation, only operand A
	  shall be considered]
Carry	- The carry output generated while performing arithmetic operations

Tables:
-------
__________________________________________________________
S3	S2	S1	S0	Operation Performed
__________________________________________________________
0	0	0	0	Addition of A and B
0	0	0	1	Subtraction of B from A
0	0	1	0	Increment A
0	0	1	1	Decrement A
0	1	0	0	AND Operation on A and B
0	1	0	1	OR Operation on A and B
0	1	1	0	XOR Operation on A and B
0	1	1	1	NOT Operation on A
1	0	0	0	Logical Shift right
1	0	0	1	Logical Shift left
1	0	1	0	Arithmetic Shift right
1	0	1	1	Arithmetic Shift left
1	1	0	0	Circular Shift right
1	1	0	1	Circular Shift left
1	1	1	0	  **NOT ASSIGNED**
1	1	1	1	  **NOT ASSIGNED**
