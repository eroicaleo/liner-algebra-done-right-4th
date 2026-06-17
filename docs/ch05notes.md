# Chapter 5 Eigenvalues and Eigenvectors

## Section 5A Invariant Subspaces

### 5.1 definition: operator

A linear map from a vector space to itself is called an operator.

> The reason we want to study invariant subspaces is because we want to
express the original space $V$ by the direct sum of some
smaller subspace. But we also want to each smaller subspace $V_k$ maps to
it self under $T$.

### 5.2 definition: invariant subspace

Suppose $𝑇 ∈ ℒ(𝑉$). A subspace $𝑈$ of $𝑉$ is called invariant
under $𝑇$ if $𝑇𝑢 ∈ 𝑈$ for every $𝑢 ∈ 𝑈$.

### 5.4 Examples

$\{0\}, V, \text{range } T, \text{null } T$ are all invariant under $T$.

> We investigate the simplest possible nontrivial invariant
> subspaces—invariant subspaces of dimension one.

### 5.5 definition: eigenvalue

Suppose $𝑇 ∈ ℒ(𝑉)$. A number $𝜆 ∈ 𝐅$ is called an eigenvalue of $𝑇$
if there exists $𝑣 ∈ 𝑉$ such that $𝑣 ≠ 0$ and $𝑇𝑣 = 𝜆𝑣$.

### 5.7 equivalent conditions to be an eigenvalue

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉)$, and $𝜆 ∈ 𝐅$.
Then the following are equivalent.

(a) $𝜆$ is an eigenvalue of $𝑇$.

(b) $𝑇 − 𝜆𝐼$ is not injective.

(c) $𝑇 − 𝜆𝐼$ is not surjective.

(d) $𝑇 − 𝜆𝐼$ is not invertible.

**Proof**:

If $\lambda$ is an eigenvalue of $𝑇$, then we can find $u \neq 0$ such that
$T u = \lambda u$, then $(T - \lambda I) (u) = 0$ so
$\text{null } (𝑇 − \lambda 𝐼)$ is not $\{0\}$, so $𝑇 − \lambda 𝐼$ is not 
injective.

Conditions (b), (c), and (d) are equivalent by 3.65.

$\square$

### 5.8 definition: eigenvector

Suppose $𝑇 ∈ ℒ(𝑉)$ and $𝜆 ∈ 𝐅$ is an eigenvalue of $𝑇$.
A vector $𝑣 ∈ 𝑉$ is called
an eigenvector of $𝑇$ corresponding to $𝜆$ if $𝑣 ≠ 0$ and $𝑇𝑣 = 𝜆𝑣$.

> a vector $𝑣 ∈ 𝑉$ with $𝑣 ≠ 0$ is an eigenvector of $𝑇$ corresponding
to $𝜆$ if and only if $𝑣 ∈ \text{null } (𝑇 − \lambda 𝐼)$.

### 5.11 linearly independent eigenvectors

Suppose $𝑇 ∈ ℒ(𝑉)$. Then every list of eigenvectors of $𝑇$ corresponding to
distinct eigenvalues of $𝑇$ is linearly independent.

**Summary of Proof**

Assume they are linearly dependent. Then find the minimal number of $v_i$
such that

$$ 
a_1 v_1 + \cdots + a_m v_m = 0
$$

And $a_i \neq 0$. Then apply $T- \lambda_m I$ to it we can reach a contradition.

$\square$

### 5.12 operator cannot have more eigenvalues than dimension of vector space

Suppose $𝑉$ is finite-dimensional. Then each operator on $𝑉$ has at most
$\dim 𝑉$ distinct eigenvalues.

### 5.17 multiplicative properties

$$ 
(𝑝𝑞)(𝑇) = 𝑝(𝑇)𝑞(𝑇); \\
𝑝(𝑇)𝑞(𝑇) = 𝑞(𝑇)𝑝(𝑇). \\
$$

### 5.18 null space and range of $𝑝(𝑇)$ are invariant under $𝑇$

Suppose $𝑇 ∈ ℒ(𝑉)$ and $𝑝 ∈ 𝒫(𝐅)$. Then $\text{null } 𝑝(𝑇)$ and
$\text{range } 𝑝(𝑇)$ are invariant under $𝑇$.

**Proof**:

If $u \in \text{range } p(T)$, then we can find $v$ such that
$p(T)(v) = u$, then $T(u) = T(p(T)(v)) = P(T)(T(v)) \in \text{range } P(T)$.

If $u \in \text{null } P(T)$, then
$P(T)(T(u)) = T(P(T)(u))= T(0)$. So $T(u) \in \text{null } P(T)$.

$\square$

## Section 5B The Minimal Polynomial

### 5.19 existence of eigenvalues

Every operator on a finite-dimensional nonzero complex vector space has an
eigenvalue.

**Proof**:

Let $n = \dim V$.

Consider $v \neq 0$ and $v, Tv, \cdots, T^nv$ is a group of $n+1$ vectors.
Since $\dim V = n$, then $v, Tv, \cdots, T^nv$ are linear dependent.

Then we can find a $k \leq n$, such that
$v, Tv, \cdots, T^{k-1}v$ are linear independent, but
$v, Tv, \cdots, T^kv$ is linear dependent.

So we can find 

$$ 
a_0v + a_1 T^1v + \cdots + a_k T^kv = 0
$$

In particular, $a_k \neq 0$.

Then consider $p(z) = a_0 + a_1 z^1 + \cdots + a_k z^k$. From
the fundamental theorem of algebra, it has a zero $\lambda$.

Then $p(z) = (z-\lambda ) q(z)$ where
$q(z) = b_0 + b_1 z^1 + \cdots + b_{k-1} z^{k-1}$.
In particular, $b_{k-1} = a_k \neq 0$.

Then

$$
\begin{align*}
q(T)(v)
&= (b_0 + b_1 T^1 + \cdots + b_{k-1} T^{k-1})(v) \\
&= b_0v + b_1 T^1v + \cdots + b_{k-1} T^{k-1}v \\
&\neq 0 &  \\
(&\because v, Tv, \cdots, T^{k-1}v \text{ are linear independent and }
b_{k-1} \neq 0)
\end{align*} 
$$ 

Thus $0 = p(T)(v) = (T-\lambda I)(q(T)(v))$, so $T$ has an eigenvalue
$\lambda$ and $q(T)(v)$ is an eigenvector.

$\square$

### 5.20 example

an operator on a complex vector space with no eigenvalues

$$ 
T(p(z)) = zp(z)
$$

### 5.21 definition: monic polynomial

A monic polynomial is a polynomial whose highest-degree coefficient equals 1.

### 5.22 existence, uniqueness, and degree of minimal polynomial

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$.
Then there is a unique monic
polynomial $𝑝 ∈ 𝒫(𝐅)$ of smallest degree such that $𝑝(𝑇) = 0$.
Furthermore, $\deg 𝑝 ≤ \dim 𝑉$.

**Proof**:

We use induction on the $\dim V$. When $\dim V = 0$, then
$p(z) = 1$, so $p(T) = I$ which is a zero operator on $V$.

Assume when $\dim V \leq n-1$, it is true. Now assume $\dim V = n$.

Given $v \neq 0$, then $v, Tv, \cdots, T^nv$ are linear dependent.
Then we can find a $1 \leq k \leq n$, such that
$v, Tv, \cdots, T^{k-1}v$ are linear independent, but
$v, Tv, \cdots, T^kv$ is linear dependent.

So we can find $a_0, \cdots, a_k$ which are not all zero such that

$$ 
a_0v + a_1 T^1v + \cdots + a_k T^kv = 0
$$

In particular, $a_k \neq 0$, otherwise
$a_0v + a_1 T^1v + \cdots + a_{k-1} T^{k-1}v = 0$ then
$a_0 = \cdots = a_k = 0$.

multiply by $a^{-1}_k$, we get

$$ 
b_0v + b_1 T^1v + \cdots + T^kv = 0
$$

Let $p(z) = z^k + \cdots + b_1z + b_0$.

Consider the $\text{null } p(T)$, note

$$ 
p(T)(T^i(v)) = T^i(p(T)(v)) = T^i(0) = 0
$$

So $v, Tv, \cdots, T^{k-1}v$ are a group of linear independent vectors
in $\text{null } p(T)$. Thus $\text{dim null } P(T) \geq k$.

From the fundamental theorem of linear mapping

$$ 
\text{dim range } p(T) = \dim V - \text{dim null } p(T) \leq n-k
$$

From 5.18 null space and range of $𝑝(𝑇)$ are invariant under $𝑇$,
we know $\text{range } p(T)$ is invariant under $T$.
Then we limit $T$ on $\text{range } p(T)$ and use induction to find a
monic polynomial $q(z)$, such that $q(T|_{\text{range } p(T)}) = 0$.

Then consider the monic polynomial $q(z)p(z)$. Given any $v$

$$ 
\begin{align*}
q(T) p(T) (v) &= q(T) (p(T)(v)) \\
&= q(T|_{\text{range } p(T)}) (p(T)(v)) \\
&\because p(T)(v) \in \text{range } p(T) \\
&= 0
\end{align*} 
$$

Furthermore $\deg q(z) \leq n-k, \deg p(z) = k$, so
$\deg q(z)p(z) \leq n$.

So we finished the induction.

$\square$

### 5.24 definition: minimal polynomial

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$.
Then the minimal polynomial
of $𝑇$ is the unique monic polynomial $𝑝 ∈ 𝒫(𝐅)$ of smallest degree such 
that $𝑝(𝑇) = 0$.

### 5.27 eigenvalues are the zeros of the minimal polynomial

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$.

(a) The zeros of the minimal polynomial of $𝑇$ are the eigenvalues of $𝑇$.

**Proof**:

Assume $\lambda$ is a zero of $p(z)$ which is the minimal polynomial of $𝑇$.
Then from the fundamental theorem of algebra, we have
$p(z) = (z-\lambda)q(z)$, since $\deg q < \deg p$ then
$q(z)$ is not the minimal polynomial of $𝑇$, then we can find
$v$ such that $q(T)(v) \neq 0$. Then

$$ 
\begin{align*}
0 = p(T)(v) = (T-\lambda I)(q(T)(v))
\end{align*} 
$$

So $\lambda$ is an eigenvalue and $q(T)(v)$ is an eigenvector.

On the other hand, if $\lambda$ is an eigenvalue and $v$ is an eigenvector,
then

$$ 
\begin{align*}
0 = p(T)(v)
&=(a_0 + a_1 T + \cdots + a_{n} T^{n})(v) \\
&= a_0v + a_1 Tv + \cdots + a_{n} T^{n}v \\
&= a_0v + a_1 \lambda v + \cdots + a_{n} \lambda ^{n}v \\
&= (a_0 + a_1 \lambda + \cdots + a_{n} \lambda ^{n})v \\
\end{align*} 
$$

Since $v \neq 0$, then $a_0 + a_1 \lambda + \cdots + a_{n} \lambda ^{n} = 0$.
So $p(\lambda) = 0$, then $\lambda$ is a zero of the minimal polynomial $T$.

$\square$

(b) If $𝑉$ is a complex vector space, then the minimal polynomial of $𝑇$
has the form

$$ 
(𝑧 − \lambda_1)⋯(𝑧 − \lambda_𝑚),
$$

where $\lambda_1, …, \lambda_𝑚$ is a list of all eigenvalues of $𝑇$,
possibly with repetitions.

**Proof**:

Using the fundamental theorem of algebra, we can represent the minimal
polynomial of $T$ as

$$ 
p(z) = (𝑧 − \lambda_1)⋯(𝑧 − \lambda_𝑚).
$$

Then use (a), we know $\lambda_1, \cdots, \lambda_m$ are eigenvalues.

$\square$

### 5.29 $𝑞(𝑇) = 0 ⟺ 𝑞$ is a polynomial multiple of the minimal polynomial

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉)$, and $𝑞 ∈ 𝒫(𝐅)$.
Then $𝑞(𝑇) = 0$
if and only if $𝑞$ is a polynomial multiple of the minimal polynomial of $𝑇$.

**Proof**:

$\Rightarrow$

Assume $p(z)$ is the minimal polynomial of $T$, then $\deg p \leq \deg q$.
Then we can use the division algorithm of polynomial to get
$q(z) = s(z)p(z) + r(z)$ where $\deg r < \deg p$.

Then

$$ 
\begin{align*}
r(T)(v) &= (q(T) - s(T)p(T))(v) \\
&= q(T)(v) - s(T)p(T)(v) \\
&= 0 - 0 \\
&= 0 \\
\end{align*} 
$$

So $r(T) = 0$, then $𝑞$ is a polynomial multiple of $p$.

$\square$

$\Leftarrow$

Assume $q(z) = s(z)p(z)$, then

$$ 
\begin{align*}
q(T)(v) &= (s(T)p(T))(v) \\
&= s(T)(p(T)(v)) \\
&= s(T)(0) \\
&= 0 \\
\end{align*} 
$$

$\square$

### 5.31 minimal polynomial of a restriction operator

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉)$, and
$𝑈$ is a subspace of $𝑉$ that is
invariant under $𝑇$.
Then the minimal polynomial of $𝑇$ is a polynomial multiple
of the minimal polynomial of $𝑇|𝑈$.

**Proof**:

Assume $p(z)$ is the minimal polynomial of $𝑇$.
Then given $v \in V$, we have $p(T)(v) = 0$.

In particular, for any $u \in U$, $p(T)(u) = 0$.

Since for any $u \in U$, $T|_U(u) = T(u)$.
$U$ is invariant under $T$, so we have
$p(T|_U)(u) = p(T)(u) = 0$.

Then apply 5.29, we have $p(z)$
is a polynomial multiple
of the minimal polynomial of $𝑇|𝑈$.

$\square$

### 5.32

$𝑇$ not invertible $⟺$ constant term of minimal polynomial of $𝑇$ is $0$.

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$.
Then $𝑇$ is not invertible if
and only if the constant term of the minimal polynomial of $𝑇$ is $0$.

**Proof**:

$$
\begin{align*}
T &\text{ not invertible } \\
& ⟺ \\
\text{null } T &\neq \{0\} \\
& ⟺ \\
0 &\text{ is an eigenvalue of } T \\
& ⟺ \\
0 &\text{ is a zero of the minimal polynomial of } T \\
& ⟺ \\
&\text{the constant term of the minimal polynomial of } 𝑇 \text{ is } 0
\end{align*} 
$$

$\square$

### 5.33 even-dimensional null space

Suppose $𝐅 = 𝐑$ and $𝑉$ is finite-dimensional.
Suppose also that $𝑇 ∈ ℒ(𝑉)$
and $𝑏, 𝑐 ∈ 𝐑$ with $𝑏^2 < 4𝑐$.
Then $\text{dim null } 𝑇^2 + 𝑏𝑇 + 𝑐𝐼$ is an even number.

**Proof**:

From
"5.18 null space and range of $𝑝(𝑇)$ are invariant under $𝑇$",
we know $\text{null } 𝑇^2 + 𝑏𝑇 + 𝑐𝐼$ is invariant under $T$.

So we can restrict $T$ to $\text{null } 𝑇^2 + 𝑏𝑇 + 𝑐𝐼$.

We reuse the symbol $V$ and let it denote
$\text{null } 𝑇^2 + 𝑏𝑇 + 𝑐𝐼$.

We just need to prove $\dim V$ is an even number.

First, we will show $T$ does not have an eigenvalue.
We prove by contradition. Assume $k$ is an eigenvalue and
$v$ is an eigenvector. Then

$$ 
\begin{align*}
0 &= (𝑇^2 + 𝑏𝑇 + 𝑐𝐼)(v) \\
&=
𝑇^2v + 𝑏𝑇v + 𝑐𝐼v \\
&= (k^2 + bk + c)v \\
\end{align*} 
$$

Since $𝑏^2 < 4𝑐$ and $k \in \mathbb{R}$, so
$k^2 + bk + c \neq 0$, so $v = 0$, then
$T$ does not have an eigenvalue.

Now let $U$ be the subspace that is invariant under $T$
with the largest even degree.

If $U \neq V$, we can find $w \not\in U$.

Consider $W = \text{span}(w, Tw)$, $W$ is invariant under $T$.
This is because $T^2w = -bTw - cw \in W$.

Now

$$ 
\dim (U+W) = \dim U + \dim W - \dim (U \cap W)
$$

Since both $U, W$ are invariant under $T$, so is $U \cap W$.

If $\dim (U \cap W) = 1$, then $U \cap W$ is an one dimensional
invariant subspace, then we can find an eigenvalue which is
contradictory to the face that $T$ does not have an eigenvalue.

So $\dim (U \cap W) = 0$, then

$$ 
\dim (U+W) = \dim U + 2
$$

So we produce an subspace that is invariant under $T$
with bigger even degree, and we reach a contradition.

So $U = V$ and we finished the proof.

$\square$
