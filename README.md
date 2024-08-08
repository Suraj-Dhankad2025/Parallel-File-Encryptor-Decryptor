# Parallel File Encryptor/Decryptor in C++ (Using Multi Processing)

## Overview

This C++ project is a command-line utility that allows for the parallel encryption and decryption of files using a variety of encryption algorithms. It leverages the Semaphore synchronization primitive, multiprocessing, and fork system calls to distribute the workload across multiple CPU cores for maximum efficiency.

### Features

- Parallel processing to maximize CPU utilization
- Progress reporting during long-running operations
- Configurable block size and number of worker processes
- Supports both encryption and decryption operations

## Requirements

- C++17 or newer

### Clone the repository:

```bash
git clone https://github.com/Suraj-Dhankad2025/parallel-file-encryptor.git
