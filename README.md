# RISC-V Simualtor

Please refer to the design documentation for more details.

### Instruction Formats
	R-Type:
		ins rd rs1 rs2
	I-Type (Except jalr ):
		ins rd rs1 immed
	SB-Type:
		ins rs1 rs2 label
	S-Type:
		ins rs1 immed(rs2)
	U-Type:
		ins rs1 immed
	UJ-Type:
		jal rd label
	jalr:
		jalr rd immed(rs1)


## Instructions to setup GUI for Phase 3 (incorporates Phase 2 as well)
1.	Extract RISCVSim.tar.gz
2.	Run the install script
3.	Run the Risc-V simulator from the shortcut.


### Note: This install script is specific to Linux. For more details please refer to requirements.txt

##  Instructions to Use CLI
1.	Navigate to the directory containing the Makefile.
2.	Run the following command for executing the Phase 2 code (without Piplining):
		make p2 INP=path/to/the/file(without the asm extension)
3.	Run the following command for executing the Phase 3 Code (with Piplining):
		make p3 INP=path/to/file (without the asm extension)

Example: <br />
	make p2 INP=test
	
Example 2: <br />
	make p3 INP=bubble

Example 3: <br />
	make p3 INP=fib
#### Note: File needs to be in same directory as the Makefile
