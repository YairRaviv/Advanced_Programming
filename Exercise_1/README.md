# Advanced Programming - Exercise 1

This folder contains the implementation for Exercise 1 of the Advanced Programming course.

## Contents

- `slast.c`: The main C file containing the implementation of a simplified "last" command
- `Makefile`: Build script for compiling the code

## Overview

This exercise implements a simplified version of the Unix/Linux "last" command called "slast" (simplified last). The program displays recent user login information from the system's wtmp file.

## Features

- Displays a specified number of recent login records
- Shows user name, terminal, host, and login time for each entry
- Special formatting for system reboots
- Parameters validation

## Implementation Details

The program accesses the `/var/log/wtmp` file which contains login records in the utmp structure format. It reads the file in reverse order to display the most recent logins first. The program filters the entries to display only user logins and system reboots.

## Compilation and Usage

```bash
# To compile the program
make

# To run the program (displays the last N login entries)
./slast N

# To clean the build files
make clean
```

## Example Usage

```
./slast 5
```

This command will display the 5 most recent login entries in the system.