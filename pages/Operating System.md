- ## What is an OS? #card
  card-last-interval:: 3.98
  card-repeats:: 2
  card-ease-factor:: 2.36
  card-next-schedule:: 2022-05-23T18:45:53.984Z
  card-last-reviewed:: 2022-05-19T19:45:53.984Z
  card-last-score:: 3
	- An OS can be defined as the interface between user and hardware. #defination
	- It is responsible for the execution of all the processes. Resource allocation, CPU management, and file management.
	- The purpose of an operating system is to provide an environment in which the user can execute the programs in an efficient manner.
- ### Types of OS. {{cloze 5}} types
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
  id:: 6283b412-e1db-46e4-af8d-4c9840be7f45
	- A Process is a program under execution.
	- The value of the program counter indicates the address of the next instruction of the process being executed.
	- Each process is represented by a process control block. (PCB)
	  id:: 6283b46b-eec4-4e4b-a7ec-5c26d7ae9a6b
- ## Thread
	- A thread is a lightweight process and forms the basic unit of CPU utilization.
	- A ((6283b412-e1db-46e4-af8d-4c9840be7f45)) can perform more than one task at the same time by including multiple threads.
	- A thread has its own program counter, register set, and stack
	- A thread shares resources with other threads of the same process: the code section, the data section, files and signals.
	- A new thread, or a child process of a given process, can be introduced by using the fork() system call. A process with n fork() system call generates 2^n – 1 child processes.
	- There are two types of threads
		- User threads (User threads are implemented by users)
		- Kernel threads (Kernel threads are implemented by OS)
- ## Scheduling Algorithms, {{cloze 8}} types.
	- Fairy smooched stupid roses, provides her much minerals #mnemonic
	- First Come First Serve (FCFS)
		- Simplest scheduling algorithm that schedules according to arrival times of processes.
	- Shortest Job First (SJF)
		- Processes which have the shortest burst time are scheduled first.
	- Shortest Remaining Time First (SRTF)
		- It is a preemptive mode of SJF algorithm in which jobs are scheduled according to the shortest remaining time.
	- Round Robin (RR) Scheduling
		- Each process is assigned a fixed time, in a cyclic way.
	- Priority Based scheduling (Non Preemptive)
		- In this scheduling, processes are scheduled according to their priorities, i.e., highest priority process is scheduled first. If priorities of two processes match, then scheduling is according to the arrival time.
	- Highest Response Ratio Next (HRRN)
		- In this scheduling, processes with the highest response ratio are scheduled. This algorithm avoids starvation.
		- Response Ratio = (Waiting Time + Burst time) / Burst time
	- Multilevel Queue Scheduling (MLQ)
		- According to the priority of the process, processes are placed in the different queues. Generally high priority processes are placed in the top level queue. Only after completion of processes from the top level queue, lower level queued processes are scheduled.
	- Multilevel Feedback Queue (MLFQ) Scheduling
		- It allows the process to move in between queues. The idea is to separate processes according to the characteristics of their CPU bursts. If a process uses too much CPU time, it is moved to a lower-priority queue.
- ## Critical Section Problem
	- The portion of the code in the program in which the shared variables are accessed and/or updated is known as {{cloze Critical Section}}
	- The remainder section is the portion of the code in the program excluding the critical section.
	- The final output of the code depends upon the order in which variables are accessed. It is known as {{cloze The Race Around Condition}}
	- ### A solution for the critical section problem must satisfy three conditions:
		- <ins>Mutual Exclusion</ins>If a process is executing in the critical section, then no other process should be allowed to enter in the critical section.
		- <ins>Progress</ins>If no process is executing in the critical section. Then the decision of a process to enter a critical section cannot be made by any other process that is executing in its remember section.
		- <ins>Bounded Waiting</ins>There exists a bound on the number of times other processes can enter into the critical section after a process has made a request to access the critical section and before the request is granted.
- ## MCQs
	- RAID stands for {{cloze Redundant Array of Independent Disks. It is used to store the same data redundantly to improve the overall performance. There are 7 RAID levels. }}
	- Fragmentation is the phenomena of {{cloze memory wastage. It reduces the capacity and performance because space is used inefficiently}}
		- Internal fragmentation. It occurs when we deal with the systems that have fixed size allocation units.
		- External fragmentation. It occurs when we deal with systems that have variable sized allocation units.
	- What is Spooling? {{cloze a process in which data is temporarily gathered to be used and executed by a device program or the system It is used with printing}}