# CS598APE HW3

This repository contains optimized code for homework 3 of CS598APE. 

`sandpile.c` contains the implementation of finding the identity element of a 2D
abelian sandpile.

![Identity sandpile on a 1001x1001 pacman grid](identity-ref.png)

*Identity sandpile on a 1001x1001 pacman grid*


To compile the program, run:

```bash
make all
```

To clean existing build artifacts, run:

```bash
make clean
```

Usage (after compiling):

```bash
./sandpile.exe <N> 
```

where `N` is the grid size

All optimizations were benchmarked with grid size N = 1001:

```bash
./sandpile.exe 1001
```
To isolate the effect of each optimization, benchmark the corresponding commit using `git checkout <commit-hash>`.
| Commit | Link | Optimization |
|---|---|---|
| `d292b3a` | [View Commit](https://github.com/sherrylong/598APE-HW3/commit/d292b3a) | Batch topples |
| `2c27f6a` | [View Commit](https://github.com/sherrylong/598APE-HW3/commit/2c27f6a) | Precompute topple region |
| `d21ad1a` | [View Commit](https://github.com/sherrylong/598APE-HW3/commit/d21ad1a) | Precompute column ranges |
| `0ee327f` | [View Commit](https://github.com/sherrylong/598APE-HW3/commit/0ee327f) | Compiler optimizations |
| `98a2d15` | [View Commit](https://github.com/sherrylong/598APE-HW3/commit/98a2d15) | OpenMP parallelization |



