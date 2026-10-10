# Experiment 9 — Disk Scheduling Algorithms: C-SCAN, LOOK, C-LOOK

**Subject:** Operating Systems Lab  |  **Roll no:** 25071A6245

## Disk Scheduling

**Aim:** Simulate the following Disk scheduling algorithms. A) C-SCAN B) LOOK C) C-LOOK

### A) C-SCAN

**Source:** [`cscan_disk.c`](cscan_disk.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of requests: 8
Enter request sequence: 98 183 37 122 14 124 65 67
Enter initial head position: 53
Enter total disk size: 200

Seek Sequence: 53 -> 65 -> 67 -> 98 -> 122 -> 124 -> 183 -> 199 -> 0 -> 14 -> 37
Total Head Movement = 382
Average Seek Time = 47.75
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of requests: 5
Enter request sequence: 176 79 34 60 92
Enter initial head position: 50
Enter total disk size: 200

Seek Sequence: 50 -> 60 -> 79 -> 92 -> 176 -> 199 -> 0 -> 34
Total Head Movement = 382
Average Seek Time = 76.40
```

#### Test case 3

```text
Roll no: 25071A6245
Enter number of requests: 6
Enter request sequence: 10 150 20 140 30 130
Enter initial head position: 100
Enter total disk size: 200

Seek Sequence: 100 -> 130 -> 140 -> 150 -> 199 -> 0 -> 10 -> 20 -> 30
Total Head Movement = 328
Average Seek Time = 54.67
```

### B) LOOK

**Source:** [`look_disk.c`](look_disk.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of requests: 8
Enter request sequence: 98 183 37 122 14 124 65 67
Enter initial head position: 53

Seek Sequence: 53 -> 65 -> 67 -> 98 -> 122 -> 124 -> 183 -> 37 -> 14
Total Head Movement = 299
Average Seek Time = 37.38
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of requests: 5
Enter request sequence: 176 79 34 60 92
Enter initial head position: 50

Seek Sequence: 50 -> 60 -> 79 -> 92 -> 176 -> 34
Total Head Movement = 268
Average Seek Time = 53.60
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

### C) C-LOOK

**Source:** [`clook_disk.c`](clook_disk.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of requests: 8
Enter request sequence: 98 183 37 122 14 124 65 67
Enter initial head position: 53

Seek Sequence: 53 -> 65 -> 67 -> 98 -> 122 -> 124 -> 183 -> 14 -> 37
Total Head Movement = 322
Average Seek Time = 40.25
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of requests: 5
Enter request sequence: 176 79 34 60 92
Enter initial head position: 50

Seek Sequence: 50 -> 60 -> 79 -> 92 -> 176 -> 34
Total Head Movement = 268
Average Seek Time = 53.60
```

#### Test case 3

```text
Roll no: 25071A6245
Enter number of requests: 6
Enter request sequence: 10 150 20 140 30 130
Enter initial head position: 100

Seek Sequence: 100 -> 130 -> 140 -> 150 -> 10 -> 20 -> 30
Total Head Movement = 210
Average Seek Time = 35.00
```
