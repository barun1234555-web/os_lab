# Experiment 2 — Priority and Round Robin Scheduling Algorithms

**Subject:** Operating Systems Lab  |  **Roll no:** 25071A6245

## Priority Scheduling

**Aim:** Write a C program for priority scheduling algorithm A. Non-preemptive B. Preemptive

### A. Non-preemptive

**Source:** [`priority_non_preemptive.c`](priority_non_preemptive.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of processes: 3
Enter Arrival Time, Burst Time and Priority for P1: 0 10 3
Enter Arrival Time, Burst Time and Priority for P2: 1 1 1
Enter Arrival Time, Burst Time and Priority for P3: 2 2 2

Process AT      BT      Pr      CT      WT      TAT
P1      0       10      3       10      0       10
P2      1       1       1       11      9       10
P3      2       2       2       13      9       11

Average Waiting Time = 6.00
Average Turnaround Time = 10.33
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of processes: 4
Enter Arrival Time, Burst Time and Priority for P1: 0 11 2
Enter Arrival Time, Burst Time and Priority for P2: 1 3 1
Enter Arrival Time, Burst Time and Priority for P3: 2 5 4
Enter Arrival Time, Burst Time and Priority for P4: 3 2 3

Process AT      BT      Pr      CT      WT      TAT
P1      0       11      2       11      0       11
P2      1       3       1       14      10      13
P3      2       5       4       21      14      19
P4      3       2       3       16      11      13

Average Waiting Time = 8.75
Average Turnaround Time = 14.00
```

#### Test case 3

```text
Roll no: 25071A6245
Enter number of processes: 3
Enter Arrival Time, Burst Time and Priority for P1: 0 24 3
Enter Arrival Time, Burst Time and Priority for P2: 0 3 1
Enter Arrival Time, Burst Time and Priority for P3: 0 3 2

Process AT      BT      Pr      CT      WT      TAT
P1      0       24      3       30      6       30
P2      0       3       1       3       0       3
P3      0       3       2       6       3       6

Average Waiting Time = 3.00
Average Turnaround Time = 13.00
```

### B. Preemptive

**Source:** [`priority_preemptive.c`](priority_preemptive.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of processes: 3
Enter Arrival Time, Burst Time and Priority for P1: 0 7 3
Enter Arrival Time, Burst Time and Priority for P2: 1 4 1
Enter Arrival Time, Burst Time and Priority for P3: 2 1 2

Process AT      BT      Pr      CT      WT      TAT
P1      0       7       3       12      5       12
P2      1       4       1       5       0       4
P3      2       1       2       6       3       4

Average Waiting Time = 2.67
Average Turnaround Time = 6.67
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of processes: 4
Enter Arrival Time, Burst Time and Priority for P1: 0 10 3
Enter Arrival Time, Burst Time and Priority for P2: 1 1 1
Enter Arrival Time, Burst Time and Priority for P3: 2 2 4
Enter Arrival Time, Burst Time and Priority for P4: 3 1 2

Process AT      BT      Pr      CT      WT      TAT
P1      0       10      3       12      2       12
P2      1       1       1       2       0       1
P3      2       2       4       14      10      12
P4      3       1       2       4       0       1

Average Waiting Time = 3.00
Average Turnaround Time = 6.50
```

#### Test case 3

```text
Roll no: 25071A6245
Enter number of processes: 3
Enter Arrival Time, Burst Time and Priority for P1: 0 24 3
Enter Arrival Time, Burst Time and Priority for P2: 0 3 1
Enter Arrival Time, Burst Time and Priority for P3: 0 3 2

Process AT      BT      Pr      CT      WT      TAT
P1      0       24      3       30      6       30
P2      0       3       1       3       0       3
P3      0       3       2       6       3       6

Average Waiting Time = 3.00
Average Turnaround Time = 13.00
```

## Round Robin Scheduling

**Aim:** Write a C program for Round Robin scheduling algorithm A. Time Quantum=2, B. Time Quantum=10

### A. Time Quantum = 2

**Source:** [`round_robin_tq2.c`](round_robin_tq2.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of processes: 3
Enter Arrival Time and Burst Time for P1: 0 5
Enter Arrival Time and Burst Time for P2: 1 3
Enter Arrival Time and Burst Time for P3: 2 1

Process AT      BT      CT      WT      TAT
P1      0       5       9       4       9
P2      1       3       8       4       7
P3      2       1       5       2       3

Average Waiting Time = 3.33
Average Turnaround Time = 6.33
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of processes: 4
Enter Arrival Time and Burst Time for P1: 0 5
Enter Arrival Time and Burst Time for P2: 1 4
Enter Arrival Time and Burst Time for P3: 2 2
Enter Arrival Time and Burst Time for P4: 4 1

Process AT      BT      CT      WT      TAT
P1      0       5       12      7       12
P2      1       4       11      6       10
P3      2       2       6       2       4
P4      4       1       7       2       3

Average Waiting Time = 4.25
Average Turnaround Time = 7.25
```

#### Test case 3

```text
Roll no: 25071A6245
Enter number of processes: 3
Enter Arrival Time and Burst Time for P1: 0 24
Enter Arrival Time and Burst Time for P2: 0 3
Enter Arrival Time and Burst Time for P3: 0 3

Process AT      BT      CT      WT      TAT
P1      0       24      30      6       30
P2      0       3       9       6       9
P3      0       3       10      7       10

Average Waiting Time = 6.33
Average Turnaround Time = 16.33
```

### B. Time Quantum = 10

**Source:** [`round_robin_tq10.c`](round_robin_tq10.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of processes: 3
Enter Arrival Time and Burst Time for P1: 0 25
Enter Arrival Time and Burst Time for P2: 2 6
Enter Arrival Time and Burst Time for P3: 4 12

Process AT      BT      CT      WT      TAT
P1      0       25      43      18      43
P2      2       6       16      8       14
P3      4       12      38      22      34

Average Waiting Time = 16.00
Average Turnaround Time = 30.33
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of processes: 4
Enter Arrival Time and Burst Time for P1: 0 15
Enter Arrival Time and Burst Time for P2: 1 8
Enter Arrival Time and Burst Time for P3: 3 22
Enter Arrival Time and Burst Time for P4: 5 5

Process AT      BT      CT      WT      TAT
P1      0       15      38      23      38
P2      1       8       18      9       17
P3      3       22      50      25      47
P4      5       5       33      23      28

Average Waiting Time = 20.00
Average Turnaround Time = 32.50
```

#### Test case 3

```text
Roll no: 25071A6245
Enter number of processes: 3
Enter Arrival Time and Burst Time for P1: 0 24
Enter Arrival Time and Burst Time for P2: 0 3
Enter Arrival Time and Burst Time for P3: 0 3

Process AT      BT      CT      WT      TAT
P1      0       24      30      6       30
P2      0       3       13      10      13
P3      0       3       16      13      16

Average Waiting Time = 9.67
Average Turnaround Time = 19.67
```
