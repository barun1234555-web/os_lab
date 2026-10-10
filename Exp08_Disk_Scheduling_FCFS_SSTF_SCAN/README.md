# Experiment 8 — Disk Scheduling Algorithms: FCFS, SSTF, SCAN

**Subject:** Operating Systems Lab  |  **Roll no:** 25071A6245

## Disk Scheduling

**Aim:** Simulate the following Disk scheduling algorithms. A) FCFS B) SSTF C) SCAN

### A) FCFS

**Source:** [`fcfs_disk.c`](fcfs_disk.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of requests: 8
Enter request sequence: 98 183 37 122 14 124 65 67
Enter initial head position: 53

Seek Sequence: 53 -> 98 -> 183 -> 37 -> 122 -> 14 -> 124 -> 65 -> 67
Total Head Movement = 640
Average Seek Time = 80.00
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of requests: 5
Enter request sequence: 176 79 34 60 92
Enter initial head position: 50

Seek Sequence: 50 -> 176 -> 79 -> 34 -> 60 -> 92
Total Head Movement = 326
Average Seek Time = 65.20
```

#### Test case 3

```text
Roll no: 25071A6245
Enter number of requests: 6
Enter request sequence: 10 150 20 140 30 130
Enter initial head position: 100

Seek Sequence: 100 -> 10 -> 150 -> 20 -> 140 -> 30 -> 130
Total Head Movement = 690
Average Seek Time = 115.00
```

### B) SSTF

**Source:** [`sstf_disk.c`](sstf_disk.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of requests: 8
Enter request sequence: 98 183 37 122 14 124 65 67
Enter initial head position: 53

Seek Sequence: 53 -> 65 -> 67 -> 37 -> 14 -> 98 -> 122 -> 124 -> 183
Total Head Movement = 236
Average Seek Time = 29.50
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of requests: 5
Enter request sequence: 176 79 34 60 92
Enter initial head position: 50

Seek Sequence: 50 -> 60 -> 79 -> 92 -> 34 -> 176
Total Head Movement = 242
Average Seek Time = 48.40
```

#### Test case 3

```text
Roll no: 25071A6245
Enter number of requests: 6
Enter request sequence: 10 150 20 140 30 130
Enter initial head position: 100

Seek Sequence: 100 -> 130 -> 140 -> 150 -> 30 -> 20 -> 10
Total Head Movement = 190
Average Seek Time = 31.67
```

### C) SCAN

**Source:** [`scan_disk.c`](scan_disk.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of requests: 8
Enter request sequence: 98 183 37 122 14 124 65 67
Enter initial head position: 53
Enter total disk size: 200
Enter direction (1 for High/Right, 0 for Low/Left): 1

Seek Sequence: 53 -> 65 -> 67 -> 98 -> 122 -> 124 -> 183 -> 199 -> 37 -> 14
Total Head Movement = 331
Average Seek Time = 41.38
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of requests: 5
Enter request sequence: 176 79 34 60 92
Enter initial head position: 50
Enter total disk size: 200
Enter direction (1 for High/Right, 0 for Low/Left): 1

Seek Sequence: 50 -> 60 -> 79 -> 92 -> 176 -> 199 -> 34
Total Head Movement = 314
Average Seek Time = 62.80
```

#### Test case 3

```text
Roll no: 25071A6245
Enter number of requests: 6
Enter request sequence: 10 150 20 140 30 130
Enter initial head position: 100
Enter total disk size: 200
Enter direction (1 for High/Right, 0 for Low/Left): 1

Seek Sequence: 100 -> 130 -> 140 -> 150 -> 199 -> 30 -> 20 -> 10
Total Head Movement = 288
Average Seek Time = 48.00
```
