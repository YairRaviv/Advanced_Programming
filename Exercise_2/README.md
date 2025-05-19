# Advanced Programming - Exercise 2

This folder contains the implementation for Exercise 2 of the Advanced Programming course.

## Contents

- `stree.c`: The main C file containing the implementation of a directory tree viewer
- `Makefile`: Build script for compiling the code

## Overview

This exercise implements a directory tree viewer called "stree" (system tree). The program displays the directory structure in a tree-like format, similar to the Linux `tree` command, but with additional file information and color coding.

## Features

- Displays directory structure in a tree-like format
- Shows detailed file information including permissions, owner, group, and size
- Color coding for different file types:
  - Blue for directories
  - Red for ZIP files
  - Green for executable files
- Skip hidden files and directories
- Displays total count of directories and files at the end

## Implementation Details

The program uses the `nftw` (File Tree Walk) function to traverse the directory structure. For each file or directory encountered, it displays the file information and updates the appropriate counters. The program also handles various edge cases, such as hidden files and directories.

## Compilation and Usage

```bash
# To compile the program
make

# To run the program (displays the directory tree starting from the current directory)
./stree

# To run the program with a specific directory as root
./stree /path/to/directory

# To clean the build files
make clean
```

## Example Output

```
.
├── [drwxr-xr-x user group           4096]  folder1
│   ├── [drwxr-xr-x user group           4096]  subfolder
│   │   ├── [-rw-r--r-- user group           1024]  file1.txt
│   │   └── [-rwxr-xr-x user group           2048]  script.sh
│   └── [-rw-r--r-- user group           512]  document.txt
└── [-rw-r--r-- user group           2048]  data.zip

2 directories, 4 files
```