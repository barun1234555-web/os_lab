# Experiment 7 — Frame Allocation Methods

**Subject:** Operating Systems Lab  |  **Roll no:** 25071A6245

## Frame Allocation

**Aim:** Simulate frame allocation Methods. A) minimum number of frames B) equal allocation C) proportional allocation

### A. Minimum number of frames

**Source:** [`minimum_frames.c`](minimum_frames.c)

#### Test case 1

```text
Roll no: 25071A6245

Enter total frames in physical memory: 10
Enter minimum frames required per process (by architecture): 2
Enter number of processes: 3
Enter page requirements for each process:
Process P1: 5
Process P2: 2
Process P3: 4

--- Minimum Frame Allocation Result ---
Process Page Req        Allocated Frames        Status
P1      5               2                       Needs Swap Space
P2      2               2                       Satisfied
P3      4               2                       Needs Swap Space

Total Frames Allocated: 6 / 10
Remaining Unallocated Frames: 4
```

#### Test case 2

```text
Roll no: 25071A6245

Enter total frames in physical memory: 5
Enter minimum frames required per process (by architecture): 2
Enter number of processes: 3

Allocation Failed! Total available frames (5) < Required minimum frames (6).
```

#### Test case 3

```text
Roll no: 25071A6245

Enter total frames in physical memory: 12
Enter minimum frames required per process (by architecture): 2
Enter number of processes: 3
Enter page requirements for each process:
Process P1: 2
Process P2: 2
Process P3: 2

--- Minimum Frame Allocation Result ---
Process Page Req        Allocated Frames        Status
P1      2               2                       Satisfied
P2      2               2                       Satisfied
P3      2               2                       Satisfied

Total Frames Allocated: 6 / 12
Remaining Unallocated Frames: 6
```

### B. Equal allocation

**Source:** [`equal_allocation.c`](equal_allocation.c)

#### Test case 1

```text
Roll no: 25071A6245

Enter total frames in physical memory: 63
Enter number of processes: 3
Enter page requirements for each process:
Process P1: 10
Process P2: 127
Process P3: 18

--- Equal Frame Allocation Result ---
Process Page Req        Allocated Frames        Unmet Pages
P1      10              21                      0
P2      127             21                      106
P3      18              21                      0

Total Allocated Frames: 63 / 63
Leftover System Frames: 0
```

#### Test case 2

```text
Roll no: 25071A6245

Enter total frames in physical memory: 100
Enter number of processes: 3
Enter page requirements for each process:
Process P1: 40
Process P2: 25
Process P3: 60

--- Equal Frame Allocation Result ---
Process Page Req        Allocated Frames        Unmet Pages
P1      40              33                      7
P2      25              33                      0
P3      60              33                      27

Total Allocated Frames: 99 / 100
Leftover System Frames: 1
```

#### Test case 3

```text
Roll no: 25071A6245

Enter total frames in physical memory: 60
Enter number of processes: 3
Enter page requirements for each process:
Process P1: 15
Process P2: 12
Process P3: 18

--- Equal Frame Allocation Result ---
Process Page Req        Allocated Frames        Unmet Pages
P1      15              20                      0
P2      12              20                      0
P3      18              20                      0

Total Allocated Frames: 60 / 60
Leftover System Frames: 0
```

### C. Proportional allocation

**Source:** [`proportional_allocation.c`](proportional_allocation.c)

#### Test case 1

```text
Roll no: 25071A6245

Enter total frames available in physical memory: 62
Enter number of processes: 2
Enter size (in pages/virtual memory) for each process:
Process P1 size: 10
Process P2 size: 127

--- Proportional Frame Allocation Result ---
Total Virtual Memory Required (S) = 137 pages

Process Size (s_i)      Allocated Frames (a_i)  Percentage
P1      10              4                       7.30%
P2      127             57                      92.70%

Total Frames Allocated: 61 / 62
Unallocated Buffer Frames: 1
```

#### Test case 2

```text
Roll no: 25071A6245

Enter total frames available in physical memory: 100
Enter number of processes: 3
Enter size (in pages/virtual memory) for each process:
Process P1 size: 50
Process P2 size: 50
Process P3 size: 50

--- Proportional Frame Allocation Result ---
Total Virtual Memory Required (S) = 150 pages

Process Size (s_i)      Allocated Frames (a_i)  Percentage
P1      50              33                      33.33%
P2      50              33                      33.33%
P3      50              33                      33.33%

Total Frames Allocated: 99 / 100
Unallocated Buffer Frames: 1
```

#### Test case 3

```text
Roll no: 25071A6245

Enter total frames available in physical memory: 60
Enter number of processes: 3
Enter size (in pages/virtual memory) for each process:
Process P1 size: 20
Process P2 size: 30
Process P3 size: 50

--- Proportional Frame Allocation Result ---
Total Virtual Memory Required (S) = 100 pages

Process Size (s_i)      Allocated Frames (a_i)  Percentage
P1      20              12                      20.00%
P2      30              18                      30.00%
P3      50              30                      50.00%

Total Frames Allocated: 60 / 60
Unallocated Buffer Frames: 0
```
