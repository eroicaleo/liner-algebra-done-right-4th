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

### 2.7 definition: spans

If $\text{span}(𝑣_1, \cdots, 𝑣_𝑚)$ equals $𝑉$, we say 
that the list $𝑣_1, …, 𝑣_𝑚$ spans $𝑉$.

### 2.9 definition: finite-dimensional vector space

A vector space is called finite-dimensional if some list of 
vectors in it spans the space.

### 2.10 definition: polynomial, $𝒫(𝐅)$

A function $𝑝 ∶ 𝐅 → 𝐅$ is called a polynomial with 
coefficients in $𝐅$ if there exist $𝑎_0, …, 𝑎_𝑚 ∈ 𝐅$ such that

$$ 
p(z) = a_0 + a_1 z + \cdots + a_{m} z^{m}
$$

for all $z \in F$.

$𝒫(𝐅)$ is the set of all polynomials with coefficients
in $𝐅$.

$\square$

> If a polynomial that is identically zero as a function on 
> $𝐅$, then all coefficients are zero (will be proved in
> 4.8)

> Conclusion: the coefficients of a
> polynomial are uniquely determined by the polynomial.

### 2.11 definition: degree of a polynomial, deg 𝑝

A polynomial $p \in 𝒫(𝐅)$ is said to have degree $𝑚$ if 
there exist scalars $a_1, \cdots, a_m \in 𝐅$ with
$a_m \neq 0$, such that for every $𝑧 ∈ 𝐅$, we have

$$ 
p(z) = a_0 + a_1 z + \cdots + a_{m} z^{m}.
$$

The polynomial that is identically $0$ is said to have degree
$−∞$.

The degree of a polynomial $𝑝$ is denoted by $\deg 𝑝$.

### 2.12 notation: $𝒫_𝑚(𝐅)$

For $𝑚$ a nonnegative integer, $𝒫_𝑚(𝐅)$ denotes the set 
of all polynomials with coefficients in $𝐅$ and degree
at most $𝑚$.

### 2.13 definition: infinite-dimensional vector space

A vector space is called infinite-dimensional if it is not 
finite-dimensional.

### 2.14 example: $𝒫(𝐅)$ is infinite-dimensional.

Assume otherwise, then some list of polynomials can span
$𝒫(𝐅)$, let $m$ be the highest degree of the polynomials, 
in the list, then $z^{m+1}$ is not in the span.

$\square$

### Linear Independence

### 2.15 definition: linearly independent

A list $v_1, \cdots, v_m$ of vectors in $𝑉$ is called 
linearly independent if the only choice of
$a_1, \cdots, a_m \in F$ that makes

$$ 
a_1 v_1 + \cdots + a_m v_m = 0
$$

is $a_1 = \cdots = a_m = 0$.

The empty list $( )$ is also declared to be linearly 
independent.

### 2.17 definition: linearly dependent

* A list of vectors in $𝑉$ is called linearly dependent if 
  it is not linearly independent.
* A list $v_1, \cdots, v_m$ of vectors in $𝑉$ is linearly 
  dependent if there exist $a_1 = \cdots = a_m \in F$, not
  all $0$, such that $a_1 v_1 + \cdots + a_m v_m = 0$.

### 2.19 linear dependence lemma

Suppose $v_1, \cdots, v_m$ is a linearly dependent list in 
$𝑉$. Then there exists $k \in \{1,2,\cdots,m\}$
such that

$$ 
v_k \in \text{span}(𝑣_1, \cdots, 𝑣_{k-1}).
$$

Furthermore, if $𝑘$ satisfies the condition above and the 
𝑘th term is removed from $v_1, \cdots, v_m$,
then the span of the remaining list equals
$\text{span}(𝑣_1, \cdots, 𝑣_𝑚)$.

**Proof**:

We can find $a_1, \cdots, a_m \in F$, not all $0$ such that

$$ 
a_1 v_1 + \cdots + a_m v_m = 0
$$

Starting from $m$, let $k$ be the largest integer such that
$a_k \neq 0$. Then

$$ 
a_1 v_1 + \cdots + a_m v_m = 
a_1 v_1 + \cdots + a_k v_k = 0
$$

That is

$$ 
v_k = a_k^{-1} (a_1 v_1 + \cdots + a_{k-1} v_{k-1})
$$

