# 📘 DATA STRUCTURES (C Programs)

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](LICENSE) [![Language: C](https://img.shields.io/badge/Language-C-%23007ACC.svg?style=flat&logo=c)](https://en.wikipedia.org/wiki/C_(programming_language))

A clean, beginner-friendly collection of data structure implementations written in C. This repo groups small, standalone programs by topic (stacks, queues, linked lists, trees, hashing, sorting, expression conversion, and more) and aims to help students understand the internal workings of each data structure through concise, well-commented code.

Why this repo?
- Small, focused programs — each `.c` file demonstrates one concept or operation.
- Beginner-friendly: readable code, comments, and simple CLI usage.
- Easy to compile and run with any GCC toolchain.

## Table of contents

- [Repository structure](#repository-structure)
- [Quick start — compile & run](#quick-start----compile--run)
- [Recommended compiler flags](#recommended-compiler-flags)
- [How to contribute](#how-to-contribute)
- [Coding & file placement guidelines](#coding--file-placement-guidelines)
- [License](#license)

---

## Repository structure

Top-level layout:

```
DATA-STRUCTURES/
├── C-PROGRAMS/          # Basic or general C programs
├── HASHING/             # Hash tables & collision handling techniques
├── INFIX-TO-POSTFIX/    # Expression conversion & postfix evaluation
├── LINKED-LIST/         # Singly, doubly & circular linked lists
├── QUEUES/              # Queue implementations (array & linked list)
├── SORTING/             # Sorting algorithms (bubble, quick, merge, etc.)
├── STACKS/              # Stack operations & applications
├── TREES/               # Binary tree, BST, traversals
└── LICENSE              # GPL-3.0 License
```

Each folder contains standalone `.c` programs that can be compiled and run individually. Files are intentionally minimal — import and run the single file you want to study.

---

## Quick start — compile & run

Requirements
- GCC (or any C compiler supporting C11)
- Optional: VS Code with C/C++ extension for editing

Example: compile and run a program (macOS / Linux / WSL)

```bash
# compile
gcc -std=c11 -Wall -Wextra -O0 path/to/file.c -o program

# run
./program
```

Example using a file from `STACKS/` (adjust filename to the file in that folder):

```bash
cd STACKS
gcc -std=c11 -Wall -Wextra StackExample.c -o StackExample
./StackExample
```

Windows (MinGW/MSYS2):

```bash
gcc -std=c11 -Wall -Wextra path\\to\\file.c -o program.exe
./program.exe
```

### Recommended compiler flags
- `-std=c11` — use C11 standard
- `-Wall -Wextra` — enable useful warnings
- `-g` — include debug info (useful when stepping through with a debugger)
- `-O0` — no optimization while learning/debugging

---

## How to contribute

Contributions are very welcome! Simple rules to keep the repo useful for beginners:

1. Fork this repository.
2. Create a descriptive branch: `git checkout -b feature/new-program-name`.
3. Add your `.c` file to the relevant folder (pick the closest topic).
4. Include a short header comment in the file describing the program, inputs and outputs, and any complexity notes.
5. Keep the code simple and well-commented.
6. Run the code locally and verify it compiles without errors.
7. Commit and push, then open a Pull Request describing what you added and why.

Suggested commit message format:

```
Add: <short description of program> — <folder/topic>
```

### Contribution rules
- Keep examples short and focused on teaching a single concept.
- Avoid external dependencies; prefer plain C and the standard library.
- Use descriptive variable names and comment non-obvious logic.

If you'd like, I can add a `CONTRIBUTING.md` with a contribution checklist and PR template — tell me and I'll create it.

---

## Coding & file placement guidelines

- Place new programs in the most relevant folder (e.g., sorting algorithms go to `SORTING/`).
- Name files clearly: `merge_sort.c`, `queue_linkedlist.c`, etc.
- Add a top-of-file comment block with:
	- Program purpose
	- Example input/output
	- Complexity (time/space)

Example header you can copy into new files:

```c
/*
 * Program: bubble_sort.c
 * Purpose: Demonstrate bubble sort on an integer array
 * Compile: gcc -std=c11 -Wall -Wextra bubble_sort.c -o bubble_sort
 * Usage: ./bubble_sort
 * Time complexity: O(n^2)
 * Space complexity: O(1)
 */
```

---

## License

This project is licensed under the GPL-3.0 License. See the `LICENSE` file for details.

---

## Contact / Maintainer

Maintained by the repository owner. Contributions and issues are welcome via GitHub.

---

If you want I can:
- add a `CONTRIBUTING.md` with templates,
- add a small `Makefile` with a `make run` target and `make <folder>/<file>` convenience rules,
- or add a Table of Contents with per-folder file lists (auto-generated). Tell me which and I'll implement it.

—

▶️ How to Compile & Run the Code

You can run these programs using Dev-C++, VS Code, or any GCC-based compiler.

1. Running in Dev-C++
		1. Open Dev-C++
		2. Go to File → Open and choose the `.c` file
		3. Click Compile & Run (or press F11)
		4. The output window will appear

—

2. Running in VS Code

Make sure to install:
	• C/C++ Extension (Microsoft)
	• MinGW / GCC Compiler

Steps:
	1. Open your project folder in VS Code
	2. Open the `.c` file you want to run
	3. Compile using terminal: `gcc program.c -o program` then `./program`
	Optional: Install Code Runner for one-click execution.

—

🤝 Contribution Guide

Contributions are welcome! Feel free to add new programs, improve existing ones, or enhance documentation.

How to Contribute
	1. Fork this repository
	2. Create a new branch: `git checkout -b feature-new-program`
	3. Add your C program to the relevant folder
	4. Ensure code is clean and well commented
	5. Commit your changes: `git commit -m "Added new data structure example"`
	6. Push and create a Pull Request

Contribution Rules
	• Keep code simple and beginner-friendly
	• Add a comment header explaining the purpose of the program
	• Place files in the correct topic folder
	• Avoid unnecessary complexity

—

📜 License

This project is licensed under the GPL-3.0 License. See the `LICENSE` file for details.

