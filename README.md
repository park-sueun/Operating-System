# Operating System, 2021 Spring Homework2 - PCTEST

## Overview
PCTEST is a tool for evaluating students' programming assignments. Run both the target program (student's submission) and the solution program (the correct program), then compare the results to ensure that the target program returns the correct results.

## Instructions for Building and Running

Users can use **Makefile** to build programs without much effort.
```
$ make pctest
$ ./pctest -i <testdir> -t <timeout> <solution> <target>
```
> testdir: The user provides the path to the directory where the test input files are stored in <testdir>.<br />
> timeout: Specify the program execution time limit (in seconds). Range: *1 < timeout < 10* <br />
> solution and target: Provide the correct version of the source code file name and the source code file name of the student program being tested, respectively. <br />
  
> $ make all : Compile the pctest.c file and create an executable file <pctest>. <br />
> $ make pctest : This command works the same as make all.<br />
> $ make clean : Not only pctest, but also built by running pctest, created solution and target executable files are also removed.<br />

## Video Demo
The video demo includes a review of the pctest program code.<br />
In addition, it covers the main scenarios of pctest through execution to ensure that the program meets the requirements.<br />

YouTube Link : https://www.youtube.com/


## Workflow

##### Step 1
Check that the test set directory exists for testing the program and validate the execution timeout.
##### Step 2
Given the source code files, pctest uses the compiler to build two executables each.
##### Step 3
Run the two executable files. At this time, the text of the test file is passed as an argument of the executable file.
##### Step 4
Determines whether the execution result of the input target is correct by checking that pctest exits successfully and the text generated to standard output is the same as the text generated by the solution.
##### Step 5
When all the given tests are executed, print out the test results.


## Solution Program

> Baekjoon: Word Count<br />
> https://www.acmicpc.net/problem/1152

