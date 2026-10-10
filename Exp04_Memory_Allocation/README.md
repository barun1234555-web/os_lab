# Experiment 4 — Implementation of Memory Allocation Methods

**Subject:** Operating Systems Lab  |  **Roll no:** 25071A6245

## Memory Allocation (fixed partition)

**Aim:** Implementation of the following Memory Allocation Methods for fixed partition a) First Fit b) Worst Fit c) Best Fit

### A. First Fit

**Source:** [`first_fit.c`](first_fit.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of blocks: 5
Enter block sizes: 100 500 200 300 600
Enter number of processes: 4
Enter process sizes: 212 417 112 426

Process Process Size    Block No.       Block Size      Internal Frag
P1      212             2               500             288
P2      417             5               600             183
P3      112             3               200             88
P4      426             Not Allocated   -               -
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of blocks: 4
Enter block sizes: 200 400 600 500
Enter number of processes: 4
Enter process sizes: 150 350 450 100

Process Process Size    Block No.       Block Size      Internal Frag
P1      150             1               200             50
P2      350             2               400             50
P3      450             3               600             150
P4      100             4               500             400
```

#### Test case 3

```text
Roll no: 25071A6245
Enter number of blocks: 5
Enter block sizes: 300 150 200 350 600
Enter number of processes: 4
Enter process sizes: 120 290 180 550

Process Process Size    Block No.       Block Size      Internal Frag
P1      120             1               300             180
P2      290             4               350             60
P3      180             3               200             20
P4      550             5               600             50
```

### B. Worst Fit

**Source:** [`worst_fit.c`](worst_fit.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of blocks: 5
Enter block sizes: 100 500 200 300 600
Enter number of processes: 4
Enter process sizes: 212 417 112 426

Process Process Size    Block No.       Block Size      Internal Frag
P1      212             5               600             388
P2      417             2               500             83
P3      112             4               300             188
P4      426             Not Allocated   -               -
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of blocks: 4
Enter block sizes: 200 400 600 500
Enter number of processes: 4
Enter process sizes: 150 250 100 300

Process Process Size    Block No.       Block Size      Internal Frag
P1      150             3               600             450
P2      250             4               500             250
P3      100             2               400             300
P4      300             Not Allocated   -               -
```

#### Test case 3

```text
Roll no: 25071A6245
Enter number of blocks: 5
Enter block sizes: 300 150 200 350 600
Enter number of processes: 4
Enter process sizes: 120 290 180 100

Process Process Size    Block No.       Block Size      Internal Frag
P1      120             5               600             480
P2      290             4               350             60
P3      180             1               300             120
P4      100             3               200             100
```

### C. Best Fit

**Source:** [`best_fit.c`](best_fit.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of blocks: 5
Enter block sizes: 100 500 200 300 600
Enter number of processes: 4
Enter process sizes: 212 417 112 426

Process Process Size    Block No.       Block Size      Internal Frag
P1      212             4               300             88
P2      417             2               500             83
P3      112             3               200             88
P4      426             5               600             174
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of blocks: 4
Enter block sizes: 200 400 600 500
Enter number of processes: 4
Enter process sizes: 150 350 450 100

Process Process Size    Block No.       Block Size      Internal Frag
P1      150             1               200             50
P2      350             2               400             50
P3      450             4               500             50
P4      100             3               600             500
```

#### Test case 3

```text
Roll no: 25071A6245
Enter number of blocks: 5
Enter block sizes: 300 150 200 350 600
Enter number of processes: 4
Enter process sizes: 120 290 180 550

Process Process Size    Block No.       Block Size      Internal Frag
P1      120             2               150             30
P2      290             1               300             10
P3      180             3               200             20
P4      550             5               600             50
```
