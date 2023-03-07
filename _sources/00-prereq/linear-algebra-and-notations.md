# Linear algebra and notations

This section introduces the basic concepts of linear algebra and notations used in this course. The concepts are introduced in a self-contained manner, and you can skip this section if you are already familiar with the concepts.

## Scalars, vectors, and matrices

- Scalars: a scalar is a single number. In this course, if not specified, scalars are denoted by lowercase letters, e.g. $x = 3.14$. When introducing a scalar, we will specify its type, e.g. $x \in \mathbb{R}$, where $\mathbb{R}$ is the set of real numbers.
- Vectors: a vector is an array of numbers, which are arranged in order. Usually we denote vectors as lowercase letters in bold, e.g.

  $$
    \mathbf{x} = \left[ \begin{array}{c c c c c} x_1 , x_2 , \dots , x_n \end{array}\right]^\top,
  $$

  where the superscript $^\top$ denotes a common vector/matrix operation called transpose, which flips the row and column, e.g. $\begin{bmatrix} x_1 \\ x_2 \end{bmatrix}^\top = \begin{bmatrix} x_1, x_2 \end{bmatrix}$, and $\begin{bmatrix} x_1, x_2 \end{bmatrix}^\top = \begin{bmatrix} x_1 \\ x_2 \end{bmatrix}$. The elements of a vector can be accessed by their index, and denoted as a scalar with a subscript, e.g. $x_1$ is the first element of $\mathbf{x}$. We can also index a set of elements of a vector. For example, we can define the set $ S = \{2, 4\} $ and then access the 2nd and 4th elements of $\mathbf{x}$ by $S$, i.e. $\mathbf{x}_S = \begin{bmatrix} x_2, x_4 \end{bmatrix}^\top $. We can also index a set of elements of a vector by a boolean array, e.g. $\mathbf{x}_{\mathbf{b}} = \begin{bmatrix} x_1, x_3 \end{bmatrix}^\top $, where $\mathbf{b} = \begin{bmatrix} \text{True}, \text{False}, \text{True}, \dots, \text{False} \end{bmatrix}^\top $. When introducing a vector, we can specify its type, e.g. if each element in $\mathbf{x}$ is in $\mathbb{R}$, we can specify it as $\mathbf{x} \in \mathbb{R}^n$, where $\mathbb{R}^n$ is the set of $n$-dimensional real vectors.

<!-- Sometimes we need to index the elements of a vector by their position, e.g. $x_1$ is the first element of $\mathbf{x}$, $x_2$ is the second element of $\mathbf{x}$, and so on. In this case, we can use the following notations: -->

- Matrices: a matrix is a 2D array of numbers. Typically we denote matrices as uppercase letters in bold, e.g.

  <!-- $$
    \mathbf{X} = \begin{bmatrix} x_{1,1} & x_{1,2} & x_{1,3} \\ x_{2,1} & x_{2,2} & x_{2,3} \end{bmatrix}.
  $$  -->
  $$
    \mathbf{X} = \begin{bmatrix} x_{1,1} & x_{1,2}, & x_{1,3} \\ x_{2,1} & x_{2,2} & x_{2,3} \end{bmatrix}.
  $$

  If a real valued matrix $\mathbf{X}$ has $m$ rows and $n$ columns, we can specify it as $\mathbf{X} \in \mathbb{R}^{m \times n}$. We usually identify an element of a matrix as a scalar with its row and column indices, e.g. $x_{2,3}$ is the element in the 2nd row and 3rd column of $\mathbf{X}$. We can also access an entire row of a matrix by writing ":" for the coordinate of columns, e.g. $\mathbf{x}_{2, :}$ is the 2nd row of $\mathbf{X}$. We can also access columns of a matrix in the same way, e.g.,  $\mathbf{x}_{:,3}$ is the 3rd column of $\mathbf{X}$. The transpose of a matrix flips the rows and columns along the diagonal, e.g.

   $$
    \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix}^\top = \begin{bmatrix} 1 & 3 \\ 2 & 4 \end{bmatrix}.
   $$

<!-- We can also index a set of elements of a matrix. For example, we can define the set $ S = {2, 4} $ and then access the 2nd and 4th rows of $\mathbf{X}$ by $S$, i.e. $\mathbf{X}_S = \begin{bmatrix} x_{2,1} & x_{2,2} & x_{2,3} \\ x_{4,1} & x_{4,2} & x_{4,3} \end{bmatrix}$. We can also index a set of elements of a matrix by a boolean array, e.g. $\mathbf{X}_{\mathbf{b}} = \begin{bmatrix} x_{1,1} & x_{1,2} & x_{1,3} \\ x_{3,1} & x_{3,2} & x_{3,3} \end{bmatrix}$, where $\mathbf{b} = \begin{bmatrix} True \\ False \\ True \\ \vdots\\ False \end{bmatrix}$.  -->

<!-- - Tensors: a tensor is an array of numbers arranged on a regular grid with a variable number of axes, e.g. $$\mathbf{X} = \begin{bmatrix} x_{1,1,1} & x_{1,1,2} & x_{1,1,3} \\ x_{1,2,1} & x_{1,2,2} & x_{1,2,3} \\ x_{1,3,1} & x_{1,3,2} & x_{1,3,3} \end{bmatrix}.$$ -->

## Operations on matrices

- A matrix $\mathbf{X}$ can be multiplied by a scalar $\alpha$ or add a scalar to a matrix:

  $$
    (\alpha\mathbf{X})_{i, j}  =  \alpha x_{i,j}, \text{ and } (\mathbf{X} + \alpha)_{i, j}  =  x_{i,j} + \alpha.
  $$

- Addition and subtraction: we can add or subtract two matrices with the same shape. The result is that all corresponding entries are added, i.e.

  $$
    (\mathbf{X} + \mathbf{Y})_{i, j} = x_{i, j} + y_{i, j}.
  $$

- Matrix multiplication: If the number of columns of matrix $\mathbf{X}$ is equal to the number of rows of matrix $\mathbf{Y}$, the matrices can be multiplied in the order $\mathbf{X}$, $\mathbf{Y}$. The result will be a new matrix $\mathbf{XY}$, that has the same number of rows as $\mathbf{X}$ and the same number of columns as $\mathbf{Y}$. The entries $\mathbf({XY})_{i,j}$ will be the following combination of the entries of row $i$ of $\mathbf{X}$ and column $j$ of $\mathbf{Y}$, i.e.

  $$
    (\mathbf{XY})_{i,j} = \sum_{k=1}^n x_{i,k} y_{k,j}.
  $$

- Element-wise multiplication: we can also multiply two matrices with the same shape element-wise, i.e.

  $$
    (\mathbf{X} \odot \mathbf{Y})_{i, j} = x_{i, j} y_{i, j},
  $$

  where $\odot$ is the symbol for element-wise multiplication, and $\mathbf{X} \odot \mathbf{Y}$ is also called the Hadamard product of $\mathbf{X}$ and $\mathbf{Y}$.


**Examples**

- The multiplication of a number and a matrix

  $$
    2  \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} = \begin{bmatrix} 2 \times 1 & 2 \times 2 \\ 2 \times 3 & 2 \times 4 \end{bmatrix} = \begin{bmatrix} 2 & 4 \\ 6 & 8 \end{bmatrix}.
  $$

- The sum of two matrices of the same shape

  $$
    \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} + \begin{bmatrix} 5 & 6 \\ 7 & 8 \end{bmatrix} = \begin{bmatrix} 1 + 5 & 2 + 6 \\ 3 + 7 & 4 + 8 \end{bmatrix} = \begin{bmatrix} 6 & 8 \\ 10 & 12 \end{bmatrix}.
  $$

- The multiplication of two matrices:

  $$
    \begin{bmatrix} 1 & 2 \\ 3 & 4 \end{bmatrix} \begin{bmatrix} 5 & 6 & 7 \\ 8 & 9 & 10 \end{bmatrix} = \begin{bmatrix} 1 \times 5 + 2 \times 8 & 1 \times 6 + 2 \times 9 & 1 \times 7 + 2 \times 10 \\ 3 \times 5 + 4 \times 8 & 3 \times 6 + 4 \times 9 & 3 \times 7 + 4 \times 10 \end{bmatrix} = \begin{bmatrix} 21 & 24 & 27 \\ 47 & 54 & 61 \end{bmatrix}.
  $$


**Some properties of matrix multiplication:**

- $(\mathbf{X}^\top)^\top = \mathbf{X}$.
- $(\mathbf{X} \mathbf{Y})^\top = \mathbf{Y}^\top \mathbf{X}^\top$.
- $(\mathbf{X} + \mathbf{Y})^\top = \mathbf{X}^\top + \mathbf{Y}^\top$.
- $\mathbf{X} \mathbf{I} = \mathbf{I} \mathbf{X} = \mathbf{X}$, where $\mathbf{I}$ is the identity matrix.
- $\mathbf{X} \mathbf{Y} = \mathbf{Y} \mathbf{X}$ if $\mathbf{X}$ and $\mathbf{Y}$ are square matrices.
- $(\alpha \mathbf{X}) \mathbf{Y} = \alpha (\mathbf{X} \mathbf{Y})$.
- $\mathbf{X} (\mathbf{Y} \mathbf{Z}) = (\mathbf{X} \mathbf{Y}) \mathbf{Z}$.
- $\mathbf{X} (\mathbf{Y} + \mathbf{Z}) = \mathbf{X} \mathbf{Y} + \mathbf{X} \mathbf{Z}$.


## Special matrices

- **Diagonal** matrices contain non-zero elements only on the diagonal, i.e. $x_{i,j} = 0$ for $i \neq j$. For example, the following matrix is a diagonal matrix:

  $$
    \begin{bmatrix} 1 & 0 & 0 \\ 0 & 2 & 0 \\ 0 & 0 & 3 \end{bmatrix}.
  $$

  All diagonal matrices are square.

- **Identity** matrices are special diagonal matrices with ones on the diagonal (and zeros elsewhere), i.e. $x_{i,j} = 1$ for $i = j$ and $x_{i,j} = 0$ for $i \neq j$. For example, the following matrix is an identity matrix:

  $$
    \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}.
  $$

- **Symmetric** matrices are square matrices that are equal to their transpose, i.e. $\mathbf{X} = \mathbf{X}^\top$, or $\mathbf{X}_{i,j} = \mathbf{X}_{j, i}$. For example, the following matrix is a symmetric matrix:

  $$
    \begin{bmatrix} 1 & 2 & 3 \\ 2 & 4 & 5 \\ 3 & 5 & 6 \end{bmatrix}.
  $$

- **Invertible** matrices are square matrices that can be multiplied with another matrix to yield the identity matrix. The inverse matrix of a matrix $\mathbf{X}$ is denoted as $\mathbf{X}^{-1}$, and according to the definition $\mathbf{X} \mathbf{X}^{-1} = \mathbf{X}^{-1} \mathbf{X} = \mathbf{I}$. The inverse matrix of an identity matrix is itself, e.g.

  $$
    \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}^{-1} = \begin{bmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & 1 \end{bmatrix}.
  $$

- An **Orthogonal** matrix is a square matrix whose columns are mutually orthogonal and have unit length, i.e. $\mathbf{X}^\top \mathbf{X} = \mathbf{X} \mathbf{X}^\top = \mathbf{I}$, where $\mathbf{I}$ is the identity matrix.

## Exercises

**1**. $\begin{bmatrix} 12 & 0 & 0 \\ 0 & 8 & 0 \\ 0 & 0 & 23 \end{bmatrix}$

    What kind of matrices is it? There can be multiple answers.

        a. Diagonal

        b. Identity

        c. Symmetric

        d. Invertible

        e. Orthogonal



*Compare your answer with the solution below*
   ```{toggle}
    **a , c, d.**

    **The given matrix has values only in the diagonal; that's why it's a diagonal matrix. The diagonal values are not 1, so it's not an identity matrix. If you transpose the given matrix, it will equal the given matrix, so it's symmetric. A diagonal matrix without any zero on its diagonal is always invertible, so this is an invertible matrix. For the orthogonal matrix $XX^T=I$, which is not valid for our given matrix, so it's not an orthogonal matrix.**
   ```

**2**. **$A$** = $\begin{bmatrix} 8 & 5 & 9 \\ 7 & 19 & 14 \end{bmatrix}$;
   **$B$** = $ \begin{bmatrix} 6 & 13 & 15 \\ 17 & 22 & 12 \\ 0 & 3 & 9 \end{bmatrix}$

Calculate the following matrix operations by hand.

  i. $AB$= ?

  ii. $2A$ = ?

  iii. $AB + 2A$ = ?


*Compare your answer with the reference solution below*
   ```{toggle}
    i. $\begin{bmatrix} 133 & 241 & 261 \\ 365 & 551 & 459 \end{bmatrix}$

    ii. $\begin{bmatrix} 16 & 10 & 18 \\ 14 & 38 & 28 \end{bmatrix}$

    iii. $\begin{bmatrix} 149 & 251 & 279 \\ 379 & 589 & 487 \end{bmatrix}$

   ```
