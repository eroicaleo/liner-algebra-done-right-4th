# Chapter 2 Finite-Dimensional Vector Spaces

## 2A Span and Linear Independence

### 2A.8

Suppose $𝑣_1, 𝑣_2, 𝑣_3, 𝑣_4$ is linearly independent in $𝑉$. Prove that the list

$$ 
𝑣_1 − 𝑣_2, 𝑣_2 − 𝑣_3, 𝑣_3 − 𝑣_4, 𝑣_4
$$

is also linearly independent.

**Proof**:

We have

$$ 
a_1 (𝑣_1 − 𝑣_2) + a_2 (𝑣_2 − 𝑣_3) + a_3 (𝑣_3 − 𝑣_4) + a_4 𝑣_4 = 0 \\
\Longleftrightarrow \\
a_1 𝑣_1 + (a_2 - a_1) 𝑣_2 + (a_3 - a_2) 𝑣_3 + (a_3 - a_4) 𝑣_4 = 0 \\
\Longleftrightarrow \\
a_1 = a_2 - a_1 = a_3 - a_2 = a_4 - a_3 = 0 \\
\Longleftrightarrow \\
a_1 = a_2 = a_3 = a_4 = 0
$$

$\square$

### 2A.9

Prove or give a counterexample: If
$𝑣_1, 𝑣_2, …, 𝑣_𝑚$ is a linearly independent
list of vectors in $𝑉$, then

$$ 
5𝑣_1 − 4𝑣_2, 𝑣_2, 𝑣_3, …, 𝑣_𝑚
$$

is linearly independent.

**Proof**:

$$ 
a_1 (5𝑣_1 − 4𝑣_2) + a_2 𝑣_2 + a_3 𝑣_3 + \cdots + a_m 𝑣_m = 0 \\
\Longleftrightarrow \\
5 a_1 = a_2 - 4 a_1 = a_3 = \cdots = a_m = 0 \\ 
\Longleftrightarrow \\
a_1 = a_2 = a_3 = \cdots = a_m = 0
$$

$\square$

### 2A.10

Prove or give a counterexample:
If $𝑣_1, 𝑣_2, …, 𝑣_𝑚$ is a linearly independent
list of vectors in $𝑉$ and $𝜆 ∈ 𝐅$ with $𝜆 ≠ 0$, then
$𝜆𝑣_1, 𝜆𝑣_2, …, 𝜆𝑣_𝑚$ is linearly independent.

**Proof**:

$$ 
a_1 (𝜆𝑣_1) + a_2 (𝜆𝑣_1) + \cdots + a_m (𝜆𝑣_m) = 0 \\
\Longleftrightarrow \\
(a_1𝜆) 𝑣_1 + (a_2𝜆) 𝑣_2 + \cdots + (a_m𝜆) 𝑣_m = 0 \\
\Longleftrightarrow \\
a_1𝜆 = a_2𝜆 = \cdots = a_m𝜆 = 0 \\
\Longleftrightarrow \\
a_1 = a_2 = \cdots = a_m = 0 \\
$$

$\square$

### 2A.11

Prove or give a counterexample: If
$𝑣_1, …, 𝑣_𝑚$ and $𝑤_1, …, 𝑤_𝑚$ are linearly
independent lists of vectors in $𝑉$ , then the list
$𝑣_1 + 𝑤_1, …, 𝑣_𝑚 + 𝑤_𝑚$ is linearly independent.

**Solution**:

Counterexample:

Let

$$ 
𝑣_1 = (1, 0), 𝑣_2 = (0, 1) \\
w_1 = (0, 1), w_2 = (1, 0)
$$

Then

$$ 
𝑣_1 + 𝑤_1 = (1, 1) = 𝑣_2 + 𝑤_2
$$

$\square$

