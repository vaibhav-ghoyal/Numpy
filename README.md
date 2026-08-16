# 🔢 Learn NumPy — A Practical Approach

> A complete, hands-on roadmap to master **NumPy**, the core library for numerical and scientific computing in Python. Every topic here is meant to be practiced with real code, not just read.

![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)
![Python](https://img.shields.io/badge/Python-3.9%2B-blue?style=for-the-badge&logo=python&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-In%20Progress-yellow?style=for-the-badge)

---

## 📌 About This Repository

This repository is a structured, topic-wise collection of **NumPy concepts explained with practical, runnable examples**. It's built for beginners who want to go from zero to confident with array-based computing, and for anyone preparing for Data Science, Machine Learning, or scientific computing roles.

Each folder/notebook focuses on **one topic**, includes:

- ✅ Concept explanation in simple words
- ✅ Practical code examples
- ✅ Common mistakes / gotchas
- ✅ Mini exercises to practice

---

## 🗂️ Table of Contents

1. [Getting Started](#-1-getting-started)
2. [NumPy Array Basics](#-2-numpy-array-basics)
3. [Array Creation Methods](#-3-array-creation-methods)
4. [Array Attributes & Data Types](#-4-array-attributes--data-types)
5. [Indexing & Slicing](#-5-indexing--slicing)
6. [Reshaping & Resizing Arrays](#-6-reshaping--resizing-arrays)
7. [Array Operations & Broadcasting](#-7-array-operations--broadcasting)
8. [Mathematical Functions](#-8-mathematical-functions)
9. [Aggregate & Statistical Functions](#-9-aggregate--statistical-functions)
10. [Sorting, Searching & Counting](#-10-sorting-searching--counting)
11. [Stacking, Splitting & Concatenation](#-11-stacking-splitting--concatenation)
12. [Copy vs View (Memory Concepts)](#-12-copy-vs-view-memory-concepts)
13. [Linear Algebra with NumPy](#-13-linear-algebra-with-numpy)
14. [Random Module (numpy.random)](#-14-random-module-numpyrandom)
15. [Working with Missing Data (NaN & Inf)](#-15-working-with-missing-data-nan--inf)
16. [Boolean Masking & Fancy Indexing](#-16-boolean-masking--fancy-indexing)
17. [Vectorization & Performance](#-17-vectorization--performance)
18. [File I/O with NumPy](#-18-file-io-with-numpy)
19. [Structured Arrays](#-19-structured-arrays)
20. [NumPy with Pandas / Matplotlib](#-20-numpy-with-pandas--matplotlib)
21. [Mini Projects](#-21-mini-projects)
22. [Interview Questions & Cheatsheet](#-22-interview-questions--cheatsheet)
23. [Resources](#-23-resources)

---

## 🟢 1. Getting Started

- What is NumPy and why it's faster than Python lists
- Installing NumPy (`pip install numpy`)
- Importing convention: `import numpy as np`
- NumPy vs Python Lists — performance comparison
- Understanding `ndarray` — the core object

```python
import numpy as np

arr = np.array([1, 2, 3, 4, 5])
print(arr, type(arr))
```

---

## 🟢 2. NumPy Array Basics

- Creating 1D, 2D, and 3D arrays
- Understanding axis (axis=0, axis=1)
- Array vs Matrix vs Vector
- `ndim`, `shape`, `size`, `dtype`

---

## 🟢 3. Array Creation Methods

- `np.array()`
- `np.zeros()`, `np.ones()`, `np.full()`
- `np.arange()`, `np.linspace()`
- `np.eye()`, `np.identity()`
- `np.empty()`
- Random array creation basics

---

## 🟢 4. Array Attributes & Data Types

- `.dtype`, `.itemsize`, `.nbytes`
- Type casting with `.astype()`
- Understanding int8, int32, float64, bool, complex
- Choosing correct dtype for memory optimization

---

## 🟢 5. Indexing & Slicing

- 1D and 2D indexing
- Negative indexing
- Slicing syntax `[start:stop:step]`
- Slicing multi-dimensional arrays
- Difference between slicing a list vs an array

---

## 🟢 6. Reshaping & Resizing Arrays

- `.reshape()`
- `.flatten()` vs `.ravel()`
- `.resize()`
- Transpose using `.T` and `np.transpose()`
- `np.newaxis` and `np.expand_dims()`

---

## 🟢 7. Array Operations & Broadcasting

- Element-wise arithmetic operations
- Scalar operations
- What is Broadcasting and its rules
- Common broadcasting errors and how to fix them

```python
a = np.array([1, 2, 3])
b = np.array([[1], [2], [3]])
print(a + b)  # Broadcasting example
```

---

## 🟢 8. Mathematical Functions

- Trigonometric: `np.sin()`, `np.cos()`, `np.tan()`
- Exponential & Logarithmic: `np.exp()`, `np.log()`, `np.log10()`
- Power & Roots: `np.power()`, `np.sqrt()`
- Rounding: `np.round()`, `np.floor()`, `np.ceil()`

---

## 🟢 9. Aggregate & Statistical Functions

- `np.sum()`, `np.mean()`, `np.median()`
- `np.std()`, `np.var()`
- `np.min()`, `np.max()`, `np.argmin()`, `np.argmax()`
- Aggregations along specific axis

---

## 🟢 10. Sorting, Searching & Counting

- `np.sort()`, `np.argsort()`
- `np.where()`, `np.searchsorted()`
- `np.count_nonzero()`
- `np.unique()`

---

## 🟢 11. Stacking, Splitting & Concatenation

- `np.concatenate()`
- `np.vstack()`, `np.hstack()`, `np.dstack()`
- `np.split()`, `np.hsplit()`, `np.vsplit()`

---

## 🟢 12. Copy vs View (Memory Concepts)

- Shallow copy vs Deep copy
- `.copy()` vs `.view()`
- Why modifying a slice affects the original array
- Checking with `.base`

---

## 🟢 13. Linear Algebra with NumPy

- Matrix multiplication: `np.dot()`, `@` operator
- `np.linalg.inv()`, `np.linalg.det()`
- Eigenvalues & Eigenvectors: `np.linalg.eig()`
- Solving linear equations: `np.linalg.solve()`
- Identity & Transpose matrices

---

## 🟢 14. Random Module (numpy.random)

- `np.random.rand()`, `np.random.randn()`
- `np.random.randint()`
- `np.random.seed()` for reproducibility
- `np.random.choice()`, `np.random.shuffle()`
- Generating random datasets for practice

---

## 🟢 15. Working with Missing Data (NaN & Inf)

- Understanding `np.nan` and `np.inf`
- `np.isnan()`, `np.isinf()`
- Handling NaN in calculations
- `np.nan_to_num()`

---

## 🟢 16. Boolean Masking & Fancy Indexing

- Conditional filtering: `arr[arr > 5]`
- Combining conditions with `&`, `|`
- Fancy indexing with index arrays
- Replacing values conditionally with `np.where()`

---

## 🟢 17. Vectorization & Performance

- Why loops are slow in Python
- Vectorized operations vs `for` loops (benchmark comparison)
- `np.vectorize()`
- Memory layout: C-order vs Fortran-order

---

## 🟢 18. File I/O with NumPy

- Saving/loading arrays: `np.save()`, `np.load()`
- Working with `.npy` and `.npz` files
- `np.savetxt()`, `np.loadtxt()`
- Reading CSV data into NumPy arrays

---

## 🟢 19. Structured Arrays

- Creating arrays with mixed data types
- Defining custom `dtype`
- Accessing structured array fields

---

## 🟢 20. NumPy with Pandas / Matplotlib

- Converting NumPy arrays to Pandas DataFrames
- Using NumPy arrays for plotting with Matplotlib
- Why NumPy is the foundation of the Python Data Science stack

---

## 🟢 21. Mini Projects

Practical projects to apply everything learned:

- 📊 Student Marks Analyzer (mean, median, top scorer)
- 🎲 Dice Roll Simulator using `np.random`
- 🖼️ Image manipulation using NumPy arrays (grayscale, crop, flip)
- 📈 Simple Linear Regression using only NumPy
- 🧮 Matrix Calculator (Add, Subtract, Multiply, Inverse)
- 🌡️ Weather Data Analysis using NumPy arrays

---

## 🟢 22. Interview Questions & Cheatsheet

- Most commonly asked NumPy interview questions
- Quick-reference cheatsheet (PDF/Markdown)
- Common errors and their fixes

---

## 📚 23. Resources

- [Official NumPy Documentation](https://numpy.org/doc/)
- [NumPy GitHub Repository](https://github.com/numpy/numpy)
- Recommended books & practice platforms

---

## 🛠️ How to Use This Repository

```bash
# Clone the repository
git clone https://github.com/vaibhav-ghoyal/Numpy.git

# Navigate into the folder
cd Numpy

# Install requirements
pip install -r requirements.txt

# Open notebooks and start practicing!
jupyter notebook
```

---

## ⭐ Support

If this repository helped you learn NumPy, consider giving it a **star ⭐** — it motivates further improvements and helps others discover it too.

---

<p align="center">Made with ❤️ for everyone learning Data Science & Numerical Computing in Python</p>
