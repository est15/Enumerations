# Tools for Reverse Engineering && Debugging
# Linux
## Strace
Trouble shooting tool for tracing system calls. [Strace Man Page](https://linux.die.net/man/1/strace)

Basic Use Example:
```bash
strace <binary-file>
```
## Ltrace
Trouble shooting tool for displaying library calls during execution. [Ltrace Man Page](https://linux.die.net/man/1/ltrace)

Basic Use Example:
```bash
ltrace <binary-file>
```
## radare2
Collection of libraries, tools, and plugins to assist with reverse engineering. 
* [Radare2 GitHub](https://github.com/radareorg/radare2)
* [R2-Cheatsheet PDF](https://github.com/zxgio/r2-cheatsheet/blob/master/r2-cheatsheet.pdf)
* [R2-Wiki Cheatsheet](https://r2wiki.readthedocs.io/en/latest/home/misc/cheatsheet/)

### Access Binary File:
```bash
r2 ./golfer --> read only
r2 -w ./gofer --> write mode
```

### Get r2 Command Help
```bash
<r2-cli-command>?
```

### R2 CLI Commands
```bash
pd <n>   --> n = number of opcodes or leave it blank & print everything
w        --> write to the current offset
oo+      --> change to write-mode
```

## EDB-Debugger
GUI x86/x86-64 Debugger (used for OSCP BufferOverFlows) [EDB-Debugger](https://www.kali.org/tools/edb-debugger/)


# Windows
## Immunity Debugger
