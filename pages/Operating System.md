- ## What is an OS? #card
  card-last-interval:: -1
  card-repeats:: 1
  card-ease-factor:: 2.5
  card-next-schedule:: 2022-05-17T18:30:00.000Z
  card-last-reviewed:: 2022-05-16T19:49:23.360Z
  card-last-score:: 1
	- An OS can be defined as the interface between user and hardware. #defination
	- It is responsible for the execution of all the processes. Resource allocation, CPU management, and file management.
	- The purpose of an operating system is to provide an environment in which the user can execute the programs in an efficient manner.
- ### Types of OS. {{cloze 5}} types
  collapsed:: true
	- Batch
		- A similar set of jobs are stored in the main memory for execution.
		- A job gets assigned to the CPU only when the previous job gets completed.
	- Multiprogramming
		- The main memory consists of jobs waiting for the CPU time.
		- The OS selects one process and assigns it to the CPU.
		- Whenever the executing process needs to wait for any other operations like input or output, then the OS selects another process from the job queue and assigns it to the CPU.
		- This way the CPU never gets idle. And the user gets the illusion of getting multiple jobs done at a time.
	- Multitasking
		- Multitasking OS combines the benefits of multiprogramming OS and CPU scheduling to perform quick switches between jobs.
		- The switch is so quick that the user can interact with each program as it runs.
	- Time Sharing
		- It requires interaction with the user to instruct the OS to perform various jobs.
		- The OS responds with an output.
		- The instructions are usually given with an input device like keyboard.
	- Real Time
		- Real time OS are built for dedicated systems to accomplish a specific set of tasks within deadline.
- ## Process
	- A Process is a program under execution.
	- The value of the program counter indicates the address of the next instruction of the process being executed.
	- Each process is represented by a process control block. (PCB)
- ## Thread
	-