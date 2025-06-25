# CPU Scheduling Algorithms

A C++ project that simulates major CPU scheduling algorithms with support for custom inputs and visual trace/stats output.

## Algorithms Implemented

- **First Come First Serve (FCFS)**
- **Round Robin (RR)** with configurable time quantum
- **Shortest Process Next (SPN)**
- **Shortest Remaining Time (SRT)**
- **Highest Response Ratio Next (HRRN)**
- **Feedback Scheduling (FB)** with fixed and varying time quantum
- **Aging** to prevent starvation

## Features

- Simulates scheduling with process arrival, burst time, and priorities
- Supports both preemptive and non-preemptive strategies
- Outputs scheduling stats or trace timelines

## Usage

1. Compile the project using:
   ```bash
   make
   ```
2. Run the executable and provide input as per the required format.

   ```
   Line 1: trace or stats  
   Line 2: Scheduling algorithms with optional parameters (e.g., 2-4 means Round Robin with quantum = 4)  
   Line 3: Last time unit for simulation  
   Line 4: Number of processes  
   Lines 5+: Process info  

   For algorithms 1–7:
   <ProcessName>,<ArrivalTime>,<ServiceTime>

   For algorithm 8 (Aging):
   <ProcessName>,<ArrivalTime>,<Priority>
   ```

## Example

```
stats
1,2-3,3
20
3
P1,0,5
P2,2,3
P3,4,1
```

## Tech Stack

- **Language**: C++
- **Build Tools**: Makefile, g++
- **Documentation**: Markdown
