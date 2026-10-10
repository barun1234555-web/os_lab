# Experiment 5 — Paging Technique of Memory Management

**Subject:** Operating Systems Lab  |  **Roll no:** 25071A6245

## Paging

**Aim:** Implementation of Paging Technique of Memory Management

### Paging Technique (logical → physical address)

**Source:** [`paging.c`](paging.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter main memory size (in bytes): 1024
Enter page size (in bytes): 128
Total frames available in memory: 8

Enter process size (in bytes): 350
Total pages required for process: 3
Enter frame numbers allocated to each page:
Page 0 -> Frame No: 5
Page 1 -> Frame No: 2
Page 2 -> Frame No: 7

Enter Logical Address to translate: 200

--- Address Translation Details ---
Page Number (p)    : 1
Page Offset (d)    : 72
Allocated Frame No : 2
Physical Address   : 328
```

#### Test case 2

```text
Roll no: 25071A6245
Enter main memory size (in bytes): 2048
Enter page size (in bytes): 256
Total frames available in memory: 8

Enter process size (in bytes): 600
Total pages required for process: 3
Enter frame numbers allocated to each page:
Page 0 -> Frame No: 1
Page 1 -> Frame No: 4
Page 2 -> Frame No: 6

Enter Logical Address to translate: 900

Invalid Logical Address! (Page number 3 exceeds allocated pages)
```

#### Test case 3

```text
Roll no: 25071A6245
Enter main memory size (in bytes): 512
Enter page size (in bytes): 64
Total frames available in memory: 8

Enter process size (in bytes): 700

Memory Allocation Failed: Not enough frames available.
```
