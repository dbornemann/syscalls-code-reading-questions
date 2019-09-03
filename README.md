# syscalls-code-reading-questions

The goal of this assignment is to introduce you to the OS/161 code. You are already a bit familiar with OS/161 after  setting up your virtual machine and learning how to configure and build OS/161 kernels. OS/161 is a simplified skeleton of a modern operating system. It comes with a configurable build system, code for some useful user-level utilities that can be run from within OS/161, and of course code for the operating system itself. 

To complete the OS/161 assignments of this course, you will need to get your hands deep in the guts of the OS/161 codebase, and the sooner you become familiar with it, the better. To that end, you should look through the files and begin to learn how the code is structured, what goes where, and how things work. This applies both to the build system and the codebase itself.

To guide you in this process, please write up and hand in answers to the questions found below.  

Note: in these questions, and throughout the course of the semester, we will refer to the terms *trap*, *interrupt*, *exception*, and *system call*. Although these terms might take on different meanings in different classes, in OS/161, they mean the following:

- We use *trap* as a generic term of transferring control into the kernel.
- We use *exception* for events that are synchronous with respect to user processes and cause a trap into the kernel: these include things like divide-by-0 or NULL pointer dereference exceptions and the trap caused by the syscall instruction in MIPS.
- We use "interrupt" for asynchronous events that cause a trap into the kernel: this includes things like interrupts from the serial console hardware, the timer hardware, etc.
- We use "system call" for synchronous requests user processes make to request service from the OS: system calls are invoked using traps -- specifically using the syscall instruction on MIPS.










Example of how to add code to markdown text

```cpp
void *threadA ( void *ptr )
{
    printf("Statement A \n");
    fflush(stdout);
    pthread_exit(0); 
}
```
Example of how to add a figure to markdown text

![](Ubuntu_16.04_Desktop.png)

