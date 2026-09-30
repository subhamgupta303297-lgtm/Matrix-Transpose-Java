# Matrix Transpose in Java 🔄

A clean, robust implementation for calculating and displaying the transpose of any $N \times M$ matrix in Java.

---

## 📌 Problem Description
Given a 2D matrix of dimensions $N \times M$ ($N$ rows and $M$ columns), compute its transpose such that rows become columns and columns become rows, resulting in an $M \times N$ matrix.

---

## 💡 Logic & Mathematical Mapping

The transformation maps every element located at position `(i, j)` in the original matrix to position `(j, i)` in the transposed matrix:

$$\text{transpose}[j][i] = \text{matrix}[i][j]$$

### Key Observations:
- **Dimension Inversion:** The resulting matrix must be declared with dimensions `[m][n]` instead of `[n][m]`.
- **Index Bounds Safety:** To prevent `ArrayIndexOutOfBoundsException` during coordinate swapping, the outer loop iterates over $N$ and the inner loop iterates over $M$, mapping directly to the target indices `[j][i]`.

---

## ⚙️ How to Compile & Run

```bash
# Compile the program
javac MatrixTranspose.java

# Run the program
java MatrixTranspose
