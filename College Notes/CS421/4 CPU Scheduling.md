CPUs are very "bursty"
	As in they do a lot of things at once then has a bit of a "cooldown" period

Dispatcher
	Dispatcher module gives control of the CPU to the process selected by the short-term scheduler.
	This involves
		Switching context
		Switching to user mode
		Jumping to the proper location in the user program to restart the program
	Dispatch latency
		Time it takes for the dispatcher to stop one process and start another running

CPU Utilization - Keep the CPU as busy as possible
Throughput - Number of processes that complete theri execution per time unit
Turnaround Time - Amount of time to execute a particular process
Waiting time - Amount of time a process has been waiting in the ready queue
Response time - The time between the request and the action

