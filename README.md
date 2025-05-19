# Advanced Programming Repository

This repository contains a collection of projects, assignments, and implementations from my Advanced Programming coursework at Ariel University.

## Repository Organization Note

This repository is organized by exercises, where each exercise is contained in its own folder (Exercise_X). This structure provides a clean organization of the different advanced programming concepts explored in each assignment.

## Overview

Advanced Programming explores sophisticated programming concepts, paradigms, and techniques beyond the basics. This repository includes implementations of various advanced programming concepts, system programming, and complex problem-solving techniques in the C programming language.

## Repository Structure

The repository is organized by exercises:

- **Exercise_1**: Simplified "last" command implementation (slast)
- **Exercise_2**: Directory tree viewer implementation (stree)

## Key Topics Covered

- **System Programming**:
  - File I/O operations
  - Directory traversal
  - System information retrieval
  - Process management

- **Advanced C Programming**:
  - Data structures
  - Memory management
  - Pointers and function pointers
  - File descriptor manipulation

- **Linux/Unix System Interfaces**:
  - System calls and library functions
  - User and group management
  - File permissions and attributes
  - Terminal I/O

## Exercise Details

### Exercise 1: Simplified Last Command (slast)

Implementation of a simplified version of the Unix/Linux "last" command. This command displays recent user login information from the system's wtmp file, showing user login history with timestamps.

### Exercise 2: Directory Tree Viewer (stree)

Implementation of a directory tree viewer that displays the directory structure in a tree-like format, similar to the Linux `tree` command. The program shows detailed file information including permissions, owner, group, and size, with color coding for different file types.

## Technologies Used

- **C Programming Language**: For system programming and low-level operations
- **Linux/Unix System Calls**: For interacting with the operating system
- **Standard C Library**: For basic operations and data structures

## Getting Started

### Prerequisites

- GCC compiler
- Linux/Unix operating system
- Make utility

### Building and Running

```bash
# Clone this repository
git clone https://github.com/YairRaviv/Advanced_Programming.git

# Navigate to a specific exercise
cd Advanced_Programming/Exercise_1

# Build the project
make

# Run the application
./slast 5    # For Exercise_1, shows last 5 login records

# Or for Exercise_2
cd ../Exercise_2
make
./stree      # Shows directory tree from current directory
```

## Learning Outcomes

- Master system programming concepts in C
- Develop efficient and reliable system utilities
- Work with file systems and system information
- Apply proper error handling in system applications
- Implement color and formatting in terminal applications

## License

This project is available for educational purposes. Please respect academic integrity policies when using this code.

## Acknowledgments

Special thanks to the course instructors and teaching assistants for their guidance throughout this learning journey.
