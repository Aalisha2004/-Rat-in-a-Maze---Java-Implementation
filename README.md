# 🐭 Rat in a Maze - Java Implementation

This Java program solves the classic **Rat in a Maze** problem using **Backtracking**. The rat starts from the top-left corner of the maze and tries to reach the bottom-right corner, moving only **right** or **down** through cells marked with `1`. Cells marked with `0` are blocked.

## 📌 Problem Statement

Given a maze represented as a 2D array of `0`s and `1`s:

* `1` indicates the cell is open and can be traversed.
* `0` indicates a blocked cell.

The rat can move **right** or **down** one step at a time. The goal is to determine a path from the start `(0, 0)` to the destination `(N-1, N-1)` and print the solution path as a matrix.

---

## 📁 Files

* `mouseSolution.java` — Main program that solves the maze using backtracking.

---

## ▶️ How to Run

### 1. Compile the program:

```bash
javac mouseSolution.java
```

### 2. Run the program:

```bash
java mouseSolution
```

---

## 🧠 Algorithm Overview

* **Backtracking** is used to explore possible paths from the start to the end.
* The `solveMazeUtil` function recursively tries to move right or down.
* If it reaches the goal, it prints the solution matrix.
* The solution matrix contains `1` for cells that are part of the path and `0` otherwise.

---

## 🧪 Sample Input

```java
int maze[][] = {
    {1, 0, 0, 0},
    {1, 1, 0, 1},
    {0, 1, 0, 0},
    {1, 1, 1, 1}
};
```

## ✅ Output

```
1000
1100
0110
0001
```

Each `1` in the output shows a step in the valid path from start to end.

---

## ❌ No Solution Case

If no valid path exists, the program prints:

```
Solution doesn't exist
```

---

## 📚 Concepts Used

* Recursion
* Backtracking
* Matrix traversal
* Basic Java syntax

---

## ✍️ Author

This program was written as an implementation of the classic rat-in-a-maze problem in Java. Ideal for educational purposes, interview prep, or understanding backtracking.

