# Description
This project is part of a university assignment for the course on Assembly Languages. The project implements the SHA-256 (Secure Hash Algorithm 256-bit) cryptographic hashing function in both C# (high-level) and x64 Assembly (low-level), with the goal of creating a 64-bit application that supports multi-threading and performs efficient data processing using SIMD (Single Instruction, Multiple Data) instructions. SHA-256 generates a unique 256-bit hash for any given input data, widely used in cryptography for data validation, digital signatures, and cryptocurrency applications.

# Key Features:
## Two Equivalent Libraries:
- A high-level implementation in C#
- A low-level implementation in x64 Assembly
## Graphical User Interface (GUI): Built using WPF, the application provides a user-friendly interface with the following features:
- Input data selection
- Thread count adjustment (1-64 threads)
- Option to choose which library to use for generating the output (C# or ASM x64)
- Performance measurement for each method
- Output file generation
## Multi-threading: The application supports multi-threading by distributing pre-generated input files (created using a Python script) across the selected number of threads. The number of threads defaults to the number of logical processors available on the system.
## Performance Optimization: The application uses SIMD instructions to optimize the performance of both libraries. The program measures the execution time (averaged from 5 runs) for each method, allowing users to compare the efficiency of C# and Assembly implementations.
## Supported Thread Counts: The program allows users to select from 1, 2, 4, 8, 16, 32, or 64 threads for parallel execution.
# Requirements:
## 64-bit Application: Fully functional on 64-bit systems
## Technologies Used:
- C# for high-level library
- x64 Assembly for low-level library
- WPF for GUI development
- Python for generating large test datasets
- Multi-threading with a flexible number of threads, auto-detected based on the number of logical processors
## Performance Metrics: Measurement of time for hashing operations with high accuracy in proper units
## Data Sets: Three large predefined sets of data for benchmarking
## SIMD Instructions: Efficient use of vectorized operations to improve performance
## Version Control: The project is managed in a version control system
