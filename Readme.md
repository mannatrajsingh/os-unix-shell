# Unix Shell from Scratch

A minimal Unix shell implemented in **C** using **POSIX system calls**, replicating core `bash` functionality such as process execution, background jobs, and signal handling.

---

## Features

- Command execution via `fork()` and `execvp()`
- Built-in commands: `cd`, `exit`, `jobs`
- Background execution using `&`
- Job tracking and management
- Signal handling (`Ctrl+C`, `Ctrl+Z`)
- Error handling for invalid commands

---

## Usage

### Build
```bash
make

Run
./myshell

Example
myshell> ls
myshell> cd ..
myshell> sleep 5 &
myshell> jobs
myshell> exit

Implementation Highlights

Process management with fork, execvp, and waitpid

Signal forwarding using signal and kill

Modular design with separate components for parsing, execution, jobs, and signals

Tech Stack

C · POSIX APIs · Unix/Linux

Author

Mannat Raj Singh
