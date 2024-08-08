##Parallel File Encryptor/Decryptor in C++ (Using Multi Processing)
###Overview
This C++ project is a command-line utility that allows for the parallel encryption and decryption of files using a variety of encryption algorithms. It leverages the Semaphore synchronization primitive, multiprocessing, and fork system calls to distribute the workload across multiple CPU cores for maximum efficiency.
Features

Parallel processing to maximize CPU utilization
Progress reporting during long-running operations
Configurable block size and number of worker processes
Supports both encryption and decryption operations

Requirements

C++17 or newer

Clone the repository:

Copygit clone https://github.com/Suraj-Dhankad2025/parallel-file-encryptor.git



-i, --input: Input file path
-o, --output: Output file path
-a, --algorithm: Encryption algorithm 
-d, --decrypt: Perform decryption 
-p, --processes: Number of worker processes 

Implementation Details
The project uses the following OS concepts and techniques:

Semaphore: A Semaphore is used to control the number of worker processes that can access the file I/O operations simultaneously. This helps to prevent race conditions and ensure data integrity.
Multiprocessing: The project uses the fork() system call to create worker processes that perform the actual encryption/decryption tasks in parallel. This allows the program to take advantage of all available CPU cores.
File I/O: The program uses low-level file I/O operations (e.g., open(), read(), write()) to read and write data to the input and output files.
Encryption algorithms: The program supports three different encryption algorithms: AES, Blowfish, and Salsa20. The appropriate algorithm is selected based on the user's input.
Progress reporting: The program periodically reports the progress of the encryption/decryption operation to the user, providing information such as the percentage of the file processed and the estimated time remaining.

Contributing
Contributions are welcome! If you find any issues or have ideas for improvements, please open an issue or submit a pull request.
License
This project is licensed under the MIT License.
