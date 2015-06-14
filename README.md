# LogicBoard
This is a java console implementation of the LogicBoard project. 
It's purpose is for proof of concept. 
Once completed it will be implemented as an application using GUI. 
This project focuses on the data structure to handle creation,edits, and saves of a logicBoard project.
All source code has been designed and implemented by Kyle Ferguson (Singularity Systems). 
This is kind of a private project


Sample of Console
Output of Driver3:

A	B	C	D	E	F	|	(((A'+B)+CD)+E+F)'	
0	0	0	0	0	0			0						
0	0	0	0	0	1			0						
0	0	0	0	1	0			0						
0	0	0	0	1	1			0						
0	0	0	1	0	0			0						
0	0	0	1	0	1			0						
0	0	0	1	1	0			0						
0	0	0	1	1	1			0						
0	0	1	0	0	0			0						
0	0	1	0	0	1			0						
0	0	1	0	1	0			0						
0	0	1	0	1	1			0						
0	0	1	1	0	0			0						
0	0	1	1	0	1			0						
0	0	1	1	1	0			0						
0	0	1	1	1	1			0						
0	1	0	0	0	0			0						
0	1	0	0	0	1			0						
0	1	0	0	1	0			0						
0	1	0	0	1	1			0						
0	1	0	1	0	0			0						
0	1	0	1	0	1			0						
0	1	0	1	1	0			0						
0	1	0	1	1	1			0						
0	1	1	0	0	0			0						
0	1	1	0	0	1			0						
0	1	1	0	1	0			0						
0	1	1	0	1	1			0						
0	1	1	1	0	0			0						
0	1	1	1	0	1			0						
0	1	1	1	1	0			0						
0	1	1	1	1	1			0						
1	0	0	0	0	0			1						
1	0	0	0	0	1			0						
1	0	0	0	1	0			0						
1	0	0	0	1	1			0						
1	0	0	1	0	0			1						
1	0	0	1	0	1			0						
1	0	0	1	1	0			0						
1	0	0	1	1	1			0						
1	0	1	0	0	0			1						
1	0	1	0	0	1			0						
1	0	1	0	1	0			0						
1	0	1	0	1	1			0						
1	0	1	1	0	0			0						
1	0	1	1	0	1			0						
1	0	1	1	1	0			0						
1	0	1	1	1	1			0						
1	1	0	0	0	0			0						
1	1	0	0	0	1			0						
1	1	0	0	1	0			0						
1	1	0	0	1	1			0						
1	1	0	1	0	0			0						
1	1	0	1	0	1			0						
1	1	0	1	1	0			0						
1	1	0	1	1	1			0						
1	1	1	0	0	0			0						
1	1	1	0	0	1			0						
1	1	1	0	1	0			0						
1	1	1	0	1	1			0						
1	1	1	1	0	0			0						
1	1	1	1	0	1			0						
1	1	1	1	1	0			0						
1	1	1	1	1	1			0						
------------------------------------------------
Gate A: 
	outputTo: A'

Gate B: 
	outputTo: A'+B

Gate C: 
	outputTo: CD

Gate D: 
	outputTo: CD

Gate E: 
	outputTo: E+F

Gate F: 
	outputTo: E+F

Gate A': 
	input1: A
	outputTo: A'+B

Gate A'+B: 
	input1: A'
	input2: B
	outputTo: (A'+B)+CD

Gate CD: 
	input1: C
	input2: D
	outputTo: (A'+B)+CD

Gate E+F: 
	input1: E
	input2: F
	outputTo: ((A'+B)+CD)+E+F

Gate (A'+B)+CD: 
	input1: A'+B
	input2: CD
	outputTo: ((A'+B)+CD)+E+F

Gate ((A'+B)+CD)+E+F: 
	input1: (A'+B)+CD
	input2: E+F
	outputTo: (((A'+B)+CD)+E+F)'

Gate (((A'+B)+CD)+E+F)': 
	input1: ((A'+B)+CD)+E+F

------------------------------------------------

Process finished with exit code 0


