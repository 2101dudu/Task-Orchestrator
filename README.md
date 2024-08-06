<h1 align="center">Sistemas Operativos<img align="center" src="https://github.com/devicons/devicon/blob/master/icons/c/c-original.svg" target="_blank" title="C" alt="C" width="30" height="30"/></h1>

<h3 align="center">Made using the C programming language during the 2st semester of the 2nd year</h3> 

<h1 align="center">Final Grade: 19/20💎</h1>

## About

A C-based server that executes bash commands from multiple concurrent clients made for our [SO](https://www.di.uminho.pt/~jno/sitedi/uc_J304N1.html) class.


## Features

- Server-to-client communication via named pipes
- Scalability via scheduling algorithms
- Multiple client requests
- Computation is all done on the server's side
- Great error handling 

## Preview
https://github.com/2101dudu/Task-Orchestrator/assets/115400010/d44d49d5-c628-4978-ad7e-897ae044c77e


## Usage
```bash
>>make

# on one terminal
>>bin/orchestrator output_folder parallel-tasks sched-policy(FCFS/SFJ) <"test-mode"> <number-test-tasks>

# on the other terminal
>>bin/client execute time(ms) -u "prog [args]"
>>bin/client execute time(ms) -p "prog-a [args]|prog-b [args]|prog-c [args]"
>>bin/client status
>>bin/client server-stop
```

## Final Notes

In this repo you will find the script "run.sh", which allows the request of any number of tasks you´d like, followed by the maximum sleep time, ranging from 1 to N. To better test the scheduler´s policy, it´s best to use ./orchestrator with "test-mode" enabled and provide the number of tasks the script will be executing.

### Example
```bash
>>make

# on one terminal
>>bin/orchestrator FOLDER 3 SFJ "test-mode" 20

# on the other terminal
>>./run.sh 20 5
```


## Group 1
The members of this group who contributed to this project were:
- <a href="https://www.github.com/Cerqueira025">Ana Cerqueira</a>
- <a href="https://www.github.com/2101dudu">Eduardo Faria</a>
- <a href="https://www.github.com/NunoMRS7">Nuno Silva</a>
