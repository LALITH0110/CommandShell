# CommandShell

This project implements a simple Unix shell from scratch, designed to handle job control and support basic shell functionalities. The lab provided a practical way to learn about process management, signal handling, and interaction with the operating system.  

## Features

- **Job control**: Built-in support for running processes in the foreground and background, listing jobs, and managing job states.
- **Signal handling**: Graceful handling of `SIGINT` and `SIGTSTP` signals.
- **Trace-driven testing**: Verified against various scenarios using predefined trace files.

---

## Project Files

### Core Files

- `Makefile`: Automates the compilation of the shell program and runs tests to validate its functionality.  
- `README.md`: This file, detailing the project structure and functionality.  
- `tsh.c`: The main source file for the shell program.

---

### Testing and Utilities

- `sdriver.pl`: A trace-driven testing driver for the shell program.  
- `trace*.txt`: A set of 15 trace files designed to simulate and test various shell interactions.  
- `tsh.out`: Sample outputs from test runs.

---

### Helper Programs

- `myspin.c`: Spins for a user-defined number of seconds, simulating a long-running process.  
- `mysplit.c`: Forks a child process that spins for a user-defined number of seconds.  
- `mystop.c`: Spins for a user-defined number of seconds and then sends `SIGTSTP` to itself.  
- `myint.c`: Spins for a user-defined number of seconds and then sends `SIGINT` to itself.  

---

## How to Use

1. Clone this repository:
   ```bash
   git clone https://github.com/LALITH0110/CommandShell
   cd <repository-directory>
