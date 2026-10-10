# Experiment 1 — FCFS and SJF Scheduling Algorithms

**Subject:** Operating Systems Lab  |  **Roll no:** 25071A6245

## FCFS Scheduling

**Aim:** Write a C program for FCFS scheduling algorithm A. without arrival times, B. with arrival times

### A. Without arrival times

**Source:** [`fcfs_without_arrival.c`](fcfs_without_arrival.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of processes: 3
Enter Burst Time for P1: 24
Enter Burst Time for P2: 3
Enter Burst Time for P3: 3

Process BT      WT      TAT
P1      24      0       24
P2      3       24      27
P3      3       27      30

Avg WT = 17.00 | Avg TAT = 27.00
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of processes: 4
Enter Burst Time for P1: 2
Enter Burst Time for P2: 10
Enter Burst Time for P3: 4
Enter Burst Time for P4: 7

Process BT      WT      TAT
P1      2       0       2
P2      10      2       12
P3      4       12      16
P4      7       16      23

Avg WT = 7.50 | Avg TAT = 13.25
```

#### Test case 3

```text
Roll no: 25071A6245
Enter number of processes: 4
Enter Burst Time for P1: 2
Enter Burst Time for P2: 4
Enter Burst Time for P3: 6
Enter Burst Time for P4: 8

Process BT      WT      TAT
P1      2       0       2
P2      4       2       6
P3      6       6       12
P4      8       12      20

Avg WT = 5.00 | Avg TAT = 10.00
```

### B. With arrival times

**Source:** [`fcfs_with_arrival.c`](fcfs_with_arrival.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of processes: 3
Enter Arrival Time and Burst Time for P1: 0 24
Enter Arrival Time and Burst Time for P2: 1 3
Enter Arrival Time and Burst Time for P3: 2 3

Process AT      BT      CT      WT      TAT
P1      0       24      24      0       24
P2      1       3       27      23      26
P3      2       3       30      25      28

Average Waiting Time = 16.00
Average Turnaround Time = 26.00
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of processes: 3
Enter Arrival Time and Burst Time for P1: 1 4
Enter Arrival Time and Burst Time for P2: 2 3
Enter Arrival Time and Burst Time for P3: 10 2

Process AT      BT      CT      WT      TAT
P1      1       4       5       0       4
P2      2       3       8       3       6
P3      10      2       12      0       2

Average Waiting Time = 1.00
Average Turnaround Time = 4.00
```

#### Test case 3

```text
Roll no: 25071A6245
Enter number of processes: 3
Enter Arrival Time and Burst Time for P1: 0 24
Enter Arrival Time and Burst Time for P2: 0 3
Enter Arrival Time and Burst Time for P3: 0 3

Process AT      BT      CT      WT      TAT
P1      0       24      24      0       24
P2      0       3       27      24      27
P3      0       3       30      27      30

Average Waiting Time = 17.00
Average Turnaround Time = 27.00
```

## SJF Scheduling

**Aim:** Write a C program for SJF scheduling algorithm A. Non-preemptive B. Preemptive

### A. Non-preemptive

**Source:** [`sjf_non_preemptive.c`](sjf_non_preemptive.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of processes: 3
Enter Arrival Time and Burst Time for P1: 0 3
Enter Arrival Time and Burst Time for P2: 5 6
Enter Arrival Time and Burst Time for P3: 6 2

Process AT      BT      CT      WT      TAT
P1      0       3       3       0       3
P2      5       6       11      0       6
P3      6       2       13      5       7

Average Waiting Time = 1.67
Average Turnaround Time = 5.33
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of processes: 4
Enter Arrival Time and Burst Time for P1: 0 7
Enter Arrival Time and Burst Time for P2: 2 4
Enter Arrival Time and Burst Time for P3: 4 1
Enter Arrival Time and Burst Time for P4: 5 4

Process AT      BT      CT      WT      TAT
P1      0       7       7       0       7
P2      2       4       12      6       10
P3      4       1       8       3       4
P4      5       4       16      7       11

Average Waiting Time = 4.00
Average Turnaround Time = 8.00
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
P2      0       3       3       0       3
P3      0       3       6       3       6

Average Waiting Time = 3.00
Average Turnaround Time = 13.00
```

### B. Preemptive

**Source:** [`sjf_preemptive.c`](sjf_preemptive.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of processes: 3
Enter Arrival Time and Burst Time for P1: 0 8
Enter Arrival Time and Burst Time for P2: 1 4
Enter Arrival Time and Burst Time for P3: 2 2

Process AT      BT      CT      WT      TAT
P1      0       8       14      6       14
P2      1       4       7       2       6
P3      2       2       4       0       2

Average Waiting Time = 2.67
Average Turnaround Time = 7.33
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of processes: 4
Enter Arrival Time and Burst Time for P1: 0 8
Enter Arrival Time and Burst Time for P2: 1 4
Enter Arrival Time and Burst Time for P3: 2 9
Enter Arrival Time and Burst Time for P4: 3 5

Process AT      BT      CT      WT      TAT
P1      0       8       17      9       17
P2      1       4       5       0       4
P3      2       9       26      15      24
P4      3       5       10      2       7

Average Waiting Time = 6.50
Average Turnaround Time = 13.00
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
P2      0       3       3       0       3
P3      0       3       6       3       6

Average Waiting Time = 3.00
Average Turnaround Time = 13.00
```
