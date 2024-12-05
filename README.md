```
 _  ____  ____            ____  _     _     ____  _          
/ \/  _ \/  __\          / ___\/ \   / \ /\/  __\/ \__/|     
| || / \||  \/|  _____   |    \| |   | | |||  \/|| |\/||     
| || \_/||    /  \____\  \___ || |_/\| \_/||    /| |  ||     
\_/\____/\_/\_\          \____/\____/\____/\_/\_\\_/  \|     
 ____  _     _____  ____  _      ____  _____  _  ____  _     
/  _ \/ \ /\/__ __\/  _ \/ \__/|/  _ \/__ __\/ \/  _ \/ \  /|
| / \|| | ||  / \  | / \|| |\/||| / \|  / \  | || / \|| |\ ||
| |-||| \_/|  | |  | \_/|| |  ||| |-||  | |  | || \_/|| | \||
\_/ \|\____/  \_/  \____/\_/  \|\_/ \|  \_/  \_/\____/\_/  \|
                                                             
```

# Usage: IOR_Slurm_automation

IOR_Slurm_automation [-h] -n NLIST [-m TASKS_PER_NODE] [-j JOBNAME] [-i ITERATIONS] [-s SIZE] [-b BLOCK] [-d]

Automate IOR tests with SLURM.

## Options:

- **-h, --help**  
  Show this help message and exit.

- **-n NLIST, --nlist NLIST**  
  List of comma-separated hostnames (i.e. targeted nodes).

- **-m TASKS_PER_NODE, --tasks_per_node TASKS_PER_NODE**  
  Maximum number of tasks to be launched; default=`1`.

- **-j JOBNAME, --jobname JOBNAME**  
  Base name for the job (optional); default=`IOR_test`.

- **-i ITERATIONS, --iterations ITERATIONS**  
  Number of iterations per test (optional); default=`10`.

- **-s SIZE, --size SIZE**  
  Size of the test file in GB (optional); default=`128`.

- **-b BLOCK, --block BLOCK**  
  Blocksize in MB (optional); default=`16`.

- **-d, --delete**  
  Delete the temporary SLURM batch script after submission (optional); default=`FALSE`.