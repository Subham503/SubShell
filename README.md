# SubShell 🐚

A custom Unix shell built from scratch in C, running on Linux/WSL.

## Features
- Interactive prompt (REPL loop)
- Execute real Linux commands (`ls`, `pwd`, `echo`, `mkdir` etc.)
- Built-in `cd` command
- Argument parsing with `strtok()`
- Process management with `fork()`, `execvp()`, `wait()`

## How to Build & Run
```bash
gcc shell.c -o shell
./shell
```

## Usage
```
myshell> ls
myshell> pwd
myshell> echo Hello World
myshell> cd /home
myshell> exit
```

## What I Learned
- How shells work under the hood
- Linux system calls (`fork`, `exec`, `wait`, `chdir`)
- Process creation and management
- Input parsing in C

## Roadmap
- [ ] Pipes support (`ls | grep txt`)
- [ ] I/O Redirection (`echo hello > file.txt`)
- [ ] Command history (arrow keys)
- [ ] Custom prompt with current directory
- [ ] `~` expansion in paths

## Tech Stack
- Language: C
- Environment: Ubuntu 22.04 (WSL2)
- Compiler: GCC 11.4
