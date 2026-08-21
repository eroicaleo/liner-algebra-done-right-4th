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

## Section 5C Upper-Triangular Matrices

### 5.39 conditions for upper-triangular matrix

Suppose $𝑇 ∈ ℒ(𝑉)$ and $𝑣_1, …, 𝑣_𝑛$ is a basis of $𝑉$. Then the following are equivalent.

(a) The matrix of $𝑇$ with respect to $𝑣_1, …, 𝑣_𝑛$ is upper triangular.

(b) $\text{span}(𝑣_1, \cdots, 𝑣_k)$ is invariant under $𝑇$
for each $𝑘 = 1, …, 𝑛$.

(c) $Tv_k \in \text{span}(𝑣_1, \cdots, 𝑣_k)$ for each $𝑘 = 1, …, 𝑛$.

### 5.40 equation satisfied by operator with upper-triangular matrix

Suppose $𝑇 ∈ ℒ(𝑉)$ and $𝑉$ has a basis with respect to which $𝑇$ has an 
upper-triangular matrix with diagonal entries $𝜆_1, …, 𝜆_𝑛$. Then

$$ 
(𝑇 − 𝜆_1𝐼)⋯(𝑇 − 𝜆_𝑛𝐼) = 0
$$

**Proof**:

Assume the matrix of $𝑇$ with respect to $𝑣_1, …, 𝑣_𝑛$ is upper 
triangular.

Then $(T - 𝜆_1𝐼) v_1 = Tv_1 - 𝜆_1 v_1 = 𝜆_1 v_1 - 𝜆_1 v_1 = 0$.

So using 5.17(b) the commutativity of multiplication we have

$(𝑇 − 𝜆_1𝐼)⋯(𝑇 − 𝜆_l𝐼)v_1 = 0$ for $l = 1, 2, \cdots, n$.

Now since $T v_2 = a_{12} v_1 + 𝜆_2 v_2$, then
$(T-𝜆_2 I) v_2 = a_{12} v_1 \in \text{span}(𝑣_1)$, so 
$(T-𝜆_1 I)(T-𝜆_2 I) v_2 = 0$.

Again, using 5.17(b) the commutativity of multiplication we have

$(𝑇 − 𝜆_1𝐼)⋯(𝑇 − 𝜆_l𝐼)v_2 = 0$ for $l = 2, \cdots, n$.

We can continue this process,
$T v_k = a_{1k} v_1 + \cdots + a_{(k-1)k} v_{k-1} + 𝜆_k v_k$,
so 
$(T - 𝜆_kI) v_k \in \text{span}(𝑣_1, \cdots, 𝑣_{k-1})$

So $(T-𝜆_1 I)\cdots(T-𝜆_k I) v_k = 0$. Then

$(𝑇 − 𝜆_1𝐼)⋯(𝑇 − 𝜆_l𝐼)v_k = 0$ for $l = k, \cdots, n$.

So for any $v_i, i = 1, \cdots , n$, $(𝑇 − 𝜆_1𝐼)⋯(𝑇 − 𝜆_𝑛𝐼)v_i = 0$.

So $(𝑇 − 𝜆_1𝐼)⋯(𝑇 − 𝜆_𝑛𝐼) = 0$.

$\square$

### 5.41 determination of eigenvalues from upper-triangular matrix

Suppose $𝑇 ∈ ℒ(𝑉)$ has an upper-triangular matrix with respect to some 
basis of $𝑉$. Then the eigenvalues of $𝑇$ are precisely the entries on the 
diagonal of that upper-triangular matrix.

**Proof**:

Assume under basis $v_1, \cdots, v_n$, the matrix of $T$

$$ 
\mathcal{M}(T) =
\begin{pmatrix}
    \lambda_1 &        & * \\
              & \ddots &   \\
    0         &        &  \lambda_n \\
\end{pmatrix}
$$

Since $T v_1 = \lambda_1 v_1$, then $\lambda_1$ is an eigenvalue.

For $k > 1$, let $V_k$ denote $\text{span}(𝑣_1, \cdots, 𝑣_k)$.

We know $(T-\lambda_k I) v_k \in V_{k-1}$.
Furthermore, for since $V_{k-1}$ is invariant under $T$, then
$(T-\lambda_k I) v_i \in V_{k-1}$ for $i = 1, \cdots, k-1$.

If we restrict $(T-\lambda_k I)$ on $V_k$, then
$\text{range } T-\lambda_k I \subseteq V_{k-1}$.
Since $\dim V_k = k, \dim V_{k-1} = k-1$, from the
fundamental theorem of linear mapping, we have
$\text{null } T-\lambda_k I \neq \{0\}$. So we can find
$u_k \neq 0$, such that $(T-\lambda_k I) u_k = 0$, so $\lambda_k$ is
an eigenvalue.

On the other hand, if $\lambda$ is an eigenvalue of $T$,
and $p(z)$ is the minimal polynomial of $T$, then
$p(\lambda) = 0$.

Since from 5.40, $(𝑇 − 𝜆_1𝐼)⋯(𝑇 − 𝜆_𝑛𝐼) = 0$, then
$q(z) = (z − 𝜆_1)⋯(z − 𝜆_𝑛)$ is a multiple of $p$ from 5.29.

Then $q(\lambda) = 0$, so $\lambda \in \{\lambda_1, \cdots, \lambda_n\}$.

$\square$

### 5.44 necessary and sufficient condition to have an upper-triangular matrix

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$. Then $𝑇$ has an 
upper-triangular matrix with respect to some basis of $𝑉$ if and only if 
the minimal
polynomial of $𝑇$ equals $(𝑧 − 𝜆_1)⋯(𝑧 − 𝜆_𝑚)$ for some 
$𝜆_1, …, 𝜆_𝑚 ∈ 𝐅$.

**Proof**:

$\Rightarrow$

Assume $T$ has has an 
upper-triangular matrix with respect to some basis
$v_1, \cdots, v_n$.

And the elements on the diagonal are $\alpha_1, \cdots, \alpha_n$.

Also assume $p(z)$ is the minimal polynomial of $T$.

From 5.40, $(T − \alpha_1 I)⋯(T − \alpha_n I) = 0$, then
$q(z) = (z − \alpha_1 )⋯(z − \alpha_n )$ is a multiple of $p(z)$.

So $p(z)$ has to take the form of $(𝑧 − 𝜆_1)⋯(𝑧 − 𝜆_𝑚)$, where
$\lambda_1, \cdots, \lambda_m \in \{\alpha_1, \cdots, \alpha_n\}$.

$\Leftarrow$

We use induction for $m$.

If $m = 1$, then $p(z) = z - \lambda_1$ is the minimal polynomial.

Then every $v_k$ is a eigenvector, so $\text{span}(𝑣_1, \cdots, 𝑣_k)$ is
invariant for $k = 1, \cdots, n$.

From "5.39 conditions for upper-triangular matrix", given any basis
$v_1, \cdots, v_n$, the matrix of $T$ is upper-triangular.

Now consider when $m = 1, \cdots, l-1$, it all holds, then let $m = l$.

Consider $U = \text{range } T-\lambda_l I$. Then from 5.18 $U$ is invariant
under $T$ so we can consider $T|_U$.

Since $(T|_U − 𝜆_1 I)⋯(T|_U − 𝜆_{l-1} I) = 0$, 
So $(z − 𝜆_1)⋯(z − 𝜆_{l-1})$ is a multiple of the minimal polynomial
of $T|_U$. Then with our induction,
we can find a basis $u_1, \cdots, u_M$ under which the matrix of $T|_U$
is an upper-triangular matrix.

Then from "5.39 conditions for upper-triangular matrix" again,
we have $T u_k = T|_U (u_k) \in \text{span}(u_1, \cdots, u_k)$.

Extend $u_1, \cdots, u_M$ to a basis of $V$ by adding
$v_1, \cdots, v_N$.

Note $T v_k = (T - \lambda_kI) v_k + \lambda_k v_k \in
\text{span}(u_1, \cdots, u_M, 𝑣_1, \cdots, 𝑣_k)$ because
$(T - \lambda_kI) v_k \in U = \text{span}(u_1, \cdots, u_M)$.

Then again use 5.39, we have
𝑇 has an upper-triangular
matrix with respect to the basis
$u_1, \cdots, u_M, v_1, \cdots, v_N$

$\square$
