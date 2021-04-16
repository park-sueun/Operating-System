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


## Solution Program

> Baekjoon: Word Count<br />
> https://www.acmicpc.net/problem/1152

