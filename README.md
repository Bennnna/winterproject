# Winter Project

This repository is a placeholder for upcoming winter project work. It can be used to track experiments, notes, and code related to the project.

## Getting Started
- Add project files and documentation as the work progresses.
- Use version control best practices for committing and reviewing changes.

## Machine Learning Practice Solutions

Worked examples are collected here so they are easy to read and reuse.

### Problem 1: Solve \(Ax = b\) with an LU factorization
Given
\[
A = \begin{bmatrix}1 & 4 & 3 \\ 2 & 1 & 3 \\ 0 & 2 & 3\end{bmatrix},\quad
b = \begin{bmatrix}-2 \\ -8 \\ 2\end{bmatrix},\quad
L = \begin{bmatrix}1 & 0 & 0 \\ 2 & 1 & 0 \\ 0 & -5 & 1\end{bmatrix},\quad
U = \begin{bmatrix}1 & 4 & 3 \\ 0 & -7 & -3 \\ 0 & 0 & -12\end{bmatrix}.
\]

1. **Forward substitution (solve \(Ly = b\)).**
   \[
   y = \begin{bmatrix}-2 \\ -4 \\ -18\end{bmatrix}.
   \]
2. **Back substitution (solve \(Ux = y\)).**
   \[
   x = \begin{bmatrix}-\tfrac{87}{14} \\ -\tfrac{1}{14} \\ \tfrac{3}{2}\end{bmatrix}.
   \]

### Problem 2: Project a vector onto another vector
For \(x_1 = [1, 5]\) projected onto \(a = [4, 3]\), compute the scalar weight
\[
\frac{x_1 \cdot a}{a \cdot a} = \frac{1\cdot4 + 5\cdot3}{4^2 + 3^2} = \frac{19}{25}.
\]
The projection is therefore
\[
\operatorname{proj}_a(x_1) = \frac{19}{25} [4, 3] = \left[\tfrac{76}{25}, \tfrac{57}{25}\right].
\]

### Problem 3: Rotate a vector by 30° counterclockwise
Using the 2D rotation matrix, rotate \(x = [1, 1]^T\):
\[
R_{30^\circ} = \begin{bmatrix}\cos 30^\circ & -\sin 30^\circ \\ \sin 30^\circ & \cos 30^\circ\end{bmatrix},\quad
x' = R_{30^\circ} x = \left[\tfrac{\sqrt{3}-1}{2}, \tfrac{\sqrt{3}+1}{2}\right].
\]
