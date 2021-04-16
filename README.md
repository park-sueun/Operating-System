# Operating System, 2021 Spring Homework3 - PFIND

## Overview
PFIND is a text search program that finds all lines of a given keyword in all text files under a specific directory.

## Instructions for Building and Running

Users can use **Makefile** to build programs without much effort.
```
$ make pfind
$ ./pfind <dir> <keyword1> <keyword2>
```
> dir : The path of the directory where the search will be performed <br />
> keyword : A list of one or more keywords that are not empty <br />
  
> $ make pfind : Compile the pfind.c file and create an executable file <pfind>. <br />
> $ make clean : Remove the pfind executable. <br/>Also, if a named pipe remains unremoved due to an abnormal termination of the program, it will remove the named pipe.<br />

## Video Demo
pfind's presentation includes:<br />
1. A description of the program design, including the communication protocol between the manager and the worker process.<br />
2. Code review of program source code<br />
3. Implementation demonstration<br />

YouTube Link : 


## Limitations and Problems of Current Design
Currently implemented pfind does not meet the following requirements.<br />
1. Improper implementation for multi-process<br />
2. pfind works only for files under the current path<br />
3. Abnormal termination when entering <dir> as an absolute path<br />
4. No option provided for pfind<br />

## Future progress
I've been thinking a lot about how to design a multiprocess by creating multiple child processes as a single thread, but I haven't found a solution yet.<br />

The biggest reason I couldn't solve was that I couldn't figure out how to create multiple child processes and keep them up to a limited number. Also, when operating as multiple processes, we have not yet understood exactly how to prevent more than one process from entering or reading pipes at the same time.<br />

Even after the project deadline, we will continue to think and challenge ourselves to successfully complete the multi-process design.<br />


