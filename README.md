# CPU Scheduling Algorithms Simulator

This project implements various CPU Scheduling algorithms in C++:

- First Come First Serve (FCFS)
- Shortest Job First (SJF) - Non-Preemptive
- Shortest Job First (SJF) - Preemptive
- Priority Scheduling
- Round Robin Scheduling (with Time Quantum = 2 and 4)

## Features

- Accepts process information from user input (Arrival Time, Burst Time, Priority)
- Calculates Waiting Time (WT) and Turnaround Time (TAT)
- Displays tabular output for each algorithm
- Supports both preemptive and non-preemptive scheduling

## How to Compile and Run

Make sure you have `g++` installed.

```bash
g++ cpu_scheduling.cpp -o cpu_scheduling
./cpu_scheduling

## Sample Input and Output

**Input:**


