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

## Section 3F Duality

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

### 3.127 condition for the annihilator to equal {0} or the whole space

Suppose $𝑉$ is finite-dimensional and $𝑈$ is a subspace of $𝑉$. Then

(a) $U^0 = \{0\} \Longleftrightarrow U = V$

**Proof**:

$$ 
\begin{align*}
U^0 = \{0\}
&\Longleftrightarrow \dim U^0 = 0 \\
&\Longleftrightarrow \dim V - \dim U = 0
&\text{ (3.125 dimension of the annihilator) }\\
&\Longleftrightarrow V = U &\text{ (2.39) }\\
\end{align*} 
$$

$\square$

(b) $U^0 = V' \Longleftrightarrow U = 0$ 

**Proof**:

$$ 
\begin{align*}
U^0 = V'
&\Longleftrightarrow \dim U^0 = \dim V'
&\text{ (2.39) } \\
&\Longleftrightarrow \dim U^0 = \dim V
&\text{ (3.111) }\\
&\Longleftrightarrow U = 0
&\text{ (3.125) }\\
\end{align*} 
$$

$\square$

### 3.128 the null space of 𝑇′

Suppose 𝑉 and 𝑊 are finite-dimensional and 𝑇 ∈ ℒ(𝑉, 𝑊). Then

(a) $\text{null } T' = (\text{range } T)^0$

**Proof**:

If $\psi \in \text{null } T'$, then $T'(\psi ) = 0$.
Also

$$ 
(T'(\psi))(v) = (\psi \circ T)(v) = \psi (T(v)) = 0
$$

So $\psi \in (\text{range } T)^0$.

If $\psi \in (\text{range } T)^0$, then $\psi (T(v)) = 0$, then
$(T'(\psi))(v) = 0, \forall v.$ So $T'(\psi) = 0$.

So $\psi \in \text{null } T'$.

$\square$

(b) $\dim \text{null } 𝑇' = \dim \text{null } 𝑇 + \dim 𝑊 − \dim 𝑉 .$

**Proof**:

$$ 
\begin{align*}
\dim \text{null } 𝑇'
&= \dim (\text{range } T)^0 &\text{ (part (a)) }\\
&= \dim W - \dim \text{range } T &\text{ (3.125) }\\
&= \dim W - (\dim V - \text{dim null } T) &\text{ (3.21) }\\
&= \dim \text{null } 𝑇 + \dim 𝑊 − \dim 𝑉
\end{align*} 
$$

$\square$

### 3.129 𝑇 surjective is equivalent to 𝑇' injective

Suppose 𝑉 and 𝑊 are finite-dimensional and 𝑇 ∈ ℒ(𝑉, 𝑊). Then

$$ 
𝑇 \text{ is surjective} ⟺ 𝑇' \text{ is injective}.
$$

**Proof**:

$$
\begin{align*}
𝑇 \text{ is surjective}
&\Longleftrightarrow \text{range } T = W \\
&\Longleftrightarrow (\text{range } T)^0 = \{0\}
&\text{ (3.127 (a))} \\
&\Longleftrightarrow \text{null } T' = \{0\}
&\text{ (3.128 (a))} \\
&\Longleftrightarrow
𝑇' \text{ is injective}
\end{align*} 
$$

$\square$

### 3.130 the range of $𝑇'$

Suppose $𝑉$ and $𝑊$ are finite-dimensional and $𝑇 ∈ ℒ(𝑉, 𝑊)$. Then

(a) $\text{dim range } T = \text{dim range } T'$;

**Proof**:

$$ 
\text{dim range } T' = \dim W - \text{dim null } T' \\
= \dim W - (\text{dim null } T + \dim W − \dim V) \\
= \dim V - \text{dim null }  T \\
= \text{dim range } T
$$

Another way

$$
\begin{align*}
\text{dim range } T' &= \dim W' - \text{dim null } T' &\text{ (fundamental theorem of linear maps) } \\
&= \dim W' - \dim (\text{range } T)^0 &\text{ (3.128 (a)) }\\
&= \dim W - \dim (\text{range } T)^0 &\text{ (3.11) }\\
&= \dim W - (\dim W - \dim (\text{range } T) ) &\text{ (3.125 dimension of the annihilator) }\\
&= \dim (\text{range } T)
\end{align*} 
$$

(b) $\text{range } T' = (\text{null } T)^0$

**Proof**:

We first prove $\text{range } T' \subseteq (\text{null } T)^0$.

Assume $\varphi \in \text{range } T'$, then we can find $\psi \in W'$,
such that $T'(\psi) = \varphi$.

Then if $u \in \text{null } T$ 

$$ 
\varphi (u) = (T'(\psi))(u) = (\psi \circ T)(u)
= \psi (T(u)) = 0
$$

So $\varphi(u) = 0, \varphi \in (\text{null } T)^0$.

Next, we compute this

$$ 
\begin{align*}
\text{dim range } T'
&= \text{dim range } T & \text{(part a)} \\
&= \dim T - \text{dim null } T &\text{ (3.21 fundamental theorem of linear maps) } \\
&= \dim (\text{null } T)^0 &\text{(3.125 dimension of the annihilator)} \\
\end{align*} 
$$

### 3.131 $𝑇$ injective is equivalent to $𝑇'$ surjective

Suppose $𝑉$ and $𝑊$ are finite-dimensional and $𝑇 ∈ ℒ(𝑉, 𝑊)$. Then

$$ 
T \text{ is injective }
\Longleftrightarrow
T' \text{ is surjective }
$$

**Proof**:

$$
\begin{align*}
T \text{ is injective }
&\Longleftrightarrow
\text{null } T = \{0\}\\
&\Longleftrightarrow
(\text{null } T)^0 = V' &\text{ (3.127 (b)) }\\
&\Longleftrightarrow
\text{range } T' = V'  &\text{ (3.130 (b)) }\\
&\Longleftrightarrow
T' \text{ is surjective } \\
\end{align*} 
$$

$\square$
