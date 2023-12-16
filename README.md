# OSProjectE
This project focuses on building multitasking capabilities into the existing  OS. 

Here's a summary of the implemented steps in the project:

Timer Interrupt: makeTimerInterrupt triggers scheduler every few ms.

Process Table: Tracks 8 processes with processActive, processStackPointer, and currentProcess.

Modified executeProgram: Loads programs, finds free segments and sets process table entries.

Scheduling: Selects active processes in a cycle within handleTimerInterrupt.

killProcess and interrupt 0x21: Allows termination of specific processes.

Process Blocking: Processes can wait for others using processWaitingOn and interrupt 0x21 calls.

Shell commands
		
	  type - To output contents of a file
		
	  exec - To execute a program
		
	  execb - To execute a program in the background
		
	  kill - To kill a process that's running
		
	  create - To create and enter contents to a file)
		
	  del - to delete a file
		
	  copy - to copy a file

By accomplishing these steps,  transformed the OS into capable of running multiple programs simultaneously and managing their execution through scheduling and termination mechanisms.

compileOS.sh file consists of several commands. By complying compileOS.sh, it will handle the compiling and assembling of the OS into a disc image. Upon which you can use the diskc.img to run it in a simulator
