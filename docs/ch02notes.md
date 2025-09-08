# Chapter 2 Finite-Dimensional Vector Spaces

## 2A Span and Linear Independence

### 2.2 definition: linear combination

A linear combination of a list $𝑣_1, …, 𝑣_𝑚$ of vectors in $𝑉$ 
is a vector of the form

$$ 
𝑎_1 𝑣_1 +⋯ + 𝑎_𝑚 𝑣_𝑚,
$$

where $𝑎_1, …, 𝑎_𝑚 ∈ 𝐅$.

### 2.4 definition: span

The set of all linear combinations of a list of vectors
$𝑣_1, …, 𝑣_𝑚$ in $𝑉$ is called
the span of $𝑣_1, …, 𝑣_𝑚$, denoted by
$\text{span}(𝑣_1, …, 𝑣_𝑚)$. In other words,

$$ 
\text{span}(𝑣_1, \cdots, 𝑣_𝑚) =
\{
a_1 v_1 + \cdots + a_m v_m : a_1, \cdots, a_m \in F
\}.
$$

The span of the empty list $()$ is defined to be $\{0\}$.

$\square$

### 2.6 span is the smallest containing subspace

The span of a list of vectors in $𝑉$ is the smallest subspace of $𝑉$ containing all vectors in the list.

**Proof**:

Let

$$ 
\text{span}(𝑣_1, \cdots, 𝑣_𝑚) =
\{
a_1 v_1 + \cdots + a_m v_m : a_1, \cdots, a_m \in F
\}.
$$

$v_i \in S$, because we can set $i = 1, j \neq i = 0$.

$$ 
v + w =
(a_1 v_1 + \cdots + a_m v_m)
+
(b_1 v_1 + \cdots + b_m v_m) \\
= (a_1+b_1) v_1 + \cdots + (a_m+b_m) v_m \in S
$$

So addition is closed.

$$ 
𝜆 v = 𝜆 (a_1 v_1 + \cdots + a_m v_m) \\
= (𝜆a_1) v_1 + \cdots + (𝜆a_m) v_m \in S
$$

So scalar multiplication is closed.

Finally $0 \in S$ by setting $a_1 = \cdots = a_m = 0$.

Every sub-space of $𝑉$ that contains each $𝑣_𝑘$ contains span
$(v_1, \cdots, v_m)$ . Thus $\text{span}(𝑣_1, \cdots, 𝑣_𝑚)$ 
is the smallest subspace of $𝑉$ containing all the vectors
$𝑣_1, …, 𝑣_𝑚$.

$\square$
