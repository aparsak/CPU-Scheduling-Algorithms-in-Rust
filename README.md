# CPU Scheduling Algorithms in Rust

This repository contains implementations of three fundamental CPU scheduling algorithms written in Rust. These algorithms are essential in operating systems to manage the execution of processes on a CPU.

## 📝 Overview

This repository provides Rust implementations of the following CPU scheduling algorithms:

- **First-Come, First-Served (FCFS)**
- **Shortest Remaining Job First (SRJF)**
- **Round Robin (RR)**

Each algorithm is designed to demonstrate the core principles of CPU scheduling, with implementations that are easy to understand and extend.

## ⚙️ Algorithms

### 1. First-Come, First-Served (FCFS)
The **FCFS** algorithm is the simplest form of CPU scheduling. In this approach, the process that arrives first gets executed first. It is a non-preemptive scheduling algorithm, meaning that once a process starts its execution, it runs to completion.

### 2. Shortest Remaining Job First (SRJF)
**SRJF** is a preemptive version of the Shortest Job First (SJF) algorithm. It selects the process with the smallest amount of time remaining until completion. If a new process arrives with a shorter remaining time than the current process, the CPU switches to the new process. This algorithm minimizes the average waiting time but can lead to process starvation if shorter processes keep arriving.

### 3. Round Robin (RR)
**Round Robin** is a preemptive scheduling algorithm where each process is assigned a fixed time slot, known as a quantum. If a process does not complete within its time slot, it is placed at the end of the queue, and the CPU moves on to the next process.

## 🚀 Getting Started

### Prerequisites

Before running the algorithms, ensure you have [Rust](https://www.rust-lang.org/tools/install) installed on your machine. 


## 📞 Contact
For any inquiries or issues, please open an issue on this repository or reach out to aparsa.khadem@gamil.com.

