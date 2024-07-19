# Process Scheduling and Memory Management Simulation

Project Overview
This project is a simulation of a process manager that handles process scheduling and memory management. The simulation focuses on a system where all processes are fully CPU-bound, meaning they have a single CPU burst and do no I/O operations. The process manager operates in cycles, where each cycle represents one quantum of time.

Features
Process Scheduling: Implements round-robin scheduling to allocate CPU time to processes.
Memory Management: Supports three memory management strategies:
Contiguous Memory Allocation
Paged Memory Allocation
Virtual Memory Allocation

Usage: allocate -f <filename> -m (infinite | first-fit | paged | virtual) -q (1 | 2 | 3)
-f filename will specify a valid relative or absolute path to the input file describing the processes. 
-m memory-strategy where memory-strategy is one of {infinite, first-fit, paged, virtual}.
-q quantum where quantum is one of {1, 2, 3}.

Example
./allocate -f processes.txt -m infinite -q 3.
