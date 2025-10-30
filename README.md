# 🧩 Algorithm Challenges & Solutions

> Collection of algorithm implementations and computational problem solutions in Python

![Python](https://img.shields.io/badge/Python-3.x-3776AB?logo=python&logoColor=white)
![Algorithms](https://img.shields.io/badge/Algorithms-Data%20Structures-orange)

## Overview

Repository containing solutions to mathematical, algorithmic, and data structure challenges. Includes implementations of classic algorithms, Project Euler problems, and practical coding exercises demonstrating fundamental computer science concepts.

## Contents

### 📐 Mathematical Algorithms

**Project Euler Solutions**
- `eulerproject1.txt` - Multiples of 3 and 5 below 1000
- `euler2.txt` - Sum of even Fibonacci numbers under 4 million
- `euler_project.txt` - Largest product of consecutive digits

**Number Theory**
- `amicablesum.txt` - Amicable numbers calculation (sum of divisors)
- `largestdivisor.txt` - Greatest common divisor (recursive)
- `largestdivisorANS2.txt` - GCD iterative implementation
- `Nrmethod.txt` - Newton-Raphson method for square root approximation

**Sequences**
- `fibonaccisequence.txt` - Recursive Fibonacci implementation

### 🔄 Sorting Algorithms

- `bubblesort.txt` - Bubble sort with timing analysis
- `insertionsortfunction.txt` - Insertion sort implementation

### 🔍 Search Algorithms

- `binarysearch.txt` - Binary search on sorted lists
- `binarytree.txt` - Binary tree structure with traversal methods

### 💾 Data Structures

**Binary Tree Implementation**
- Node class with left/right pointers
- Tree creation and attachment methods
- Post-order leaf checker
- Tree printing functionality

### 📊 Time Complexity Visualisation

- `big0.txt` - Big O notation graphing tool
  - Exponential growth (2^n)
  - Quadratic growth (n²)
  - Logarithmic growth (log n)
  - Factorial growth (n!)
  - Matplotlib visualisation

### 🎯 Practical Applications

**Parking System Simulator**
- `parking_system.txt` - Multi-task parking management system
  - Day-specific pricing (Monday-Friday, Saturday, Sunday)
  - Time-based rate calculations (8:00-15:59 vs 16:00-23:59)
  - Frequent parker discount validation (mod 11 check digit)
  - Daily revenue tracking
  - Payment processing with change calculation

**Time Challenge**
- `time_challenge.txt` - Typing speed test measuring input accuracy and time

**File Handling**
- `filehandling.txt` - Student record management with pickle serialisation

## Technical Highlights

### Algorithms Implemented

**Recursion**
```python
# Fibonacci (exponential time complexity)
def fib(x):
    if x==0 or x==1:
        return 1
    return fib(x-1) + fib(x-2)
```

**Iterative GCD (Euclidean Algorithm)**
```python
# O(log min(a,b)) time complexity
def gcdIter(a, b):
    testValue = min(a, b)
    while a % testValue != 0 or b % testValue != 0:
        testValue -= 1
    return testValue
```

**Newton-Raphson Method**
```python
# Square root approximation with epsilon precision
guess = y/2.0
while abs(guess*guess - y) >= epsilon:
    guess = guess - (((guess**2)-y)/(2*guess))
```

### Problem-Solving Skills Demonstrated

✅ **Mathematical reasoning** - Number theory and sequences  
✅ **Algorithm efficiency** - Time/space complexity analysis  
✅ **Data structures** - Trees, arrays, and custom structures  
✅ **Recursion vs iteration** - Multiple implementation approaches  
✅ **Numerical methods** - Approximation algorithms  
✅ **Real-world modelling** - Parking system with business logic  
✅ **Validation logic** - Check digit algorithms (mod 11)

## Project Euler Achievements

- **Problem 1:** Sum of multiples - O(1) solution using arithmetic series
- **Problem 2:** Fibonacci even sum - Efficient iterative approach
- **Problem 3:** Largest product in series - Sliding window technique

## Data Structure Implementations

### Binary Tree
- Array-based storage with index pointers
- Dynamic node attachment
- Traversal algorithms
- Leaf node detection

### Features
- Global node counter for array indexing
- Parent-child relationship management
- Post-order traversal for leaf identification

## Complexity Analysis

**Visualisation Tool Features:**
- Plots growth rates: O(2ⁿ), O(n²), O(log n), O(n!)
- Matplotlib integration for clear visualisation
- Input/output relationship demonstration
- Educational tool for understanding algorithm scaling

## Key Concepts Covered

**Algorithms:**
- Sorting (Bubble, Insertion)
- Searching (Binary Search)
- Recursion and iteration trade-offs
- Numerical approximation methods

**Data Structures:**
- Binary trees
- Arrays and lists
- Custom node structures

**Mathematics:**
- Number theory (GCD, amicable numbers)
- Sequence generation (Fibonacci)
- Numerical methods (Newton-Raphson)

**Software Engineering:**
- File I/O and serialisation
- Input validation
- Error handling
- Modular design

## Usage

Each file is self-contained and can be run independently:

```bash
python eulerproject1.txt
python bubblesort.txt
python binarytree.txt
```

For visualisation tools:
```bash
# Requires matplotlib
pip install matplotlib
python big0.txt
# Enter: exponential, quadratic, logarithmic, or factorial
```

## Learning Outcomes

This collection demonstrates:
- **Problem decomposition** - Breaking complex problems into manageable parts
- **Algorithm selection** - Choosing appropriate approaches for different scenarios
- **Code optimisation** - Improving efficiency through better algorithms
- **Practical application** - Solving real-world problems with code

---

**Developed by Fardeen Idrus**

*A showcase of algorithmic thinking and problem-solving through practical implementation.*
