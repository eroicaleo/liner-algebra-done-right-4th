# Chapter 5 Eigenvalues and Eigenvectors

## Section 5A Invariant Subspaces

### 5A.1

Suppose $𝑇 ∈ ℒ(𝑉)$ and $𝑈$ is a subspace of $𝑉$.

(a) Prove that if $𝑈 ⊆ \text{null } T$, then $𝑈$ is invariant under $𝑇$.

**Proof**:

Assume $u \in U ⊆ \text{null } T$， $T(u) = 0 \in U$

$\square$

(b) Prove that if $\text{range } T ⊆ 𝑈$, then $𝑈$ is invariant under $𝑇$.

**Proof**:

If $u \in U$, then $T(u) \in \text{range } T ⊆ U$.

$\square$

### 5A.2

Suppose that $𝑇 ∈ ℒ(𝑉)$ and $V_1, \cdots, V_m$ are subspaces of $𝑉$ 
invariant under $𝑇$.
Prove that $𝑉_1 +⋯ + 𝑉_𝑚$ is invariant under $𝑇$.

**Proof**:

Assume $v \in 𝑉_1 +⋯ + 𝑉_𝑚$, then we have

$$ 
v = v_1 + \cdots + v_m, v_i \in V_i
$$

So

$$ 
T(v) = T(v_1) + \cdots + T(v_m)
$$

Since $T(v_i) \in V_i$, then $T(v) \in 𝑉_1 +⋯ + 𝑉_𝑚$.

$\square$

### 5A.3

Suppose $𝑇 ∈ ℒ(𝑉)$. Prove that the intersection of every collection of
subspaces of $𝑉$ invariant under $𝑇$ is invariant under $𝑇$.

**Proof**:

Let

$$ 
U = \cap_i U_i
$$

where $U_i$ is invariant under $𝑇$.

If $v \in U$, then $v \in U_i$, then $T(v) \in U_i$, so $T(v) \in U$.

$\square$

### 5A.4

Prove or give a counterexample: If $𝑉$ is finite-dimensional and $𝑈$ is a 
subspace of $𝑉$ that is invariant under every operator on $𝑉$ , then
$𝑈 = \{0\}$ or $𝑈 = 𝑉$.

**Proof**:

The statement is correct. We prove by contradition.

Assume $U$ is a subspace and $U \neq \{0\}$ and $U \neq V$.

Let $u_1, \cdots, u_m$ be a basis of $U$ and we can extends it to a basis
of $V$ by adding $v_1, \cdots, v_n$.

Define $T$ such that $T(u_i) = v_1, T(v_j) = v_1$.
So $T$ is an operator.

Then $U$ is not an invariant under $T$. We reach a contradition.

$\square$

### 5A.5

Suppose $𝑇 ∈ ℒ(𝐑^2)$ is defined by $𝑇(𝑥, 𝑦) = (−3𝑦, 𝑥)$. Find the 
eigenvalues of $𝑇$.

**Solution**:

$$
\begin{align*}
(−3𝑦, 𝑥) &= k(x, y) \\
& \Rightarrow \\
x = ky&, -3y = kx \\
& \Rightarrow \\
k^2 &= -3
\end{align*}
$$

So $T$ does not have any eigenvalues.

$\square$

### 5A.6

Define $𝑇 ∈ ℒ(𝐅^2)$ by $𝑇(𝑤, 𝑧) = (𝑧, 𝑤)$. Find all eigenvalues and 
eigenvectors of $𝑇$.

**Solution**:

Note $F$ can either be $\mathbb{R}$ or $\mathbb{C}$.

$$
\begin{align*}
k(w,z) &= (z,w) \\
& \Rightarrow \\
z = kw &, kz=w \\
& \Rightarrow \\
k^2 &= 1 \\
& \Rightarrow \\
k = &\pm1 
\end{align*} 
$$

If $k = 1$, then the eigenvectors are $(a,a)$. 
If $k = -1$, then the eigenvectors are $(a,-a)$. 

$\square$

### 5A.7

Define $𝑇 ∈ ℒ(𝐅^3)$ by $𝑇(𝑧_1, 𝑧_2, 𝑧_3) = (2𝑧_2, 0, 5𝑧_3)$. Find all 
eigenvalues and eigenvectors of $𝑇$.

**Proof**:

Note $F$ can either be $\mathbb{R}$ or $\mathbb{C}$.

$$
\begin{align*}
k(𝑧_1, 𝑧_2, 𝑧_3) &= (2𝑧_2, 0, 5𝑧_3) \\
& \Rightarrow \\
k z_1 = 2 z_2, k z_2 &= 0, k z_3 = 5 z_3
\end{align*} 
$$

If $k = 0$, then $z_3 = 0$. Also we have $0 = k z_1 = 2 z_2$, so $z_2 = 0$,
so the eigenvectors for $k = 0$ will
be $(a, 0, 0)$ for $a \neq 0$.

If $k \neq 0$, then $z_2 = 0$, then $z_1 = 0$. Since the eigenvectors cannot
be $0$, so $z_3 \neq 0$, so $k = 5$.
And the eigenvectors will be $(0,0, a)$ for $a \neq 0$.

$\square$

### 5A.8

Suppose $𝑃 ∈ ℒ(𝑉)$ is such that $𝑃^2 = 𝑃$. Prove that if $\lambda$ is an 
eigenvalue of $𝑃$, then $\lambda = 0$ or $\lambda = 1$.

**Proof**:

First we have the assumption that $V$ is a vector space over
$\mathbb{R}$ or $\mathbb{C}$.

If $\lambda$ is a eigenvalue and $u$ is a an eigenvector, then

$$ 
\begin{align*}
P^2(u) &= P(u) \\
& \Rightarrow \\
P(\lambda u) &= \lambda u \\ 
& \Rightarrow \\
\lambda^2 u &= \lambda u \\ 
\end{align*} 
$$

Since $u \neq 0$, then $\lambda^2 = \lambda$.
Since $\lambda$ is a real or complex number,
then $\lambda = 0$ or $\lambda = 1$.

$\square$

### 5A.9

Define $𝑇 ∶ 𝒫(𝐑) → 𝒫(𝐑)$ by $𝑇𝑝 = 𝑝'$. Find all eigenvalues and 
eigenvectors of $T$.

**Proof**:

Assume

$$ 
p(x) = a_0 + a_1 x + \cdots + a_{m} x^{m}
$$

Then

$$ 
T(p) = p'(x) = a_1 + 2 a_2 x + \cdots + m a_{m} x^{m-1}
$$

If $\lambda$ is an eigenvalue and $p$ is an eigenvector,

then 

$$
\begin{align*}
& \lambda a_0 + \lambda a_1 x + \cdots + \lambda a_{m} x^{m} \\
&=
a_1 + 2 a_2 x + \cdots + m a_{m} x^{m-1}
\end{align*} 
$$

So we have

$$ 
\begin{align*}
\lambda a_m &= 0 \\
\lambda a_{m-1} &= m a_m \\
&\cdots \\
\lambda a_1 &= 2 a_2 \\
\lambda a_0 &= a_1 \\
\end{align*} 
$$

If $\lambda = 0$, then $a_m = \cdots = a_1 = 0$, so the eigenvectors are
$p(x) = a \neq 0$.

If $\lambda \neq  0$, then $a_m = \cdots = a_0 = 0$, so there is no 
eigenvectors.

$\square$

### 5A.10

Define $𝑇 ∈ ℒ(𝒫_4(𝐑))$ by $(𝑇𝑝)(𝑥) = 𝑥𝑝'(𝑥)$ for all $𝑥 ∈ 𝐑$.
Find all eigenvalues and eigenvectors of $𝑇$.

**Proof**:

Assume

$$ 
p(x) = a_0 + a_1 x + \cdots + a_{m} x^{m}
$$

Then

$$ 
T(p) = xp'(x) = a_1x + 2 a_2 x^2 + \cdots + m a_{m} x^{m}
$$

If $\lambda$ is an eigenvalue and $p$ is an eigenvector,

then 

$$
\begin{align*}
& \lambda a_0 + \lambda a_1 x + \cdots + \lambda a_{m} x^{m} \\
&=
a_1x + 2 a_2 x^2 + \cdots + m a_{m} x^{m}
\end{align*} 
$$

So we have

$$ 
\begin{align*}
\lambda a_m &= m a_m \\
\lambda a_{m-1} &= (m-1) a_{m-1} \\
&\cdots \\
\lambda a_1 &=  a_1 \\
\lambda a_0 &= 0 \\
\end{align*} 
$$

If $\lambda = 0$, then $a_m = \cdots = a_1 = 0$, so the eigenvectors are
$p(x) = a \neq 0$.

If $\lambda \neq  0$, then we can have $\lambda$ to be any positive integer $n$,
and then eigenvectors will be $ax^n$ for $a \neq 0$.

$\square$

### 5A.11

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉)$,
and $𝛼 ∈ 𝐅$.
Prove that there exists $𝛿 > 0$ such that
$𝑇− \lambda 𝐼$ is invertible
for all $\lambda ∈ 𝐅$ such that
$0 < |\alpha − \lambda| < \delta$.

**Proof**:

Note $𝐅$ is either $\mathbf{R}$ or $\mathbf{C}$.

Since $V$ is finite-dimensional, then from
"5.12 operator cannot have more eigenvalues
than dimension of vector space", $T$ has at most
$\dim V$ eigenvalues.

Then we can find $\delta$ such that
$|\alpha - \lambda_i| \geq \delta$ where $\lambda_i$ is
an eigenvalue.

So if $0 < |\alpha − \lambda| < \delta$, then
$\lambda$ is not an eigenvalue.

Then from "5.7 equivalent conditions to be an eigenvalue"
we know $𝑇− \lambda 𝐼$ is invertible.

$\square$

### 5A.12

Suppose $𝑉 = 𝑈 ⊕ 𝑊$, where $𝑈$ and $𝑊$ are nonzero subspaces of $𝑉$. 
Define $𝑃 ∈ ℒ(𝑉)$ by $𝑃(𝑢 + 𝑤) = 𝑢$ for each $𝑢 ∈ 𝑈$ and
each $𝑤 ∈ 𝑊$. Find all eigenvalues and eigenvectors of $𝑃$ .

**Proof**:

Assume $\lambda$ is an eigenvalue, then

$$
\begin{align*}
P(u+w) &= \lambda (u+w) = u \\
& \Rightarrow \\
(\lambda - 1) u + \lambda w &= 0 \\
& \Rightarrow \\
(\lambda - 1) u &= \lambda w = 0 & \text{because } 𝑉 = 𝑈 ⊕ 𝑊 \\
\end{align*} 
$$

If $\lambda \neq 1$ and $\lambda \neq 0$, then we must have $u = w = 0$,
then $u+w$ is not an eigenvector, as a result, $\lambda$ is not
an eigenvalue.

If $\lambda = 1$, then every nonzero vector in $U$ is an eigenvector.
Indeed, given $u \in U, u \neq 0$, then $P(u) = u = 1 \cdot u$.

If $\lambda = 0$, then every nonzero vector in $W$ is an eigenvector.
Indeed, given $w \in W, w \neq 0$, then $P(w) = 0 = 0 \cdot w$.

$\square$
