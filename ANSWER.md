Q - List all of the main states a process may be in at any point in time on a standard Unix system. Briefly explain what each of these states mean.

Q - What is a Zombie Process? How does it get created? How does it get destroyed?

A - It is a process that has completed execution but still has an entry in the process table, it is a process in the "Terminated state". A child that terminates, but has not been waited for becomes a "zombie". kill the parent process of the zombie. At that point, all of the parent’s children will be adopted by the init process (pid 1), which periodically runs wait() to reap any zombie children.

Q - Describe the job of the Scheduler in the OS in general.

A -  Is the process of allocating system resources to many different tasks by an operating system.

Q - Describe the benefits of the MLFQ over a plain Round-Robin scheduler.

A - A process that waits too long in a lower priority queue may be moved to a higher priority queue.
