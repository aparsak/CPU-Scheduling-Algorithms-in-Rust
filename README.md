# CPU Scheduling Simulator in Rust

This repository contains a **CPU Scheduling Simulator** implemented in **Rust**. It features implementations of three fundamental CPU scheduling algorithms, which are essential in operating systems to manage the execution of processes on a CPU.

## 📝 Overview

This repository provides Rust implementations of the following CPU scheduling algorithms:

- **First-Come, First-Served (FCFS)**
- **Shortest Remaining Job First (SRJF)**
- **Round Robin (RR)**

Each algorithm is designed to showcase the core principles of CPU scheduling, with implementations that are easy to understand and extend. You can input different scenarios and see how each algorithm schedules processes, providing valuable insights into their performance and efficiency.


## ⚙️ Algorithms

### 1. First-Come, First-Served (FCFS)
The **FCFS** algorithm is the simplest form of CPU scheduling. In this approach, the process that arrives first gets executed first. It is a non-preemptive scheduling algorithm, meaning that once a process starts its execution, it runs to completion.

### 2. Shortest Remaining Job First (SRJF)
**SRJF** is a preemptive version of the Shortest Job First (SJF) algorithm. It selects the process with the smallest amount of time remaining until completion. If a new process arrives with a shorter remaining time than the current process, the CPU switches to the new process. This algorithm minimizes the average waiting time but can lead to process starvation if shorter processes keep arriving.

### 3. Round Robin (RR)
**Round Robin** is a preemptive scheduling algorithm where each process is assigned a fixed time slot, known as a quantum. If a process does not complete within its time slot, it is placed at the end of the queue, and the CPU moves on to the next process.

## 📂 Input File Format

The input for these algorithms is provided through an `input.txt` file. The file should contain information about each task, formatted as follows:

- **pid**: A unique identifier for the process.
- **arrival_time**: The time at which the process arrives in milliseconds.
- **burst_time**: The time required by the process on the CPU in milliseconds.

An example `input.txt` might look like this:

| PID | Arrival Time | Burst Time |
|-----|--------------|------------|
|  1  |      0       |     4      |
|  2  |      1       |     5      |
|  3  |      2       |     2      |
|  4  |      3       |     1      |
|  5  |      4       |     3      |
|  6  |      5       |     4      |


## 📊 Statistical Output

At the end of the simulation, the program calculates and prints out statistical information, which includes:

1. **Average Waiting Time**: The average time a task spends waiting in the queue before it starts execution.
2. **Average Turnaround Time**: The average total time taken for a task to complete, from the moment it arrives until it finishes execution.

You can verify the results generated by the simulator with the online tool at [CPU Scheduling Simulator](https://cpu-scheduling-sim.netlify.app/).


## 🚀 Getting Started

### Prerequisites

Before running the simulator, ensure you have [Rust](https://www.rust-lang.org/tools/install) installed on your machine.

## 📞 Contact
For any inquiries or issues, please open an issue on this repository or reach out to aparsa.khadem@gamil.com.
