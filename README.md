# C++ Algorithmic Solutions & Data Structures

## 📖 Overview
This repository contains a collection of C++ implementations solving classic computer science problems. The projects range from Object-Oriented implementations of mathematical concepts (Complex Numbers, Rationals) to advanced backtracking algorithms (N-Queens, Stable Marriage) and numerical analysis.

These programs demonstrate proficiency in memory management, operator overloading, recursion, and iterative backtracking.

## 📂 Project Categories

### ♟️ Backtracking & Recursion
A significant portion of this repository focuses on solving constraint satisfaction problems using backtracking.

* **The 8 Queens Problem (Multiple Variations):**
    * **1D Array Logic:** Solves the problem using a single 1D array to represent row positions.
    * **2D Array Logic:** Validates safe spots using a full board matrix representation.
    * **Goto Implementation:** A low-level iterative approach using `goto` labels to manage control flow.
    * **Fancy Output:** Renders the chess board visually in the console using ASCII/Unicode block characters to represent black and white squares.
    * **N-Queens Generalization:** A dynamic solution that accepts user input for `N` and solves for any board size using heap memory allocation.


* **8 Numbers in a Cross:**
    * Places numbers 0-7 in a cross pattern such that no two adjacent numbers are consecutive integers.
* **Stable Marriage Problem:**
    * Implements the matching algorithm to find stable pairings between $n$ men and $n$ women based on preference lists.

### 🧮 Object-Oriented Programming (OOP)
Custom classes built from scratch to handle mathematical data types not native to C++.

* **Complex Number Class:**
    * Encapsulation of Real and Imaginary parts.
    * **Operator Overloading:** Custom implementation of `+`, `-`, and `*` to allow natural syntax (e.g., `c3 = c1 + c2`).
* **Rational Number Class:**
    * Handles fraction arithmetic (Add, Subtract, Multiply, Divide).
    * **Automatic Reduction:** Uses the Euclidean Algorithm (GCD) to automatically simplify fractions upon instantiation.
    * **Mixed Number Output:** Logic to print improper fractions as mixed numbers (e.g., "1 1/2").

### 📐 Math & Numerical Algorithms
* **Numerical Integration (Riemann Sum):**
    * Calculates the area under a curve for linear, square, and cubic functions.
    * **Advanced Feature:** Uses **Function Pointers** (`typedef double (*FUNC)(double)`) to pass mathematical functions as arguments to the integrator.
* **Memoization (Fibonacci & Factorial):**
    * Uses `static` arrays to cache results of recursive calls, drastically improving performance for repeated calculations.
* **Towers of Hanoi (Iterative):**
    * Solves the classic puzzle without recursion.
    * Uses `std::vector` to simulate stacks for the three towers and bitwise/modulo logic to determine ring movement.


## 🛠️ Technical Highlights
* **Pointers & Memory:** Manual memory management using `new` and `delete`.
* **Control Flow:** Mastery of loops, recursion, and `goto` for state-machine logic.
* **STL Containers:** Usage of `std::vector` and arrays.
* **Polymorphism:** Operator overloading and function pointers.

## 🚀 How to Compile & Run
You can compile any of these files using `g++` or any standard C++ compiler.

**Example:**
```bash
# Compile the N-Queens solver
g++ nqueens.cpp -o nqueens

# Run the executable
./nqueens
