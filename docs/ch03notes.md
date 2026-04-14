# Chapter 3 Linear Maps

## Section 3A Vector Space of Linear Maps

## Section 3B Null Spaces and Ranges

## Section 3C Matrices

### 3.31 definition: matrix of a linear map, $ℳ(𝑇)$

Suppose $𝑇 ∈ ℒ(𝑉, 𝑊)$ and $v_1, \cdots, v_n$ is a basis of $𝑉$ and $w_1, \cdots, w_m$ is a basis of $𝑊$.

The matrix of $𝑇$ with respect to these bases is the $𝑚$-by-$𝑛$ 
matrix $ℳ(𝑇)$ whose entries $A_{i, j}$ are defined by
$$
𝑇𝑣_𝑘 = A_{1, k} w_1 + \cdots + A_{m, k} w_m \\
$$

### 3.35 matrix of the sum of linear maps

Suppose $S, T \in \mathcal{L}(V, W).$ Then
$\mathcal{M}(S+T) = \mathcal{M}(S) + \mathcal{M}(T)$.

**Proof**:

Assume $\mathcal{M}(S) = [A_{i, j}], \mathcal{M}(T) = [B_{i, j}]$.

$$ 
Tv_k = A_{1, k} w_1 + \cdots + A_{m, k} w_m \\
Sv_k = B_{1, k} w_1 + \cdots + B_{m, k} w_m \\
(T+S)v_k = Tv_k + Sv_k \\
=(A_{1, k} w_1 + \cdots + A_{m, k} w_m) + \\
(B_{1, k} w_1 + \cdots + B_{m, k} w_m) \\
= (A_{1, k}+B_{1, k}) w_1 + \cdots + (A_{m, k}+B_{m, k}) w_m
$$

So $\mathcal{M}(S+T) = [A_{i, j} + B_{i, j}] = [A_{i, j}] + [B_{i, j}] = \mathcal{M}(S) + \mathcal{M}(T)$.

$\square$

### 3.38 the matrix of a scalar times a linear map

Suppose $𝜆 ∈ 𝐅$ and $𝑇 ∈ ℒ(𝑉, 𝑊)$. Then $ℳ(𝜆𝑇) = 𝜆ℳ(𝑇)$.

**Proof**:

Assume $\mathcal{M}(T) = [A_{i, j}]$, then

$$
(𝜆T)(v_k) = 𝜆(Tv_k) \\
= 𝜆 (A_{1, k} w_1 + \cdots + A_{m, k} w_m) \\
= (𝜆A_{1, k}) w_1 + (𝜆A_{m, k}) w_m \\
$$

So

$$ 
\mathcal{M}(𝜆T) = [𝜆 A_{i, j}] = 𝜆 [A_{i, j}] = 𝜆 \mathcal{M}(T)
$$

$\square$

### 3.44 notation: $𝐴_{𝑗,⋅}$ , $𝐴_{⋅,𝑘}$

Suppose $𝐴$ is an $𝑚$-by-$𝑛$ matrix.

* If $1 ≤ 𝑗 ≤ 𝑚$, then $A_{j, .}$ 
denotes the $1$-by-$𝑛$ matrix consisting of row $𝑗$ of $𝐴$.

* If $1 ≤ 𝑘 ≤ 𝑛$, then $A_{., k}$ denotes the $𝑚$-by-$1$ matrix consisting of column $𝑘$ of $𝐴$.

### 3.50 linear combination of columns

Suppose $𝐴$ is an $𝑚$-by-$𝑛$ matrix and
$b = \begin{pmatrix}
b_1 \\
\vdots  \\
b_n \\
\end{pmatrix}
$ is an 𝑛-by-1 matrix. Then

$$ 
Ab = b_1 A_{., 1}  + \cdots + b_n A_{., n} 
$$

In other words, 𝐴𝑏 is a linear combination of the columns of 𝐴, 
with the scalars that multiply the columns coming from 𝑏.

**Proof**:

The $k$th row on the left is

$$ 
Ab_{k, 1} = A_{1, k} b_1 + \cdots + A_{n, k} b_n
$$

Which is the same as the $k$th row on the right.

$\square$

### 3.56 column–row factorization

Suppose $𝐴$ is an $𝑚$-by-$𝑛$ matrix with entries in $𝐅$ and 
column rank $𝑐 ≥ 1$. Then
there exist an $𝑚$-by-$𝑐$ matrix $𝐶$ and a $𝑐$-by-$𝑛$ matrix $𝑅$, both with entries in $𝐅$, such that $𝐴 = 𝐶𝑅$.

**Proof**:

The column $A_{., 1}, \cdots, A_{., n}$ can be reduced $c$ columns
which is a basis of the span of the columns of $A$.
Put these $c$ columns together to make $C$.

Each columns of $A$ is the linear combination of the columns of $C$.
Then make the coefficients into column of $R$.

Then $A = CR$.

### 3.57 column rank equals row rank

Suppose $𝐴 ∈ 𝐅^{𝑚, 𝑛}$ . Then the column rank of 𝐴 equals the row rank of 𝐴.

**Proof**: Assume column rank is $c$, then $A = CR$.
$C$ is $m \times c$ and $R$ is $c \times n$.

Each row of $A$ is the linear combination of the row of $R$,
so row rank of $A \leq c$.

To prove the other direction, consider $A^T$, 

$$ 
\text{ column rank of } 𝐴 = \\
\text{ row rank of } 𝐴t ≤ \\
\text{ column rank of } 𝐴t = \\
\text{ row rank of } 𝐴.
$$

So column rank and row rank are equal.

$\square$

## Section 3E Duality

### 3.108 definition: linear functional

A linear functional on $𝑉$ is a linear map from $𝑉$ to $𝐅$.
In other words, a linear functional is an element of
$ℒ(𝑉, 𝐅)$.

### 3.109 example: linear functionals

* Define 𝜑 ∶ 𝒫(𝐑) → 𝐑 by

$$ 
\varphi(𝑝) = 3𝑝″ (5) + 7𝑝(4).
$$

Then 𝜑 is a linear functional on 𝒫(𝐑).

* Define 𝜑 ∶ 𝒫(𝐑) → 𝐑 by

$$ 
\varphi(p) = \int_{0}^{1} p
$$

for each 𝑝 ∈ 𝒫(𝐑). Then 𝜑 is a linear functional on 𝒫(𝐑).

### 3.110 definition: dual space, 𝑉′

The dual space of 𝑉, denoted by 𝑉′, is the vector space of all linear 
functionals on 𝑉. In other words, 𝑉′ = ℒ(𝑉, 𝐅).

### 3.111 dim 𝑉′ = dim 𝑉

Suppose $𝑉$ is finite-dimensional. Then $𝑉′$ is also finite-dimensional and

$$ 
\dim V' = \dim V
$$

**Proof**:

$$ 
\dim V' = \dim V \times \dim F = \dim V
$$

$\square$
