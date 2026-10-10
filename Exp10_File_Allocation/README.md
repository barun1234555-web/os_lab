# Experiment 10 — File Allocation Strategies

**Subject:** Operating Systems Lab  |  **Roll no:** 25071A6245

## File Allocation

**Aim:** Simulate all file allocation strategies. A. Sequential, B. Indexed, C. Linked

### A. Sequential

**Source:** [`sequential_allocation.c`](sequential_allocation.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter start block and length of file: 12 4
File allocated successfully. Blocks: 12 13 14 15
```

#### Test case 2

```text
Roll no: 25071A6245
Enter start block and length of file: 0 5
File allocated successfully. Blocks: 0 1 2 3 4
```

#### Test case 3

```text
Roll no: 25071A6245
Enter start block and length of file: 20 6
File allocated successfully. Blocks: 20 21 22 23 24 25
```

### B. Indexed

**Source:** [`indexed_allocation.c`](indexed_allocation.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter index block: 9
Enter number of blocks and block numbers: 4 14 18 23 29
Index Block 9 points to: 14 18 23 29
File allocated successfully.
```

#### Test case 2

```text
Roll no: 25071A6245
Enter index block: 5
Enter number of blocks and block numbers: 3 10 20 30
Index Block 5 points to: 10 20 30
File allocated successfully.
```

#### Test case 3

```text
Roll no: 25071A6245
Enter index block: 9
Enter number of blocks and block numbers: 3 4 11 15
Index Block 9 points to: 4 11 15
File allocated successfully.
```

### C. Linked

**Source:** [`linked_allocation.c`](linked_allocation.c)

#### Test case 1

```text
Roll no: 25071A6245
Enter number of blocks and block sequence: 4 5 11 25 34
Linked Allocation Sequence: 5 -> 11 -> 25 -> 34 -> NULL
File allocated successfully.
```

#### Test case 2

```text
Roll no: 25071A6245
Enter number of blocks and block sequence: 3 2 8 18
Linked Allocation Sequence: 2 -> 8 -> 18 -> NULL
File allocated successfully.
```

#### Test case 3

```text
Roll no: 25071A6245
Enter number of blocks and block sequence: 4 1 5 12 20
Linked Allocation Sequence: 1 -> 5 -> 12 -> 20 -> NULL
File allocated successfully.
```
