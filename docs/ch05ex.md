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

### 5A.13

Suppose $𝑇 ∈ ℒ(𝑉)$. Suppose $𝑆 ∈ ℒ(𝑉)$ is invertible.

(a) Prove that $𝑇$ and $𝑆^{−1}𝑇𝑆$ have the same eigenvalues.

**Proof**:

If $\lambda$ is an eigenvalue of $T$, then we can find $v \neq 0$ such
that $T(v) = \lambda v$. Since $S$ is invertible, we can find
$u$ such that $u = S^{-1}(v)$. Since $S^{-1}$ is invertible and $v \neq 0$, then $u \neq 0$.

$$ 
\begin{align*}
𝑆^{−1}𝑇𝑆(u) &= 𝑆^{−1}𝑇𝑆(S^{-1}(v)) \\
&= 𝑆^{−1}𝑇(v) \\
&= 𝑆^{−1}(\lambda v) \\
&= \lambda 𝑆^{−1}(v) \\
&= \lambda u \\
\end{align*} 
$$

On the other hand, if $\lambda$ is an eigenvalue of $𝑆^{−1}𝑇𝑆$,
and assume $v \neq 0$ such
that $𝑆^{−1}𝑇𝑆(v) = \lambda v$

Then we have

$$ 
\begin{align*}
S(𝑆^{−1}𝑇𝑆(v)) &= S(\lambda v) \\
TS(v) &= \lambda S(v) \\
\end{align*} 
$$

Since $v \neq 0$ and $S$ is invertible, then $S(v) \neq 0$.
So $S(v)$ is an eigenvector of $T$.

$\square$

(b) What is the relationship between the eigenvectors of $𝑇$ and
the eigenvectors of $𝑆^{−1}𝑇𝑆$?

**Proof**:

From (a), if $v$ is an eigenvector of $T$, then $S^{-1}(v)$ is an eigenvector
of $𝑆^{−1}𝑇𝑆$.

Conversely, if $v$ is an eigenvector of $𝑆^{−1}𝑇𝑆$, then
$S(v)$ is an eigenvector of $T$.

$\square$

### 5A.14

Give an example of an operator on $𝐑^4$ that has no (real) eigenvalues.

**Solution**:

Consider this operator (borrowed from 5.9(b))

$$ 
T : (a, b, c, d) \rightarrow (-b, a, -d, c)
$$

Assume $k$ is an real eigenvalue, then

$$ 
T((a, b, c, d)) = k (a, b, c, d) = (-b, a, -d, c)
$$

Then

$$ 
\begin{align*}
ka &= -b \\
kb &= a  \\
kc &= -d \\
kd &= c  \\
& \Rightarrow \\
k^2 b = -b &,
k^2 d = -d 
\end{align*} 
$$

If $k \neq 0$, then $(k^2+1) > 0$ so $(k^2+1)b = 0$ means $b = 0$. Similarly
$d = 0$, then $a = c = 0$, so $k$ is not an
eigenvalue.

If $k = 0$, then $a = c = 0$, then $b = d = 0$, so $k$ is still not an
eigenvalue.

$\square$

### 5A.15

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉)$, and $\lambda ∈ 𝐅$. Show that $\lambda$ 
is an eigenvalue of $𝑇$ if and only if $\lambda$ is an eigenvalue of the dual operator
$𝑇' ∈ ℒ(𝑉')$.

**Proof**

Given $v_1, \cdots, v_m$ be a basis of $V$ and $\varphi_1, \cdots, \varphi_m$
be its dual basis.

Let $A$ be the matrix of $T$ under basis $v_1, \cdots, v_m$ and
$A'$ be the matrix of $T'$ under basis $\varphi_1, \cdots, \varphi_m$.

From "3.132 matrix of $𝑇'$ is transpose of matrix of $𝑇$", we know
$A' = A^t$.

Let $E$ be the identity matrix, then the matrix for operator $T - \lambda I$
is $A - \lambda E$. Similarly, the matrix for operator $T' - \lambda I'$,
is $A' - \lambda E$.

Note that $(A - \lambda E)^t = A^t - \lambda E^t = A' - \lambda E$.

Then from "5.7 equivalent conditions to be an eigenvalue" we have the
following equivalent relation.

$$ 
\begin{align*}
& \lambda \text{ is an eigenvalue of } 𝑇 \\
& \Leftrightarrow \\
& T - \lambda I \text{ is not invertible} \\
& \Leftrightarrow \\
& \text{dim range } T - \lambda I < \dim V \\
& \Leftrightarrow \\
& \text{column rank of } A - \lambda E < \dim V \\
& \Leftrightarrow \\
& \text{row rank of } A - \lambda E < \dim V \\
& \Leftrightarrow \\
& \text{column rank of } A' - \lambda E < \dim V
& \text{because } (A - \lambda E)^t = A' - \lambda E\\
& \Leftrightarrow \\
& \text{dim range } T' - \lambda I' < \dim V \\
& \Leftrightarrow \\
& T' - \lambda I' \text{ is not invertible} \\
& \Leftrightarrow \\
& \lambda \text{ is an eigenvalue of the dual operator } T'
\end{align*} 
$$

$\square$

The following is my original thought, but it seems not working.

$\Rightarrow$

Assume $\lambda$ is an eigenvalue of $𝑇$, and let $v_1$ be an eigenvector so
$T(v_1) = \lambda v_1 = w_1$.

Note $w_1 \in \text{range } T$, we can extend it to a basis of $\text{range } T$
by adding $w_2, \cdots, w_m$

Then we can find a group of linear independent vectors $v_1, \cdots, v_m$ 
such that $T(v_i) = w_i$.

Then we can find a basis of $\text{null } T$: $u_1, \cdots, u_n$.

Together
$v_1, \cdots, v_m, u_1, \cdots, u_n$ forms a basis of $V$.

Furthermore, we can extend $w_1, \cdots, w_m$ to a basis of $V$ by adding
vectors $x_1, \cdots, x_n$ 

Then consider the dual basis $\varphi_1, \cdots, \varphi_{m+n}$ of
$w_1, \cdots, w_m, x_1, \cdots, x_n$.

Let

$$
\begin{align*}
v &= a_1 v_1 + \cdots + a_m v_m + b_1 u_1 + \cdots + b_n u_n \\
&= a_1 v_1 + \cdots + a_m v_m + b_1 u_1 + \cdots + b_n u_n
\end{align*} 

$$

Then

$$ 
\begin{align*}
T'(\varphi_1)(v) &= \varphi_1(T(v)) \\
&= \varphi_1(a_1 Tv_1 + \cdots + a_m Tv_m) \\
&= \varphi_1(a_1 w_1 + \cdots + a_m w_m) \\
&= a_1 w_1
\end{align*} 
$$

$\square$

### 5A.16

Suppose $𝑣_1, …, 𝑣_𝑛$ is a basis of $𝑉$ and $𝑇 ∈ ℒ(𝑉)$.
Prove that if $\lambda$ is an
eigenvalue of $𝑇$, then

$$
|\lambda| ≤ 𝑛 \max \{∣ℳ(𝑇)_{𝑗, 𝑘}∣ : 1 ≤ 𝑗, 𝑘 ≤ 𝑛 \}
$$

, where $ℳ(𝑇)_{𝑗, 𝑘}$ denotes the entry in row $𝑗$, column $𝑘$ of
the matrix of $𝑇$ with respect to the basis $𝑣_1, …, 𝑣_𝑛$.

**Proof**:

Let $A = ℳ(𝑇)$, and $M = \max \{∣ℳ(𝑇)_{𝑗, 𝑘}∣ : 1 ≤ 𝑗, 𝑘 ≤ 𝑛 \}$ . 

Assume $v$ is an eigenvector and
$T(v) = \lambda v$.

Also assume

$$ 
v = a_1 v_1 + \cdots + a_n v_n
$$

So we have

$$ 
\begin{align*}
\lambda v &= T(v) \\
&= a_1 T(v_1) + \cdots + a_n T(v_n)
\end{align*} 
$$

On the other hand

$$ 
\lambda v = \lambda a_1 v_1 + \cdots + \lambda a_n v_n
$$

So we have

$$ 
a_1 T(v_1) + \cdots + a_n T(v_n) = \lambda a_1 v_1 + \cdots + \lambda a_n v_n
$$
Compare the coefficients of $v_1, \cdots, v_n$ on both sides, we have

$$
\begin{align*}
\lambda a_1 &= a_1 A_{1,1} + a_2 A_{1,2} + \cdots + a_n A_{1, n} \\
\lambda a_2 &= a_1 A_{2,1} + a_2 A_{2,2} + \cdots + a_n A_{2, n} \\
\cdots \\
\lambda a_n &= a_1 A_{n,1} + a_2 A_{n,2} + \cdots + a_n A_{n, n} \\
\end{align*} 
$$

Assume $|a_1| \geq |a_i|$, then we must have $|a_1| > 0$.
This is because $v$ as an eigenvector cannot be $0$.

$$ 
\begin{align*}
|\lambda a_1| &\leq |a_1 A_{1,1}| + |a_2 A_{1,2}| + \cdots + |a_n A_{1, n}| \\
&\Rightarrow \\
|\lambda | &\leq
|a_1 A_{1,1}|/|a_1| + |a_2 A_{1,2}|/|a_1| + \cdots + |a_n A_{1, n}|/|a_1| \\
&\leq |A_{1,1}| + |A_{1,2}| + \cdots + |A_{1, n}|\\
& \leq M + M + \cdots + M \\
& \leq nM \\
\end{align*} 
$$

$\square$

### 5A.17

Suppose $𝐅 = 𝐑, 𝑇 ∈ ℒ(𝑉)$, and $\lambda ∈ 𝐑$. Prove that $\lambda$ is an 
eigenvalue of 𝑇
if and only if $\lambda$ is an eigenvalue of the complexification $𝑇_𝐂$.

The complexification is defined in Exercise 1B.8
See Exercise 33 in Section 3B for the definition of $𝑇_𝐂$.

**Proof**:

$\Rightarrow$

Assume $\lambda$ is an eigenvalue of $T$ and $v$ is an eigenvector,
then $T(v) = \lambda v$.

Now consider

$$
\begin{align*}
T_c (v + iv) &= T(v) + i T(v) \\
&= \lambda v + i (\lambda v) \\
&= \lambda (v + iv) \\
\end{align*}
$$ 

Since $v \neq 0$, then $v + iv \neq 0$.
Then $v + iv$ is an eigenvector and $\lambda$ is an eigenvalue.

$\Leftarrow$

Assume $\lambda$ is an eigenvalue of $T_C$ and $u + iv \neq 0$ is an 
eigenvector. Then $u \neq 0$ or $v \neq 0$.

$$ 
\begin{align*}
T_C(u+iv) &= \lambda (u+iv) \\
&\Rightarrow \\
T(u) + i T(v) &= \lambda u + i \lambda v \\
&\Rightarrow \\
T(u) = \lambda u &, T(v) = \lambda v \\
\end{align*} 
$$

So one of $u$ or $v$ is an eigenvector for sure. And $\lambda$ is
an eigenvalue.

$\square$

### 5A.18

Suppose $𝐅 = 𝐑, 𝑇 ∈ ℒ(𝑉)$, and $\lambda ∈ 𝐂$. Prove that $\lambda$ is an 
eigenvalue of the complexification $𝑇_𝐂$ if and only if $\overline{\lambda}$ 
is an eigenvalue of $𝑇_𝐂$.

**Proof**:

$\Rightarrow$

$\lambda = a + bi$ is an eigenvalue of the complexification $𝑇_𝐂$,
then there is a $u+iv \neq 0$ such that

So we have

$$
\begin{align*}
T_C(u+iv) &= T(u) + iT(v) \\
&= \lambda (u+iv) \\
&=
(a+bi) (u+iv) \\
&= (au - bv) + i(bu+av) \\
&\Rightarrow \\
T(u) = (au - bv) &, T(v) = bu+av \\
\end{align*} 
$$

Now consider

$$
\begin{align*}
T_C(u-iv) &= T(u) - iT(v) \\
&= (au - bv) - i(bu+av) \\
&= (a-ib)(u-iv) \\
\end{align*} 
$$ 

So $\overline{\lambda} = a-bi$ is also an eigenvalue of $T_C$.

The other direction is similar.

$\square$

### 5A.19

Show that the forward shift operator $𝑇 ∈ ℒ(𝐅^∞)$ defined by

$$ 
𝑇(𝑧_1, 𝑧_2, … ) = (0, 𝑧_1, 𝑧_2, … )
$$

has no eigenvalues.

**Proof**:

We use contradition.

Assume $\lambda$ is an eigenvalue and $(𝑧_1, 𝑧_2, … )$ is an eigenvector
So we can find $z_m \neq 0$.

Also

$$
\begin{align*}
\lambda z_1 &= 0 \\
\lambda z_2 &= z_1 \\
&\cdots \\
\lambda z_{m} &= z_{m-1} \\
\lambda z_{m+1} &= z_{m} \\
\end{align*} 
$$

If $\lambda = 0$, then $\lambda z_{m+1} = 0 \neq z_m$, so we have contradition.

If $\lambda \neq 0$, then since $\lambda z_1 = 0$, we have $z_1 = 0$,
similarly, $z_2 = \cdots = z_m = 0$, we reach a contradition.

So $T$ has no eigenvalues.

$\square$

### 5A.20

Define the backward shift operator $𝑆 ∈ ℒ(𝐅^∞)$ by

$$ 
𝑆(𝑧_1, 𝑧_2, 𝑧_3, … ) = (𝑧_2, 𝑧_3, … ).
$$

(a) Show that every element of $𝐅$ is an eigenvalue of $𝑆$.

**Proof**:

Let $\lambda \in F$.

If $\lambda = 0$, then $(1, 0, 0, \cdots )$ is an eigenvector.

If $\lambda \neq 0$, then $(1, \lambda, \lambda ^2, \cdots )$ is an
eigenvector.

$\square$

(b) Find all eigenvectors of $𝑆$.

**Solution**:

From part (a), the eigenvectors are $(a, 0, 0, \cdots )$ with $a \neq 0$
and $(1, \lambda, \lambda ^2, \cdots )$.

$\square$

### 5A.21

Suppose $𝑇 ∈ ℒ(𝑉)$ is invertible.

(a) Suppose $\lambda ∈ 𝐅$ with $\lambda ≠ 0$. Prove that $\lambda$ is an 
eigenvalue of $𝑇$ if and only if $1/\lambda$ is an eigenvalue of $𝑇^{−1}$.

**Proof**:

$\Rightarrow$

$$ 
\begin{align*}
&\lambda \text{ is an eigenvalue } \\
&\Rightarrow \\
\text{We can find } u &\neq 0, \text{ such that } T(u) = \lambda u \\
&\Rightarrow \\
u = T^{-1}(T(u)) &= T^{-1}(\lambda u) = \lambda T^{-1}(u)\\
&\Rightarrow \\
T^{-1}(u) &= 1/\lambda u & \text{because } \lambda \neq 0
\end{align*} 
$$

Since $u \neq 0$, then $1/\lambda$ an eigenvalue of $𝑇^{−1}$.

$\Leftarrow$

The reverse side is similar.

$\square$

(b) Prove that $𝑇$ and $𝑇^{−1}$ have the same eigenvectors.

**Proof**:

The proof in (a) already showed if $u$ is an eigenvector of $T$, it's
also a eigenvector of $𝑇^{−1}$ and vice versa.

$\square$

### 5A.22

Suppose $𝑇 ∈ ℒ(𝑉)$ and there exist nonzero vectors $𝑢$ and $𝑤$ in $𝑉$ such 
that 

$$ 
Tu = 3w \text{ and } Tw = 3u
$$

Prove that 3 or −3 is an eigenvalue of $𝑇$.

**Proof**:

If $u = -w$, then $Tu = 3w = -3u$, since $u \neq 0$, then $-3$ is an 
eigenvalue. 

If $u \neq -w$, then consider

$$ 
T(u+w) = Tu + Tw = 3w + 3u = 3 (u + w)
$$

Since $u \neq -w$, then $u+w \neq 0$. So $3$ is an eigenvalue.

$\square$

### 5A.23

Suppose $𝑉$ is finite-dimensional and $𝑆, 𝑇 ∈ ℒ(𝑉)$.
Prove that $𝑆𝑇$ and $𝑇𝑆$ have the same eigenvalues.

**Proof**:

If $\lambda$ is an eigenvalue of $ST$ and $u \neq 0$ is an eigenvector
such that $ST(u) = \lambda u$.

Then we have $TS(T(u)) = T(ST(u)) = T(\lambda u) = \lambda T(u)$.

If $T(u) \neq 0$, then $\lambda$ is an eigenvalue of $TS$.

If $T(u) = 0$, then $\lambda = 0$,
then we need to show $\text{null } TS \neq \{0\}$.

If $S$ is invertible, then we can find $v$ such that $S(v) = u$. Note
$v$ can not be $0$ since $S(0) = 0 \neq u$. Then $TS(v) = T(u) = 0$.
So $v \in \text{null } TS$.

If $S$ is not invertible, then we can find $v \neq 0$, such that $S(v) = 0$.
Then $TS(v) = T(S(v)) = T(0) = 0$, so $v \in \text{null } TS$.

In any case, $\text{null } TS \neq \{0\}$. And $0$ is also an eigenvalue
of $TS$.

The reverse side is similar.

$\square$

### 5A.24

Suppose $𝐴$ is an $𝑛$-by-$𝑛$ matrix with entries in $𝐅$.
Define $𝑇 ∈ ℒ(𝐅^𝑛)$ by $𝑇𝑥 = 𝐴𝑥$, where elements of $𝐅^𝑛$ are
thought of as $𝑛$-by-$1$ column vectors.

(a) Suppose the sum of the entries in each row of $𝐴$ equals $1$.
Prove that $1$ is an eigenvalue of $𝑇$.

**Proof**:

Consider the vector

$$
\begin{align*}
v &= e_1 + \cdots + e_n \neq 0\\
&\Rightarrow \\
T(v) &= T(e_1) + \cdots + T(e_n) \\
&= Ae_1 + \cdots + Ae_n \\
&= (\sum_{i = 1}^{n} a_{1i}) e_1 + \cdots + (\sum_{i = 1}^{n} a_{ni}) e_n \\
&= e_1 + \cdots + e_n \\
&= v
\end{align*} 
$$

So $T(v) = v$ and $1$ is an eigenvalue of $𝑇$.

$\square$

(b) Suppose the sum of the entries in each column of $𝐴$ equals $1$.
Prove that $1$ is an eigenvalue of $𝑇$.

**Proof**:

Consider $T'$ is the dual map of $T$ in $(F^n)'$. Then its matrix under
dual basis is $A^T$. Then the sum of the entries in each row of $A^T$
equals $1$. Then we can apply part (a) and know $1$ is an
eigenvalue of $T'$.

No we use the Exercise 5A.15 in this section which states
$𝜆$ is an eigenvalue of $𝑇$ if and only if $𝜆$ is an eigenvalue of the dual 
operator $𝑇' ∈ ℒ(𝑉')$. And then we know $1$ is an
eigenvalue of $T$.

$\square$

### 5A.25

Suppose $𝑇 ∈ ℒ(𝑉)$ and $𝑢, 𝑤$ are eigenvectors of $𝑇$ such that $𝑢 + 𝑤$ 
is also an eigenvector of $𝑇$. Prove that $𝑢$ and $𝑤$ are eigenvectors of 
$𝑇$ corresponding to the same eigenvalue.

**Proof**:

Assume

$$ 
\begin{align*}
T(u) &= \lambda_1 u \\
T(w) &= \lambda_2 w \\
T(u+w) &= \lambda_3 (u + w) \\
\end{align*} 
$$

Then

$$ 
\begin{align*}
\lambda_3 (u + w) & = T(u+w) \\
&= T(u) + T(w) \\
&= \lambda_1 u + \lambda_2 w \\
& \Rightarrow \\
(\lambda_3 - \lambda_1) u + (\lambda_3 - \lambda_2) w &= 0
\end{align*} 
$$

If $\lambda_1 \neq \lambda_2$, then $u$ and $w$ is independent, so
$\lambda_3 - \lambda_1 = \lambda_3 - \lambda_2 = 0$.

Then $\lambda_1 = \lambda_2 = \lambda_3$, we have an contradition.

So $\lambda_1 = \lambda_2$.

$\square$

### 5A.26

Suppose $𝑇 ∈ ℒ(𝑉)$ is such that every nonzero vector in $𝑉$ is an 
eigenvector of $𝑇$. Prove that $𝑇$ is a scalar multiple of the identity 
operator.

**Proof**:

Consider $v_1 \neq 0, v_2 \neq 0$, and their eigenvalues are
$\lambda_1, \lambda_2$.

If $v_1 = -v_2$, then $T(v_1+v_2) = 0$, then $\lambda_1 v_1+ \lambda_2 v_2 = 0$. Then $(\lambda_1 - \lambda_2) v_1 = 0$.

Since $v_1 \neq 0$ then $\lambda_1 - \lambda_2 = 0$, i.e.
$\lambda_1 = \lambda_2$.

If $v_1 \neq -v_2$, then $v_1 + v_2 \neq 0$ is also an eigenvector of $T$.
From the last Exercise, we know $\lambda_1 = \lambda_2$.

So for any $v$, $T(v) = \lambda_1 v$. Then
$𝑇$ is a scalar multiple of the identity operator.

$\square$

### 5A.27

Suppose that $𝑉$ is finite-dimensional and $𝑘 ∈ {1, …, \dim 𝑉 − 1}$. Suppose
$𝑇 ∈ ℒ(𝑉)$ is such that every subspace of $𝑉$ of dimension $𝑘$ is invariant
under $𝑇$. Prove that $𝑇$ is a scalar multiple of the identity operator.

**Proof**:

Let $\dim V = n$. Consider $v_1 \in V, v_1 \neq 0$, we can extend $v_1$ to a 
basis of $V$ by adding $v_2, \cdots, v_n$.

Assume

$$ 
T(v_1) = a_1 v_1 + \cdots + a_n v_n
$$

If $a_n \neq 0$, then let $U = \text{span}(𝑣_1, \cdots, 𝑣_k)$. $U$ is an
invariant of $T$.

So $T(v_1) = a_1 v_1 + \cdots + a_k v_k$. Since $T(v_1)$ can be
represented by $v_1, \cdots, v_n$ uniquely, we have $a_n = 0$.

Similarly we can show $a_2 = \cdots = a_n = 0$.
So $v_1$ is an eigenvector.

That means every vector $v$ is an eigenvector of $T$.

From last Exercise, we know $𝑇$ is a scalar multiple of the identity operator.

$\square$

### 5A.28

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$.
Prove that $𝑇$ has at most $1 + \text{dim range } T$
distinct eigenvalues.

**Proof**:

We prove by contradition.
Assume there are more than $1 + \text{dim range } T$, then
there are a least $1 + \text{dim range } T$ nonzero eigenvalues.

Let $m = \text{dim range } T$, we can find $m+1$ eigenvectors with
different eigenvalues, i.e.

$$ 
\begin{align*}
T(v_1) = \lambda_1 v_1, &\cdots, T(v_{m+1}) = \lambda_{m+1} v_{m+1} \\
& \Rightarrow \\
\lambda_1 v_1, &\cdots , \lambda_{m+1} v_{m+1} \in \text{range } T \\
& \Rightarrow \\
v_1, &\cdots , v_{m+1} \in \text{range } T 
& \text{Because } \lambda_i \neq 0 \\
& \Rightarrow \\
\text{dim range } T &\geq m+1 & \text{Because } v_i \text{ are independent} \\
\end{align*} 
$$

So we reached an contradition.

$\square$

### 5A.29

Suppose $𝑇 ∈ ℒ(𝐑^3)$ and $−4$, $5$, and $\sqrt{7}$ are eigenvalues of $𝑇$. 
Prove that
there exists $𝑥 ∈ 𝐑^3$ such that $𝑇𝑥 − 9𝑥 = (−4, 5, \sqrt{7})$.

**Proof**:

$−4$, $5$, and $\sqrt{7}$ are eigenvalues of $𝑇$, and from
5.12, we know operator cannot have more eigenvalues than dimension of
vector space. Since $\dim \mathbb{R}^3 = 3$, then $T$ cannot have other
eigenvalues, so $9$ is not an eigenvalue of $T$.

Since $9$ is not an eigenvalue of $T$, then $T - 9I$ is invertible.
Then we can find $x$ such that $(T - 9I) x = (−4, 5, \sqrt{7})$.

$\square$

### 5A.30

Suppose $𝑇 ∈ ℒ(𝑉)$ and $(𝑇 − 2𝐼)(𝑇 − 3𝐼)(𝑇 − 4𝐼) = 0$. Suppose 𝜆 is an
eigenvalue of $𝑇$. Prove that 𝜆 = 2 or 𝜆 = 3 or 𝜆 = 4.

**Proof**:

We prove by contradition.
Assume $k$ is an eigenvalue of $𝑇$, where $k \neq 2, 3, 4$.
If $v \neq 0$ is an eigenvector and $T(v) = k v$, then

$$ 
\begin{align*}
(𝑇 − 2𝐼)(𝑇 − 3𝐼)(𝑇 − 4𝐼)(v) &=
(k-4)(𝑇 − 2𝐼)(𝑇 − 3𝐼)(v) \\
&= (k-4) (k-3) (𝑇 − 2𝐼) (v) \\
&= (k-4) (k-3) (k-2) (v) \\
\end{align*}
$$

Since $k \neq 2, 3, 4, v \neq 0$, then $(k-4) (k-3) (k-2) (v) \neq 0$.

But this contradicts to the fact $(𝑇 − 2𝐼)(𝑇 − 3𝐼)(𝑇 − 4𝐼) = 0$.

So $k = 2$ or $k = 3$ or $k = 4$.

$\square$

### 5A.31

Give an example of $𝑇 ∈ ℒ(𝐑^2)$ such that $𝑇^4 = −𝐼$.

**Proof**:

Consider the matrix of $T$ is

$$ 
\mathcal{M}(T) =
\begin{bmatrix}
\sqrt[]{2}/2 & -\sqrt[]{2}/2 \\    
\sqrt[]{2}/2 &  \sqrt[]{2}/2 \\    
\end{bmatrix}
$$

Then since $\mathcal{M}(T)^4 = -I$ then $T^4 = -I$.

$\square$

### 5A.32

Suppose $𝑇 ∈ ℒ(𝑉)$ has no eigenvalues and $𝑇^4 = 𝐼$. Prove that
$𝑇^2 = −𝐼$.

**Proof**:

$$
\begin{align*}
0&=T^4 - I \\
&= (T^2 + I)(T + I)(T - I)
\end{align*}
$$

Since $T$ has no eigenvalues then $T-I, T+I$ are invertible.
So is $(T + I)(T - I)$.

So for any $u \in V$, we can find $v \in V$, such that

$$ 
u = (T + I)(T - I)(v)
$$

So $(T^2 + I)(u) = (T^2 + I)(T + I)(T - I)(v)=0$.

So $T^2 + I = 0$, then $𝑇^2 = −𝐼$.

$\square$

### 5A.33

Suppose $𝑇 ∈ ℒ(𝑉)$ and $𝑚$ is a positive integer.

(a) Prove that $𝑇$ is injective if and only if $𝑇^𝑚$ is injective.

**Proof**:

$\Rightarrow$

Assume $T$ is injective and if $T^m(u) = 0$, then
$0 = T^m(u) = T(T^{m-1}(u))$, we have $T^{m-1}(u) = 0$.
Similarly $T^{m-2}(u) = \cdots = T^2(u) = T(u) = 0$, so $u = 0$,
That means $T^{m}$ is injective.

$\Leftarrow$

Assume $T(u) = 0$ then $T^{m}(u) = T^{m-1}(T(u))=0$, so $u = 0$,
then $T$ is injective.

$\square$

(b) Prove that $𝑇$ is surjective if and only if $𝑇^𝑚$ is surjective.

**Proof**:

$\Rightarrow$

We prove by induction. First, $T$ is surjective.
Assume $T^k$ is surjective, and given $w \in V$.

Since $T^k$ is surjective, we can find $v \in V$ such that
$T^k(v) = w$. Since $T$ is also surjective, we can find
$u \in V$ such that $T(u) = v$, then $T^{k+1}(u) = T^k(T(u)) = T^k(v) = w$.

So $T^{k+1}$ is also surjective. Then we finish the induction.

$\Leftarrow$

$T^m$ is surjective, and given $w \in V$. We can find
$v \in V$ such that $T^{m}(v) = w$, then we have
$T(T^{m-1}(v)) = w$.

$\square$

### 5A.34

Suppose $𝑉$ is finite-dimensional and $𝑣_1, …, 𝑣_𝑚 ∈ 𝑉$.
Prove that the list
$𝑣_1, …, 𝑣_𝑚$ is linearly independent if and only if there exists
$𝑇 ∈ ℒ(𝑉)$ 
such that $𝑣_1, …, 𝑣_𝑚$ are eigenvectors of $𝑇$ corresponding to distinct 
eigenvalues.

**Proof**:

$\Leftarrow$

It is an immediate results from "5.11 linearly independent eigenvectors".

$\Rightarrow$

Since $V$ is finite-dimensional, and $𝑣_1, …, 𝑣_𝑚$ is linearly independent，
we can extend it to a basis of $V$ by adding $w_1, \cdots, w_n$.

Let $T(v_i) = i v_i$ and $T(w_i) = 0$, then $T$ is a linear map and
$𝑣_1, …, 𝑣_𝑚$ are eigenvectors of $𝑇$ corresponding to distinct 
eigenvalues

$\square$

### 5A.35

Suppose that $\lambda_{1}, …, \lambda_{𝑛}$ is a list of distinct real 
numbers. Prove that the
list $𝑒^{\lambda_{1}𝑥} , …, 𝑒^{\lambda_{𝑛}𝑥}$ is linearly independent in 
the vector space of real-valued functions on 𝐑.

Hint: Let
$𝑉 = \text{span}(𝑒^{\lambda_{1}𝑥} , …, 𝑒^{\lambda_{𝑛}𝑥})$,
and define an operator $𝐷 ∈ ℒ(𝑉)$ by
$𝐷 𝑓 = 𝑓'$. Find eigenvalues and eigenvectors of $𝐷$.

**Proof**:

Based on the hint, $Df = f'$ is a linear operator of $ℒ(𝑉)$. Also note
from calculus, we know

$$ 
D 𝑒^{\lambda_{1}𝑥} = \lambda_1 𝑒^{\lambda_{1}𝑥}
$$

Then $𝑒^{\lambda_{1}𝑥} , …, 𝑒^{\lambda_{𝑛}𝑥}$ are eigenvectors with
different eigenvalues.

From "5.11 linearly independent eigenvectors", we know
$𝑒^{\lambda_{1}𝑥} , …, 𝑒^{\lambda_{𝑛}𝑥}$ is linearly independent.

$\square$

### 5A.36

Suppose that $\lambda_1, …, \lambda_𝑛$ is a list of distinct positive 
numbers. Prove that
the list $\cos(\lambda_1𝑥), …, \cos(\lambda_𝑛𝑥)$ is linearly independent in 
the vector space of real-valued functions on 𝐑.

**Proof**:

We know that $Df = f''$ is a linear operator of $ℒ(𝑉)$.

Also note from calculus, we know

$$ 
D \cos(\lambda_i 𝑥) = -\lambda_i^2 \cos \lambda_i 𝑥
$$

Since $\lambda_i$ are distinct positive numbers, so $-\lambda_i^2$ are
also distinct.

From "5.11 linearly independent eigenvectors", we know
$\cos(\lambda_1𝑥), …, \cos(\lambda_𝑛𝑥)$ is linearly independent.

$\square$

### 5A.37

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$. Define $𝒜 ∈ ℒ(ℒ(𝑉))$ by
$𝒜(𝑆) = 𝑇𝑆$ for each $𝑆 ∈ ℒ(𝑉)$. Prove that the set of eigenvalues of 
$𝑇$ equals the set of eigenvalues of $𝒜$.

**Proof**:

Assume $\lambda$ is an eigenvalue of $T$. Then we can find $u \neq 0$, such
that $T(u) = \lambda u$.
We need to fine $S$ such that $𝒜(S) = \lambda S$.

Let $v_1, \cdots, v_m$ be a basis of $V$, let $S(v_i) = u$, then $S \in ℒ(𝑉)$.

$$ 
\begin{align*}
TS(a_1 v_1 + \cdots + a_m v_m) &=
T(a_1 Sv_1 + \cdots + a_m Sv_m) \\
&= T(a_1 u + \cdots + a_m u) \\
&= a_1 Tu + \cdots + a_m Tu \\
&= a_1 \lambda u + \cdots + a_m \lambda u \\
&= \lambda (a_1 u + \cdots + a_m u) \\
&= \lambda (a_1 Sv_1 + \cdots + a_m Sv_m) \\
&= \lambda S(a_1 v_1 + \cdots + a_m v_m)
\end{align*} 
$$

So $𝒜(S) = \lambda S$.

Now assume $\lambda$ is an eigenvalue of $𝒜$, then we can find $S \neq 0$,
such that $TS = \lambda S$.

Since $S \neq 0$, we can find $v \in \text{range } S$ such that $v \neq 0$.
Let $S(u) = v$, then

$$ 
\begin{align*}
T(v) &= TS(u) \\
&= \lambda S(u) \\
&= \lambda v
\end{align*} 
$$

So $\lambda$ is an eigenvalue of $T$.

$\square$

### 5A.38

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉)$, and $𝑈$ is a subspace of 
$𝑉$ invariant under $𝑇$. The quotient operator $𝑇/𝑈 ∈ ℒ(𝑉/𝑈)$ is defined 
by

$$ 
(T/U)(v + U) = Tv + U
$$

for each $v \in V$.

(a) Show that the definition of $𝑇/𝑈$ makes sense (which requires using the
condition that $𝑈$ is invariant under 𝑇) and show that $𝑇/𝑈$ is an operator
on $𝑉/𝑈$.

**Proof**:

Assume $u+U = v+U$, then from
"3.101 two translates of a subspace are equal or disjoint",
we know $u-v \in U$.

$$
\begin{align*}
(T/U)(v + U) &= Tv + U \\
(T/U)(u + U) &= Tu + U \\
(Tv+U) - (Tu+U) &= (Tv - Tu) + U \\ 
&= T(v-u) + U \\ 
&= U & \text{ since } u-v \in U \text{ which is invariant under } T\\ 
\end{align*} 
$$

So $T/U$ is well defined.

Next, we will prove $T/U$ is linear map.

First

$$ 
\begin{align*}
(T/U)((u+U)+(v+U))
&=(T/U)((u+v)+U) \\
&= T(u+v) + U \\
&= (T(u) + T(v)) + U \\
&= (T(u) + U) + (T(v) + U) \\
&= (T/U)(u+U) + (T/U)(v+U) \\
\end{align*} 
$$

Second

$$ 
\begin{align*}
(T/U)(a(u+U)) 
&= (T/U)(au + U) \\
&= T(au) + U \\
&= aT(u) + U \\
&= a(T(u) + U) \\
&= a((T/U)(u+U)) \\
\end{align*} 
$$

$\square$

(b) Show that each eigenvalue of $𝑇/𝑈$ is an eigenvalue of $𝑇$.

**Proof**:

Assume $k$ is an eigenvalue of $T/U$. Then $T/U - kI$ is not injective,
so we can find $u \not\in U$ such that $(T/U-kI)(u+U) = (T-kI)(u) + U = 0+U$,
that means we can find $v \in U$ such that $(T-kI)(u) = v \in U$.

Since $U$ is invariant under $T$,
so we can consider $T$ limited on $U$, i.e. $T|_U$. 

If $(T|_U-kI)$ is not invertible, we can find $w \in U$ and $w \neq 0$,
such that $(T|_U-kI)(w) = 0$, since $T|_U(w) = T(w)$.
Then $(T-kI)(w) = 0$. So $k$ is eigenvalue of $T$.

If $(T|_U-kI)$ is invertible, we can find $w \in U$ such that
$(T|_U-kI)(w) = v$, then we also have $(T-kI)(w) = v$.

Since $u \not\in U, w \in U$, we have $u-w \neq 0$.
And $(T-kI)(u-w) = (T-kI)(u) - (T-kI)(w) = v - v = 0$.

Therefore, $k$ is an eigenvalue of $T$.

$\square$

### 5A.39

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$. Prove that $𝑇$ has an 
eigenvalue if and only if there exists a subspace of $𝑉$ of dimension
$\dim 𝑉 − 1$ that is invariant under $𝑇$.

**Proof**:

$\Leftarrow$

Let $U$ be a invariant space under $T$ and $\dim U = \dim V - 1$.

Then consider the quotient space $V/U$ and the operator $T/U$ on it defined
in the last exercise.

Since $\dim V/U = \dim V - \dim U = 1$, then $T/U$ has an eigenvalue.
From the previous exercise part (b), each eigenvalue of $𝑇/𝑈$ is an 
eigenvalue of $𝑇$. So $T$ has an eigenvalue. 

$\Rightarrow$

We will use induction. Let $m = \dim V$.
First if $m = 1$, then $\{0\}$ is invariant and it's dimension is $0 = m - 1$.
The statement is true.

Now assume the statement holds for all $m \leq n$, and we will prove
when $m = n + 1$.

Assume $k$ is an eigenvalue, consider the linear mapping $T-kI$.

Consider $\text{range } T- kI$. From
"5.18 null space and range of $𝑝(𝑇)$ are invariant under $𝑇$", we know
$\text{range } T- kI$ is invariant under $T$.

Since $T-kI$ is not surjective, then $\text{dim range } T-kI < n+1$

If $\text{dim range } T-kI = n$, then we are done.

If $\text{dim range } T-kI < n$, then from
fundamental theorem of linear maps (3.21), we know
$\text{dim null } T-kI \geq 2$.

Then we can find $v_1, v_2 \in \text{null } T-kI$ which are linear independent.

Let $U = \text{span}(𝑣_1)$

Now we can use exercise 5A.38 and consider the quotient space $V/U$ and
its operator $T/U$.

Note that $k$ is an eigenvalue of $T/U$ and $v_2+U$ is an eigenvector since

$$
\begin{align*}
(T/U)(v_2+U) &= T(v_2) + U \\
&= k v_2 + U \\
&= k (v_2 + U) 
\end{align*} 
$$

Since $\dim U = 1$, then $\dim V/U = \dim V - \dim U = (n+1)-1 = n$.
And $T/U$  has an eigenvalue $k$, so we can apply the induction and get
an invariant subspace $W'$ and $\dim W' = n-1$.

Now assume $w_1+U, \cdots, w_{n-1}+U$ is a basis of $W'$.

Then we can cosider the space $W = \text{span}(w_1, \cdots, w_{n-1}, v_1)$.

Since $W'$ is invariant under $T/U$, then we have

$$ 
\begin{align*}
T(w_i) + U &= (T/U)(w_i+U) \\
&= a_1 (w_1+U) + \cdots + a_{n-1} (w_{n-1}+U) \\
&= (a_1 w_1 + \cdots + a_{n-1} w_{n-1}) + U
\end{align*} 
$$

And since $U = \text{span}(𝑣_1)$, it means

$$ 
T(w_i) = a_1 w_1 + \cdots + a_{n-1} w_{n-1} + a_n v_1 \in W
$$

Also $T(v_1) = k v_1 \in W$. So $W$ is invariant under $T$.

Now if

$$
\begin{align*}
a_1 w_1 + \cdots + a_{n-1} w_{n-1} + a_n v_1 &= 0 \\
&\Rightarrow \\
a_1 w_1 + \cdots + a_{n-1} w_{n-1} &= -a_n v_1 \\
&\Rightarrow \\
(a_1 w_1 + \cdots + a_{n-1} w_{n-1}) + U &= -a_n v_1 + U \\
&\Rightarrow \\
a_1 (w_1+U) + \cdots + a_{n-1} (w_{n-1}+U) &= 0 + U \\
&\Rightarrow \\
a_1 = \cdots = a_{n-1} &= 0 \\ 
&\Rightarrow \\
a_n &= 0 \text{ as well}
\end{align*} 
$$

So $w_1, \cdots, w_{n-1}, v_1$ are linear independent.

The $\dim W = n$, this completes the induction.

$\square$

Here is the anwser from AI:

Let $k$ be an eigenvalue of $T$ and let
$W = range(T − kI)$. By 5.18, $W$ is invariant 
under $T$. Since $T − kI$ is not surjective 
($k$ is an eigenvalue, so $T − kI$ is not 
injective, and $V$ is finite-dimensional),
$\dim W < \dim V$.

Case 1: $\dim W = \dim V − 1$. Then $W$ is the desired invariant subspace.

Case 2: $\dim W < \dim V − 1$.

Since $W$ is invariant under $T$, the quotient operator $T/W ∈ L(V/W)$ is well-defined. For any $v ∈ V$:

$$
\begin{align*}
(T/W)(v+W) &= Tv + W \\
&= kv + (T-kI)v + W \\
&= k(v + W)
\end{align*} 
$$

So $(T/W) = kI$.

Let $Z = π⁻¹(Z')$ be the preimage of $Z'$ under the quotient map $π : V → V/W$.

Then $Z$ is invariant under $T$, for $z \in Z$,

$$ 
\begin{align*}
π(T(z)) &= T(z) + W \\
&= (T/W)(z+W) \\
&= k(z+W) \\
&= k π(z) \\
&\in Z' \\
&\Rightarrow \\
T(z) &\in Z
\end{align*} 
$$

Then note $\text{null } \pi = W$ and
$\text{range } \pi = Z'$

So $\dim Z = \dim W + \dim Z' = n-1$.

$\square$

### 5A.40

Suppose $𝑆, 𝑇 ∈ ℒ(𝑉)$ and $𝑆$ is invertible. Suppose $𝑝 ∈ 𝒫(𝐅)$ is a 
polynomial.
Prove that

$$ 
𝑝(𝑆𝑇𝑆^{−1}) = 𝑆𝑝(𝑇)𝑆^{−1}
$$

**Proof**:

Note since $𝑆$ is invertible, then $SS^{-1} = I$.

So $(STS^{-1})^n = (STS^{-1}) \cdots (STS^{-1}) = ST^nS^{-1}$.

If $p(z) = a_0 + a_1 z + \cdots + a_{m} z^{m}$

Then

$$ 
\begin{align*}
𝑝(𝑆𝑇𝑆^{−1}) &= a_0 + a_1 (𝑆𝑇𝑆^{−1}) + \cdots + a_{m} (𝑆𝑇𝑆^{−1})^{m} \\
&= a_0 SS^{-1} + a_1 (𝑆𝑇𝑆^{−1}) + \cdots + a_{m} (𝑆𝑇^{m}𝑆^{−1}) \\
&= S(a_0 + a_1 T + \cdots + a_{m} T^{m})S^{-1} \\
&= 𝑆𝑝(𝑇)𝑆^{−1}
\end{align*} 
$$

$\square$

### 5A.41

Suppose $𝑇 ∈ ℒ(𝑉)$ and $𝑈$ is a subspace of $𝑉$ invariant under $𝑇$. 
Prove that $𝑈$ is invariant under $𝑝(𝑇)$ for every polynomial $𝑝 ∈ 𝒫(𝐅)$.

**Proof**:

We use the induction to show $U$ is invariant under $T^n$.
Since $U$ is invariant under $T$, assume $U$ is invariant under $T^n$.

For any $u \in U$, since $T^n(u) \in U$, then $T^{n+1}(u) = T(T^n(u)) \in U$,
so $U$ is invariant under $T^{n+1}$.

Then given any $u \in U$, $a_nT^{n}(u) \in U$.

$$ 
\begin{align*}
p(T)(u) &= (a_0 + a_1 T + \cdots + a_{m} T^{m})(u) \\
&= a_0(u) + a_1 T(u) + \cdots + a_{m} T^{m}(u) \\
& \in U
\end{align*} 
$$

So $𝑈$ is invariant under $𝑝(𝑇)$ for every polynomial $𝑝 ∈ 𝒫(𝐅)$.

$\square$

### 5A.42

Define $𝑇 ∈ ℒ(𝐅^𝑛)$ by
$𝑇(𝑥_1, 𝑥_2, 𝑥_3, …, 𝑥_𝑛) = (𝑥_1, 2𝑥_2, 3𝑥_3, …, 𝑛𝑥_𝑛)$.

(a) Find all eigenvalues and eigenvectors of 𝑇.

**Proof**:

For any $i$ such that $1 \leq i \leq n$, $i$ is an eigenvalue, because
let $e_i$ be the ith item of standard basis of $𝐅^𝑛$.

$$ 
T(e_i) = i \cdot e_i
$$

Since $\dim 𝐅^𝑛 = n$, then $T$ can only have $n$ distinct eigenvalues.
Then we found all eigenvalue.

If $v = a_1 e_1 + \cdots + a_n e_n$ is an eigenvector with eigenvalue of $i$,
then

$$
\begin{align*}
i v &= T(v) \\
&= a_1 Te_1 + \cdots + a_n Te_n \\
&= 1 a_1 e_1 + \cdots + n a_n e_n \\
& \Rightarrow \\
(1-i)a_1 e_1 + \cdots + (n-i) a_n e_n &= 0 \\
& \Rightarrow \\
(k-i) a_k &= 0 \\
& \Rightarrow \\
a_k &= \begin{cases}
    0 &\text{if } k \neq i \\
    \text{anything } &\text{if } k = i\\
\end{cases} 
\end{align*} 
$$

so $v = a_i e_i$ with $a_i \neq 0$. That's all eigenvectors of $T$.

$\square$

(b) Find all subspaces of $𝐅^𝑛$ that are invariant under $𝑇$.

**Solution**:

Assume $U$ is invariant under $T$ and
$v \in U$ and $v \neq 0$, let

$$ 
v = a_1 e_1 + \cdots + a_n e_n
$$

If $a_i \neq 0$, we want to show $e_i \in U$.
If $a_j = 0$ when $j \neq i$, then $a_i^{-1}v = e_i \in U$, we are done.

Other we have some $a_j \neq 0$ with $j \neq i$.

Since $U$ is invariant subspace, then $T(\frac{1}{j} v) \in U$,
so we have $v - T(\frac{1}{j}v) \in U$.
We also have

$$ 
\begin{align*}
v - T(\frac{1}{j}v) &=
(a_1 e_1 + \cdots + a_n e_n) - \frac{1}{j}(a_1 Te_1 + \cdots + a_n Te_n) \\
&= \sum \limits_{k=1}^{n} (1-k/j)a_k e_k \\
&= \sum \limits_{k=1}^{n} b_k e_k
\end{align*} 
$$

So, for $v - T(\frac{1}{j}v)$, $b_i \neq 0$ but $b_j = 0$.
For other $k \neq i, j$, if $a_k \neq 0$ then $b_k = (1-k/j)a_k \neq 0$.
If $a_k = 0$, then $b_k = (1-k/j)a_k = 0$.

So the number of non zero coefficients is reduced by $1$.
By continuing this process, we can show $e_i \in U$.

That means $\text{span}(e_i, \cdots, e_j) \subseteq U$, on the other hand
$u = a_1 e_1 + \cdots + a_n e_n$. So $U \subseteq \text{span}(e_i, \cdots, e_j)$.

That means all subspaces of $𝐅^𝑛$ that are invariant under $𝑇$ are
the form of $\text{span}(e_i, \cdots, e_j)$.

$\square$

### 5A.43

Suppose that $𝑉$ is finite-dimensional,
$\dim 𝑉 > 1$, and $𝑇 ∈ ℒ(𝑉)$. Prove that
$\{𝑝(𝑇) ∶ 𝑝 ∈ 𝒫(𝐅)\} ≠ ℒ(𝑉)$.

**Proof**: 

Assume $\dim V = n$.

One strategy is that: since $\dim L(V) = n^2$, we should prove
$\dim \{𝑝(𝑇) ∶ 𝑝 ∈ 𝒫(𝐅)\} < n^2$.

We will use the results from section about next section, i.e. section 5.3.

Assume $p(z)$ is the minimal polynomial of $T$. Then from 5.22 we know
$\deg p \leq n$.

Given any $q(z)$, from 4.9 division algorithm for polynomials, we know we
can find $s(z), r(z)$ such that $q(z) = s(z)p(z) + r(z)$, where
$\deg r < n$.

That means $q(T) = s(T)p(T) + r(T)$, since $p(T) = 0$, then $q(T) = r(T)$.

Since $\deg r < n$, then we have

$$
\begin{align*}
\{𝑝(𝑇) ∶ 𝑝 ∈ 𝒫(𝐅)\} &= \text{span}(I, T, \cdots, T^{n-1}) \\
&\Rightarrow \\
\dim \{𝑝(𝑇) ∶ 𝑝 ∈ 𝒫(𝐅)\} &\leq n
\end{align*}
$$

Since $n > 1$, then $n < n^2$.

$\square$

Another strategy (not working so far) is
we should find some $p$ such that $\text{range } p(T)$ or $\text{null } p(T)$
is not trivial invariant subspace.

We consider the $U = \text{null } T$. Since we know from
exercise 5A.41, $U$ is invariant under $p(T)$,
we want to find a operator
$S$ such that $U$ is not invariant under $S$.

Case 1: $U = V$, then $T = 0$, then $p(T) = kI$. Let $v_1, v_2 \in V$ be
linear independent, then let $S(v_1) = v_2, S(v_2) = v_1$, then $S \neq kI = P(T)$.

Case 2: $U \subset V$, we can find a basis of $U$: $u_1, \cdots, u_m$.
We can also extend it to a basis of $V$ by adding $v_1, \cdots, v_n$.
Let $S(u_i) = v_1$, then $U$ is not invariant under $S$.

$\square$

## Section 5B The Minimal Polynomial

### 5B.1

Suppose $𝑇 ∈ ℒ(𝑉)$. Prove that $9$ is an eigenvalue of $𝑇^2$ if and only if $3$ or
$−3$ is an eigenvalue of $𝑇$.

**Proof**:

$\Rightarrow$

Assume $u \neq 0$ is an eigenvector and $(T^2 - 9I)(u) = 0$.
Then we have $(T-3I)(T+3I)(u) = 0$.

If $(T+3I)(u) = 0$, then $-3$ is an eigenvalue and $u$ is an eigenvector.

If $(T+3I)(u) \neq 0$, let $w = (T+3I)(u)$. We have $(T-3I)(w) = 0$.
Then $+3$ is an eigenvalue and $w$ is an eigenvector.

$\Leftarrow$

If $3$ is an eigenvalue and $u \neq 0$ is an eigenvector such that
$(T-3I)(u) = 0$, then

$$
\begin{align*}
(T^2 - 9I)(u) &=
(T+3I)(T-3I)(u) \\
&= (T+3I)(0) \\
&= 0
\end{align*} 
$$

So $9$ is an eigenvalue of $𝑇^2$ and $u$ is an eigenvector.
Similarly for the case when $−3$ is an eigenvalue of $𝑇$.

$\square$

### 5B.2

Suppose $𝑉$ is a complex vector space and $𝑇 ∈ ℒ(𝑉)$ has no eigenvalues.
Prove that every subspace of $𝑉$ invariant under $𝑇$ is either $\{0\}$ or infinite-
dimensional.

**Proof**:

Assume $U \subseteq V$ is subspace that is invariant under $T$.
Then we can restrict $T$ under $U$ to get $T|_U$.
Then $T|_U$ is an operator on $U$.

Assume $U \neq \{0\}$ is a finite-dimensional space.

Then from "5.19 existence of eigenvalues", it must have an eigenvalue $\lambda$ and an
eigenvector of $u \neq 0$ such that $T|_U(u) = \lambda u$.

But since $u \in U$, then we also have $T(u) = T|_U(u) = \lambda u$.
This means $T$ has an eigenvalue $\lambda$ and an eigenvector of $u \neq 0$.

Then we reached an contradition. So if $U \neq \{0\}$, then $U$ is infinite-dimensional.

$\square$

### 5B.3

Suppose $𝑛$ is a positive integer and $𝑇 ∈ ℒ(𝐅^𝑛)$ is defined by

$$ 
T (x_1, \cdots, x_n) =
(𝑥_1 +⋯ + 𝑥_𝑛, …, 𝑥_1 +⋯ + 𝑥_𝑛)
$$

anwser the following:

(a) Find all eigenvalues and eigenvectors of $𝑇$.

**Solution**:

Assume $k$ is an eigenvalue and $(x_1, \cdots, x_n) \neq 0$ is an eigenvector,

Then

$$
\begin{align*}
T (x_1, \cdots, x_n) &=
(𝑥_1 +⋯ + 𝑥_𝑛, …, 𝑥_1 +⋯ + 𝑥_𝑛) \\
&= k (x_1, \cdots, x_n)
\end{align*} 
$$

Then we have

$$ 
k x_1 = k x_2 = \cdots = k x_n = 𝑥_1 +⋯ + 𝑥_𝑛
$$

If $k = 0$, then any $(x_1, \cdots, x_n) \neq 0$ satisfy $𝑥_1 +⋯ + 𝑥_𝑛 = 0$, is an eigenvector.
So if $n = 1$, then $x_1 = 0$, then $0$ is not an eigenvalue.

If $k \neq 0$, then $x_1 = x_2 = \cdots = x_n = a \neq 0$ and $k = n$.

So in summary, there are 2 possible eigenvalues when $n > 1$:

1. $k = 0$, and $(x_1, \cdots, x_n) \neq 0$ satisfy $𝑥_1 +⋯ + 𝑥_𝑛 = 0$
2. $k = n$, and $(x_1, \cdots, x_n) = (a, \cdots, a)$ with $a \neq 0$.

if $n = 1$, then only case 2 is valid. 

$\square$

(b) Find the minimal polynomial of 𝑇.

**Solution**:

We first assume $n > 1$.

Let $p(z)$ be the minimal polynomial of $𝑇$.

From "5.27 eigenvalues are the zeros of the minimal polynomial", we know

$$ 
p(z) = z(z-n)q(z)
$$

This means $p(z)$ is a multiple of $z(z-n)$.

Now we consider $(T-nI)T$ applied on $e_i$ where $e_i$ is one of the standard basis.

$$
\begin{align*}
(T-nI)T(e_i) &=
(T-nI) (1, \cdots , 1) \\
&= (n, \cdots , n) - (n, \cdots , n) \\
&= 0
\end{align*} 
$$

Then $(T-nI)T(v) = 0$ for any $v \in F^n$. That means $(T-nI)T = 0$.

Then from "5.29 $𝑞(𝑇) = 0 ⟺ 𝑞$ is a polynomial multiple of the minimal polynomial", we know
$z(z-n)$ is a multiple $p(z)$.

Since $z(z-n)$ is a monic polynomial, $p(z) \mid z(z-n)$ and $z(z-n) \mid p(z)$ we must have $p(z) = z(z-n)$.

Now we assume $n = 1$. In this case $T-I = 0$ because $(T-I)(v) = T(v) - v = v - v = 0$.
so $p(z) \mid z - 1$. On the other hand $1$ is a zero of $p(z)$ so $z - 1 \mid p(z)$.
So $p(z) = z - 1$.

$\square$

### 5B.4

Suppose $𝐅 = 𝐂, 𝑇 ∈ ℒ(𝑉), 𝑝 ∈ 𝒫(𝐂)$, and 𝛼 ∈ 𝐂. Prove that 
𝛼 is an
eigenvalue of 𝑝(𝑇) if and only if 𝛼 = 𝑝(𝜆) for some eigenvalue 
𝜆 of 𝑇.

**Proof**:

$\Rightarrow$

Consider the polynomial $p(z) - \alpha \in 𝒫(𝐂)$.
And consider $U = \text{null } p(T) - \alpha I$.
Since $𝛼$ is an eigenvalue of $𝑝(𝑇)$,
$U \neq \{0\}$.

From "5.18 null space and range of $𝑝(𝑇)$ are invariant under $𝑇$", we know $U$ is invariant under $T$.
And then we can restrict $T$ on $U$ to get $T|_U$.

Let $q(z)$ be the minimal polynomial of $T|_U$.
Since $p(T|_U) - \alpha$ is $0$ on $U$,
from
"5.29 $𝑞(𝑇) = 0 ⟺ 𝑞$ is a polynomial multiple of the minimal 
polynomial",
we have $q \mid p(z) - \alpha$ 

Since $q(z) \in 𝒫(𝐂)$, from fundamental theorem of algebra,
we can find one of its zero, say $\lambda$.

So $q(z) = (z-\lambda)s(z)$. Since $\deg s < \deg q$,
then $s(z)$ is not a multiple of $q$, then $s(T|_U)$
is not $0$ on $U$ again from 5.29. We can find $v \in U$, such that
$s(T|_U)(v) \neq 0$. Let $w = s(T|_U)(v)$, then we have
$(T|_U - \lambda I)(w) = 0$.

Since $w \in U$, then we have $T(w) = T|_U(w)$, so
$(T-\lambda I)(w) = (T|_U - \lambda I ) (w) = 0$,
i.e. $T(w) = \lambda w$.
So $\lambda$ is an eigenvalue of $T$.

Since $q \mid p(z) - \alpha$ and $\lambda$ is a zeor of $q$,
we have $p(\lambda) - \alpha = 0$.

$\Leftarrow$

If $𝛼 = 𝑝(𝜆)$, and $T(u) = \lambda u$, then

$$
\begin{align*}
p(T)(u) &= (a_0 I + a_1 T + \cdots + a_{m} T^{m})(u) \\
&= a_0 I(u) + a_1 T(u) + \cdots + a_{m} T^{m}(u) \\
&= a_0 u + a_1 \lambda(u) + \cdots + a_{m} \lambda^{m}(u) \\
&= (a_0 + a_1 \lambda + \cdots + a_{m} \lambda^{m})(u) \\
&= \alpha u
\end{align*} 
$$

So $𝛼$ is an eigenvalue of $𝑝(𝑇)$.

$\square$

### 5B.5

Give an example of an operator on $𝐑^2$ that shows the result in Exercise 4 does not hold if 𝐂 is replaced with 𝐑.

**Solution**:

Consider $T$ is an operator, it rotates a vector $(x, y)$ by
90 degree counterclock-wise.

So $T(1,0) = (0,1), T(0,1) = (-1,0)$.

So $T^2(1,0) = T(0,1) = (-1,0)$, then
if we reuse the symbol in exercise 4,
we have $p(z) = z^2, \alpha = -1$, then it's not possible to
find a real number $\lambda$ such that
$p(\lambda) = \lambda^2 = -1$.

$\square$

### 5B.6

Suppose $𝑇 ∈ ℒ(𝐅^2)$ is defined by $𝑇(𝑤, 𝑧) = (−𝑧, 𝑤)$.
Find the minimal polynomial of $𝑇$.

**Solution**:

Consider

$$
\begin{align*}
T(1,0) &= (0, 1) \\
T^2(1,0) &= T(0, 1) \\
&= (-1, 0)
\end{align*}  
$$

And

$$
\begin{align*}
T(0,1) &= (-1, 0) \\
T^2(0,1) &= T(-1, 0) \\
&= (0, -1)
\end{align*}  
$$

That means $T^2(e_1) + e_1 = 0$ and $T^2(e_2) + e_2 = 0$.

So $T^2 + 1 = 0$. so $T^2 + 1$ is a multiple of minimal polynomial.

On the other hand, if $T+\lambda I$ is $0$, then

$$
\begin{align*}
(T+\lambda I)(e_1) &= 0 \\
& \Rightarrow \\
(0, 1) &= (-\lambda, 0)
\end{align*} 
$$

This is no possible, so $T+\lambda I \neq 0$.

So $T^2 + 1$ is the minimal polynomial.

$\square$

### 5B.7

(a) Give an example of $𝑆, 𝑇 ∈ ℒ(𝐅^2)$ such that the minimal 
polynomial of $𝑆𝑇$ does not equal the minimal polynomial of 
$𝑇𝑆$.

**Solution**:

Consider $S(x,y) = (x, x)$ and $T(x,y)=(0,x)$.

Then $ST(x,y)=S(0,x)=(0,0)$ so $ST = 0$, then
the minimal polynomial of $ST$ is $z$.

On the other hand,

$TS(x,y) = T(x,x) = (0,x)$, so
$(TS)^2(1,0) = (TS)(0,1) = (0,0)$, and
$(TS)^2(0,1) = (TS)(0,0) = (0,0)$, so
the minimal polynomial of $TS$ is $z^2$.

$\square$

(b) Suppose $𝑉$ is finite-dimensional and $𝑆, 𝑇 ∈ ℒ(𝑉)$.
Prove that if at least
one of $𝑆, 𝑇$ is invertible, then the minimal polynomial of
$𝑆𝑇$ equals the minimal polynomial of $𝑇𝑆$.

Hint: Show that if 𝑆 is invertible and 𝑝 ∈ 𝒫(𝐅), then
$𝑝(𝑇𝑆) = 𝑆^{−1}𝑝(𝑆𝑇)𝑆$.

**Proof**:

Assume $S$ is invertible.
$p$ is the minimal polynomial of $𝑆𝑇$.
$q$ is the minimal polynomial of $TS$.

We will show $p(TS) = 0$ and $q(ST) = 0$.

Just use exercise 5A.40,

$$ 
\begin{align*}
p(TS) &= p(S^{-1}STS) \\
&= 𝑆^{−1}𝑝(𝑆𝑇)𝑆 \\
&= 𝑆^{−1} 0 S \\
&= 0
\end{align*} 
$$

Then use
"5.29 $𝑞(𝑇) = 0 ⟺ 𝑞$ is a polynomial multiple of the minimal 
polynomial", we know $p$ is an multiple of $q$.

On the other hand,

$$ 
\begin{align*}
q(ST) &= q(STSS^{-1}) \\
&= S q(TS) S^{-1} \\
& = S 0 S^{-1} \\
& = 0
\end{align*} 
$$

So $q$ is a multiple of $p$.

In summary, $p = q$.

$\square$

### 5B.8

Suppose $𝑇 ∈ ℒ(𝐑^2)$ is the operator of counterclockwise rotation
by $1^∘$. Find the minimal polynomial of $𝑇$.

Because $\dim 𝐑^2 = 2$, the degree of the minimal polynomial of
$𝑇$ is at most $2$.
Thus the minimal polynomial of $𝑇$ is not the tempting polynomial 
$𝑥^{180} + 1$, even though $𝑇^{180} = −𝐼$.

**Solution**:

We write the standard basis in polar form

$$ 
e_1 = (1, 0) = (\cos 0^\circ, \sin 0^\circ) \\
e_2 = (0, 1) = (\cos 90^\circ , \sin 90^\circ) \\
$$

Then note

$$
\begin{align*}
T^2(e_1) &= (\cos 2^\circ , \sin 2^\circ) \\
T^2(e_1) + e_1 &= (\cos 2^\circ , \sin 2^\circ) +
(\cos 0^\circ, \sin 0^\circ)\\
&= (2 \cos 1 ^ \circ \cos 1 ^ \circ,
2 \sin 1 ^\circ \cos 1 ^ \circ ) \\
&= 2 \cos 1^ \circ (\cos 1^\circ , \sin 1^\circ) \\
&= 2 \cos 1^ \circ T(e_1)
\end{align*} 
$$

Similarly,

$$
\begin{align*}
T^2(e_2) + e_2 &= (\cos 90^\circ , \sin 90^\circ) +
(\cos 92^\circ, \sin 92^\circ) \\
&= (2 \cos 91 ^ \circ \cos 1 ^ \circ,
2 \sin 91 ^\circ \cos 1 ^ \circ ) \\
&= 2 \cos 1^ \circ (\cos 91^\circ , \sin 91^\circ) \\
&= 2 \cos 1^ \circ T(e_2) \\
\end{align*} 
$$

So $T^2 - 2 \cos 1^ \circ T + I = 0$.

On the other hand, since $T$ is a rotation,
$T$ does not have eigenvalue, so the minimal polynomial
cannot be degree 1.

Therefore, the minimal polynomial is
$p(z) = z^2 - 2 \cos 1^ \circ z + 1$.

$\square$

### 5B.9

Suppose $𝑇 ∈ ℒ(𝑉)$ is such that with respect to some basis of 
$𝑉$, all entries
of the matrix of $𝑇$ are rational numbers. Explain why all 
coefficients of the
minimal polynomial of $𝑇$ are rational numbers.

**Proof**: unsolved.

### 5B.10

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉)$, and
$𝑣 ∈ 𝑉$. Prove that

$$ 
\text{span}(𝑣, Tv, \cdots, T^𝑚v) =
\text{span}(𝑣, Tv, \cdots, T^{\dim V - 1} v)
$$

for all integers $𝑚 ≥ \dim 𝑉 − 1$.

**Proof**:

Let $p$ be the minimal polynomial of $T$, from the
polynomial division algorithm, we know given $z^m$,
we can find $s(z), r(z)$ such that

$$ 
z^m = p(z)s(z) + r(z)
$$

with $\deg r < \deg p \leq \dim V$.
So $\deg r \leq \dim V - 1$.
Let $\deg r = n$.

So we have

$$ 
\begin{align*}
T^m &= p(T)s(T) + r(T) \\
& = 0 + r(T) \\
& = r(T) \\
& = a_0 I + a_1 T + \cdots + a_{n} T^{n}
\end{align*}
$$

So $T^m(v) = (a_0 I + a_1 T + \cdots + a_{n} T^{n})(v)
\in \text{span}(𝑣, Tv, \cdots, T^{\dim V - 1} v).$
That means

$$ 
\text{span}(𝑣, Tv, \cdots, T^𝑚v) \subseteq
\text{span}(𝑣, Tv, \cdots, T^{\dim V - 1} v)
$$

On the other hand, since $𝑚 ≥ \dim 𝑉 − 1$, we have

$$ 
\text{span}(𝑣, Tv, \cdots, T^𝑚v) \supseteq 
\text{span}(𝑣, Tv, \cdots, T^{\dim V - 1} v)
$$

So we have

$$ 
\text{span}(𝑣, Tv, \cdots, T^𝑚v) =
\text{span}(𝑣, Tv, \cdots, T^{\dim V - 1} v)
$$

$\square$

### 5B.11

Suppose $𝑉$ is a two-dimensional vector space, $𝑇 ∈ ℒ(𝑉)$,
and the matrix of $𝑇$ with respect to some basis of $𝑉$ is
$$ 
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
$$

Prove that

(a) Show that $𝑇^2 − (𝑎 + 𝑑)𝑇 + (𝑎𝑑 − 𝑏𝑐)𝐼 = 0$.

**Proof**:

$$ 
\begin{align*}
T^2 &=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}^2 \\
&=
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix}
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix} \\
&=
\begin{pmatrix}
a^2 + bc & ab + bd \\
ac + cd  & bc + d^2 \\
\end{pmatrix} \\
\end{align*} 
$$

$$ 
\begin{align*}
(a+d)T &=
(a+d)
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix} \\
&=
\begin{pmatrix}
a^2 + ad & ab + bd \\
ac + cd  & ad + d^2 \\
\end{pmatrix}
\end{align*} 
$$

$$ 
\begin{align*}
(𝑎𝑑 − 𝑏𝑐)𝐼 &=
\begin{pmatrix}
ad-bc & 0 \\
0  & ad-bc \\
\end{pmatrix}
\end{align*} 
$$

So $𝑇^2 − (𝑎 + 𝑑)𝑇 + (𝑎𝑑 − 𝑏𝑐)𝐼 = 0$.

(b) Show that the minimal polynomial of $𝑇$ equals

$$ 
\begin{cases}
    z-a &\text{if } b=c=0 \text{ and } a=d\\
    z^2 - (a+d)z + (ad - bc) &\text{otherwise}\\
\end{cases}
$$

**Proof**:

Assume the minimal polynomial of $T$ is $p$.

If $\deg T = 1$ then assume
$T + \lambda I = 0$.

$$
\begin{align*}
0 &= 
\begin{pmatrix}
a & b \\
c & d \\
\end{pmatrix} + \lambda I \\
&=
\begin{pmatrix}
a + \lambda  & b \\
c & d + \lambda \\
\end{pmatrix}
\end{align*} 
$$

So $a = d = -\lambda$, $b = c = 0$.

If $\deg T = 2$, then from part (2) we know
$𝑇^2 − (𝑎 + 𝑑)𝑇 + (𝑎𝑑 − 𝑏𝑐)𝐼 = 0$, since
minimal polynomial is unique, then
$z^2 - (a+d)z + (ad - bc)$ is the minimal polynomial.

$\square$

### 5B.12

Define $𝑇 ∈ ℒ(𝐅^𝑛)$ by
$𝑇(𝑥_1, 𝑥_2, 𝑥_3, …, 𝑥_𝑛) = (𝑥_1, 2𝑥_2, 3𝑥_3, …, 𝑛𝑥_𝑛)$.
Find the minimal polynomial of $𝑇$.

**Proof**:

Let $p$ be the minimal polynomial of $T$.

Let $e_1, \cdots, e_n$ be the standard basis of $F^n$.
Then note $T(e_i) = i e_i$, then $i$ is an eigenvalue of $T$.

So from "5.27 eigenvalues are the zeros of the minimal polynomial",
part (b)
$p$ has the form of $(z-1)^{i_1}\cdots(z-n)^{i_n}$.
with $i_1, \cdots, i_n \geq 1$.

On the other hand, $\deg p \leq n$, so
$p = (z-1)\cdots(z-n)$.

$\square$

### 5B.13

Suppose $𝑇 ∈ ℒ(𝑉)$ and $𝑝 ∈ 𝒫(𝐅)$.
Prove that there exists a unique $𝑟 ∈ 𝒫(𝐅)$
such that $𝑝(𝑇) = 𝑟(𝑇)$ and $\deg 𝑟$ is less than the degree of 
the minimal polynomial of $𝑇$.

**Proof**:

Let $q$ be the minimal polynomial of $T$, from the division
algorithm of polynomials, we know we can find unique
$s(z), r(z)$ such that

$$ 
p(z) = s(z)q(z) + r(z)
$$

and $\deg r < \deg q$, then

$$
\begin{align*}
p(T) &= s(T)q(T) + r(T) \\
&= s(T) 0 + r(T) \\
&= r(T)
\end{align*} 
$$

For the uniqueness, if $r'(T) = P(T) = r(T)$, and
$\deg r' < \deg q$, then $(r-r')(T) = 0$.
Furthermore, $\deg (r-r') < \deg q$, since $q$ is the minimal
polynomial of $T$, then $r-r'$ has to be $0$.

$\square$

### 5B.14

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$ has minimal polynomial
$4 + 5𝑧 − 6𝑧^2 − 7𝑧^3 + 2𝑧^4 + 𝑧^5$ . Find the minimal polynomial of $𝑇^{−1}$.

**Solution**:

First note that

$$ 
\begin{align*}
4I + 5T − 6T^2 − 7T^3 + 2T^4 + T^5 &= 0 \\
& \Rightarrow \\
-(5 − 6T − 7T^2 + 2T^3 + T^4)T &= 4I \\
& \Rightarrow \\
T &\text{ is invertible}
\end{align*} 
$$

Then we have

$$ 
\begin{align*}
4I + 5T − 6T^2 − 7T^3 + 2T^4 + T^5 &= 0 \\
& \Rightarrow \\
T^{5} (4T^{-5} + 5 T^{-4} - 6T^{-3} - 7 T^{-2} + 2T^{-1} + I)
&= 0\\
\end{align*}
$$

Since $T$ is invertible, so is $T^{5}$.
Then we have

$4T^{-5} + 5 T^{-4} - 6T^{-3} - 7 T^{-2} + 2T^{-1} + I = 0$.

If we can find a polynomial with degree less than $5$ that can
nullify $T^{-1}$, then we can use similar approach to find
a polynomial with degree less than $5$ to nullify $T$ which
contradicts the fact that minimal polynomial of $T$ has
degree $5$.

$\square$

### 5B.15

Suppose $𝑉$ is a finite-dimensional complex vector space with
$\dim 𝑉 > 0$ and $𝑇 ∈ ℒ(𝑉)$. Define $𝑓 ∶ 𝐂 → 𝐑$ by

$$ 
𝑓 (\lambda) = \text{dim range } (𝑇 − \lambda𝐼).
$$

Prove that $𝑓$ is not a continuous function.

**Proof**:

Let $\dim V = n$. Since
$𝑉$ is a finite-dimensional complex vector space, then from
"5.19 existence of eigenvalues", we know
$T$ has an eigenvalue, say $\lambda$.

From "5.12 operator cannot have more eigenvalues than dimension of vector space", we know
$T$ can have at most $n$ distinct eigenvalues, so
we can find a neighborhood of $\lambda$, $V_{\delta }(\lambda)$,
such that if $c \in V_{\delta }(\lambda)$ and
$c \neq \lambda$, then $c$ is not an eigenvalue.

For these $c$, $T - cI$ is invertible, so
$\text{dim range } T-cI = n$.
On the other hand, $\text{dim range } T-\lambda I < n$ since
$\text{dim range } T-\lambda I = n - \text{dim null } T-\lambda I$,
and $\text{dim null } T-\lambda I > 0$.

So $𝑓 (\lambda)$ is not continuous at $\lambda$.

$\square$

### 5B.16

Suppose $𝑎_0, …, 𝑎_{𝑛 − 1} ∈ 𝐅$. Let
$𝑇$ be the operator on $𝐅^𝑛$ whose matrix (with
respect to the standard basis) is

$$ 
\begin{pmatrix}
0 &   &        &  & &  & -a_0 \\ 
1 & 0 &        &  & &  & -a_1 \\ 
  & 1 & \ddots &  & &  & -a_2 \\ 
  &   & \ddots &  & &  & \vdots \\
  &   &        &  & & 0 & -a_{n-2} \\
  &   &        &  & & 1 & -a_{n-1} \\
\end{pmatrix}
$$

Here all entries of the matrix are $0$ except for all $1’s$
on the line under the
diagonal and the entries in the last column (some of which might 
also be $0$).
Show that the minimal polynomial of $𝑇$ is the polynomial.

$$ 
𝑎_0 + 𝑎_1𝑧 +⋯ + 𝑎_{𝑛 − 1}𝑧^{𝑛 − 1} + 𝑧^𝑛
$$

**Proof**:

Let $p(z) = 𝑎_0 + 𝑎_1𝑧 +⋯ + 𝑎_{𝑛 − 1}𝑧^{𝑛 − 1} + 𝑧^𝑛$ 

Consider $e_1 = (1, 0, \cdots, 0)$. And note

$$
\begin{align*}
T(e_1) &= e_2 \\ 
T^2(e_1) &= T(e_2) = e_3 \\
& \cdots \\
T^{n-1}(e_1) &= e_n \\
T^n(e_1) &= T(e_n) = -(a_0, a_1, a_2, \cdots, a_{n-1})
\end{align*} 
$$

So

$$ 
𝑎_0(e_1) + 𝑎_1T(e_1) +⋯ + 𝑎_{𝑛 − 1}T^{𝑛 − 1}(e_1) + T^𝑛(e_1) = 0
$$

i.e. $p(T)(e_1) = 0$.

Furthermore, notice for $1 \leq i \leq n-1$ 

$$ 
\begin{align*}
0 &= T^i(0) \\
&=T^i (𝑎_0(e_1) + 𝑎_1T(e_1) +⋯ + 𝑎_{𝑛 − 1}T^{𝑛 − 1}(e_1) + T^𝑛(e_1)) \\
&= 𝑎_0(T^i(e_1)) + 𝑎_1T(T^i(e_1)) +⋯ + 𝑎_{𝑛 − 1}T^{𝑛 − 1}(T^i(e_1)) + T^𝑛(T^i(e_1)) \\
&= 𝑎_0(e_{i+1}) + 𝑎_1T(e_{i+1}) +⋯ + 𝑎_{𝑛 − 1}T^{𝑛 − 1}(e_{i+1}) + T^𝑛(e_{i+1})
\end{align*} 
$$

i.e. $p(T)(e_{i+1}) = 0$. This means $p(T) = 0$.

Also, since $T^{i}(e_1) = e_{i+1}$, so
$e_1, T(e_1), \cdots, T^{n-1}(e_1)$ are independent, then
it's not possible to find a polynomial $q$ with $\deg q < n$,
such that $q(T) = 0$. Otherwise $q(T)(e_1) = 0$, which is not
possible.

So the minimal polynomial of $T$ is $p$.

$\square$

### 5B.17

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉)$, and $𝑝$ is the 
minimal polynomial of $𝑇$. Suppose $𝜆 ∈ 𝐅$. Show that the minimal 
polynomial of $𝑇 − 𝜆𝐼$ is the
polynomial $𝑞$ defined by $𝑞(𝑧) = 𝑝(𝑧 + 𝜆)$.

**Proof**:

First

$$ 
\begin{align*}
q(T - \lambda I) &=
p(T - \lambda I + \lambda I) \\
&= p(T) \\
&= 0
\end{align*} 
$$

Now assume there is another monic polynomial $q'$ with
$\deg q' < \deg q = \deg p$ and
$q'(T-\lambda I) = 0$

Then let $p'(z) = q'(z-\lambda)$, then $p'$ is also
a monic polynomial such that
$\deg p' = \deg q' < \deg q = \deg p$.

Also $p'(T) = q'(T - \lambda I) = 0$.

This is contradictary to the fact that $p$ is the minimal
polynomial.

So $q$ is the minimal polynomial of $T-\lambda I$.

$\square$

### 5B.18

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉)$, and $𝑝$ is the 
minimal polynomial
of $𝑇$. Suppose $\lambda ∈ 𝐅 \backslash \{0\}$.
Show that the minimal polynomial of $𝜆𝑇$ is the
polynomial $𝑞$ defined by
$𝑞(𝑧) = \lambda ^{\deg 𝑝} 𝑝( 𝑧 / \lambda  )$.

**Proof**:

let $m = \deg 𝑝$, and

$$ 
p(z) = a_0 + a_1 z + \cdots + z^{m}
$$

Then

$$
\begin{align*}
q(\lambda T) &=
\lambda ^{m} p(\frac{\lambda T}{\lambda}) \\
&= \lambda ^{m} p(T) \\
&= 0 \\
\end{align*} 
$$

Also

$$
\begin{align*}
q(z) &= \lambda ^m p( z / \lambda  ) \\
&= \lambda ^m a_0 + \lambda ^{m-1} a_1 z + \cdots +
z^m
\end{align*} 
$$

So $q$ is monic.

Now assume $q'(z) = b_0 + b_1 z + \cdots + z^{k}$ satisfy
$k < m$ and $q'(\lambda T) = 0$.

Then

$$ 
\begin{align*}
0 &= q'(\lambda T) \\
&= b_0 + b_1 (\lambda T) + \cdots + (\lambda T)^{k} \\
&= (\lambda)^k (b_0 \lambda^{-k} + b_1 \lambda^{1-k}T
+ \cdots  + T^k)
\end{align*} 
$$

Since $\lambda \neq 0$, so $\lambda^k \neq 0$, then
$b_0 \lambda^{-k} + b_1 \lambda^{1-k}T + \cdots  + T^k = 0$,

Let $p'(z) = b_0 \lambda^{-k} + b_1 \lambda^{1-k}z + \cdots + z^k$.

So we found a monic polynomial
$p'$ with $p'(T) = 0$ and $\deg p' < \deg p$.

This is contradictary to the fact that $p$ is the minimal
polynomial.

So
the minimal polynomial of $𝜆𝑇$ is the
polynomial $𝑞$ defined by
$𝑞(𝑧) = \lambda ^{\deg 𝑝} 𝑝( 𝑧 / \lambda  )$.

$\square$

### 5B.19

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$.
Let $ℰ$ be the subspace of $ℒ(𝑉)$ defined by

$$ 
ℰ = \{q(T): q \in 𝒫(𝐅)\}
$$

Prove that $\dim ℰ$ equals the degree of the minimal polynomial of $𝑇$.

**Proof**:

Let $p(z)$ be the minimal polynomial of $𝑇$.
And $\deg p = m$.
Given any $q(z)$, using
the "4.9 division algorithm for polynomials", we know we can find
$s, r$ such that

$$ 
q(z) = s(z) p(z) + r(z)
$$

with $\deg r < \deg p$.

The use "5.17 multiplicative properties", we know

$$ 
q(T) = s(T) p(T) + r(T)
$$

So

$$
\begin{align*}
q(T)(v) &= (s(T) p(T) + r(T))(v) \\
&= s(T) p(T)(v) + r(T)(v) \\
&= r(T) (v)
\end{align*} 
$$

So $q(T) = r(T)$.

Since $\deg r < \deg p$, then $r(z)$ can be represented by
$1, z, z^2, \cdots, z^{m-1}$.

So $q(T) = r(T) \in \text{span}(I, T, T^2, \cdots, T^{m-1})$.
so $ℰ \subseteq \text{span}(I, T, T^2, \cdots, T^{m-1})$.
So $\dim ℰ \leq m$ 

On the other hand, $I, T, T^2, \cdots, T^{m-1}$ are linear independent.
Otherwise, we can find $a_i$ such that they are not all 0 and

$$ 
a_0 I + a_1 T + \cdots + a_{m-1} T^{m-1} = 0
$$

That means we find another polynomial with degree less than $m$ such that
it's 0, which contradicts the assumption that $p(z)$ is the minimal
polynomial.

Since $I, T, T^2, \cdots, T^{m-1}$ are linear independent,
then $\dim ℰ \geq m$.

In summary, $\dim ℰ = m$.

$\square$

### 5B.20

Suppose $𝑇 ∈ ℒ(𝐅^4)$ is such that the eigenvalues of 𝑇 are 3, 5, 8. Prove 
that
$(𝑇 − 3𝐼)^2(𝑇 − 5𝐼)^2(𝑇 − 8𝐼)^2 = 0$.

**Proof**:

Let $p(z)$ be the minimal polynomial of $T$. From
"5.22 existence, uniqueness, and degree of minimal polynomial",
$\deg p \leq \dim F^4 = 4$.

From "5.27 eigenvalues are the zeros of the minimal polynomial"
we know $p(3) = p(5) = p(8) = 0$.

From "4.6 each zero of a polynomial corresponds to a degree-one factor"
we know $p(z) = (z-3)(z-5)(z-8)q(z)$.

Since $\deg p \leq 4$, $\deg q = 1$ or $\deg q = 0$.

Case 1: $\deg q = 0$, then $p(z) = (z-3)(z-5)(z-8)$. Then
$(z-3)^2(z-5)^2(z-8)^2$ is a multiple of $p(z)$.

Case 2: $\deg q = 1$, then $q(z) = z- \lambda$ and
$p(z) = (z-\lambda)(z-3)(z-5)(z-8)$.

Use 5.27 again, we know $\lambda$ is an eigenvalue of $T$, so
$\lambda = 3, 5, 8$. In any case,
$(z-3)^2(z-5)^2(z-8)^2$ is a multiple of $p(z)$.

Then we can use 5.29 to conclude $(𝑇 − 3𝐼)^2(𝑇 − 5𝐼)^2(𝑇 − 8𝐼)^2 = 0$.

$\square$

### 5B.21

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$. Prove that the minimal
polynomial of $𝑇$ has degree at most $1 + \text{dim range } 𝑇$.

If $\text{dim range } T < \dim 𝑉 − 1$, then this exercise gives a better upper bound
than 5.22 for the degree of the minimal polynomial of $𝑇$.

**Proof**:

Let $m = \text{dim range } T$.
Let $U = \text{range } T$, then consider $T|_U$.
Since $U$ is invariant under $T$, so $T|_U$ is well defined.

Let $p(z)$ be the minimal polynomial of $T|_U$, then from 5.22, $\deg p \leq m$.
Consider $q(z) = p(z)z$. We would like to show $q(T) = p(T)T = 0$.

Given $v \in V$,

case 1: $v \in \text{null } T$, then $p(T)T(v) = p(T)(T(v)) = p(T)(0) = 0$.

case 2: $v \not\in \text{null } T$, then $T(v) = u \in \text{range } T$,
so $p(T|_U)(u) = 0$. Also, since $u \in \text{range } T$, then
$p(T)(u) = p(T|_U)(u)$, so $0 = p(T|_U)(u) = p(T)(u) = p(T)(T(u)) = (p(T)T)(u)$.

So in summary, $p(T)T = 0$.

Then from 5.29, $p(T)T$ is a multiple of minimal polynomial.
Then the minimal
polynomial of $𝑇$ has degree at most $1 + \text{dim range } 𝑇$.

$\square$

### 5B.22

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$.
Prove that $𝑇$ is invertible if and only if
$𝐼 ∈ \text{span}(𝑇, 𝑇^2 , …, 𝑇^{\dim 𝑉})$.

**Proof**:

Let $m = \dim V$

$\Leftarrow$

$$
\begin{align*}
I &= a_1 T + \cdots + a_m T^m \\
&= T(a_1 I + \cdots + a_m T^{m-1}) \\
&= (a_1 I + \cdots + a_m T^{m-1})T \\
\end{align*}  
$$

So $T$ has an inverse mapping: $a_1 I + \cdots + a_m T^{m-1}$.

$\Rightarrow$

From
5.32 $𝑇$ not invertible ⟺ constant term of minimal polynomial of $𝑇$ is 0
we know if $p(z)$ is the minimal polynomial, then

$$ 
p(z) = a_0 + a_1 z + \cdots + a_{k} z^{k}
$$

where $a_0 \neq 0, k \leq m$, so

$$ 
I = -\frac{a_1}{a_0} T - \cdots -\frac{a_k}{a_0} T^{k}
\in \text{span}(𝑇, 𝑇^2 , …, 𝑇^{\dim 𝑉})
$$

$\square$

### 5B.23

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$. Let $𝑛 = \dim 𝑉$.
Prove that if $𝑣 ∈ 𝑉$, then
$\text{span}(𝑣, 𝑇𝑣, …, 𝑇^{𝑛 − 1}𝑣)$ is invariant under $𝑇$.

**Proof**:

Let $U = \text{span}(𝑣, 𝑇𝑣, …, 𝑇^{𝑛 − 1}𝑣)$.

We only need to prove $T^nv \in U$.

Since $𝑣, 𝑇𝑣, …, 𝑇^{𝑛 − 1}𝑣, T^n v$ are linear dependent, we can find

$$ 
a_0 v + a_1 Tv + \cdots + a_{n-1} T^{n-1}v + a_n T^n v = 0
$$

and $a_0, \cdots a_n$ are not all $0$.

Let $m$ be the biggest integer such that $a_m \neq 0$. So we have

$$ 
a_0 v + a_1 Tv + \cdots + a_{m-1} T^{m-1} v + a_m T^m v = 0 \\
\Rightarrow \\
T^m v = -\frac{a_0}{a_m} v -\frac{a_1}{a_m} Tv \cdots -\frac{a_{m-1}}{a_m} T^{m-1} v
$$

Apply $T^{n-m}$ on both sides we have

$$ 
T^{n-m}(T^m v) = T^{n-m}(-\frac{a_0}{a_m} v -\frac{a_1}{a_m} Tv - \cdots -\frac{a_{m-1}}{a_m} T^{m-1} v) \\
\Rightarrow \\
T^n v = -\frac{a_0}{a_m} T^{n-m}v -\frac{a_1}{a_m} T^{n-m+1}v - \cdots -\frac{a_{m-1}}{a_m} T^{n-1} v
$$

$\square$

### 5B.24

Suppose $𝑉$ is a finite-dimensional complex vector space. Suppose $𝑇 ∈ ℒ(𝑉)$
is such that $5$ and $6$ are eigenvalues of $𝑇$ and that $𝑇$ has no other eigenvalues.
Prove that $(𝑇 − 5𝐼)^{\dim 𝑉 − 1}(𝑇 − 6𝐼)^{\dim 𝑉 − 1} = 0$.

**Proof**:

Let $p(z)$ be the minimal polynomial of $T$. From
5.27 eigenvalues are the zeros of the minimal polynomial (b)

$$ 
p(z) = (z-\lambda_1) \cdots (z-\lambda_m)
$$

where $\lambda_1, …, \lambda_𝑚$ is a list of all eigenvalues of $𝑇$, 
possibly with repetitions.

So $\lambda_i = 5, 6$. So $p(z) = (z-5)^s(z-6)^t, s,t \geq 1$.

If $s > \dim V - 1$, then $\deg p > \dim V$ which is not possible,
so $s \leq \dim V - 1$.
Similarly $t \leq \dim V - 1$.

Then $(𝑇 − 5𝐼)^{\dim 𝑉 − 1}(𝑇 − 6𝐼)^{\dim 𝑉 − 1}$ is a multiple of $p$.
So $(𝑇 − 5𝐼)^{\dim 𝑉 − 1}(𝑇 − 6𝐼)^{\dim 𝑉 − 1} = 0$.

$\square$

### 5B.25

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉)$, and $𝑈$ is a subspace of 
$𝑉$ that is invariant under $𝑇$.

(a) Prove that the minimal polynomial of $𝑇$ is a polynomial multiple of the
minimal polynomial of the quotient operator $𝑇/𝑈$.

**Proof**:

Assume the minimal polynomial of $𝑇$ is $p(z)$, given any $v \in V$, we
need to prove $p(T/U)(v+U) = 0$.

Since $T/U(v+U) = T(v) + U$, then

$$
\begin{align*}
p(T/U)(v+U) &= p(T)(v) + U \\
&= 0 + U
\end{align*} 
$$

Then $p(T/U)$ is a zero operator on $V/U$.

Then from 5.29 $𝑞(𝑇) = 0 ⟺ 𝑞$ is a polynomial multiple of the minimal 
polynomial, we can conclude $p$ is a polynomial multiple of the
minimal polynomial of the quotient operator $𝑇/𝑈$.

$\square$

(b) Prove that

(minimal polynomial of $𝑇|_𝑈$) × (minimal polynomial of $𝑇/𝑈$)

is a polynomial multiple of the minimal polynomial of 𝑇.

**Proof**:

Assume minimal polynomial of $𝑇|_𝑈$ is $p(z)$ and
minimal polynomial of $𝑇/𝑈$ is $q(z)$.

We need to prove, given any $v \in V$, $p(T)q(T)(v) = 0$.

First since the minimal polynomial of $𝑇/𝑈$ is $q(z)$. Then
$q(T/U)(v+U) = 0 + U$. On the other hand, $q(T/U)(v+U) = q(T)(v) + U$.
Thus it means $q(T)(v) \in U$.

Since the minimal polynomial of $𝑇|_𝑈$ is $p(z)$, then
$p(𝑇|_𝑈)(q(T)(v)) = 0$.

Since $U$ is invariant under $T$, then from exercise 5A.41 we know $U$
is also invariant under $p(T)$. Thus for any $u \in U$, $p(T|_U)(u) = p(T)(u)$.
So $p(T)(q(T)(v)) = p(𝑇|_𝑈)(q(T)(v)) = 0$.

Then again from 5.29 $𝑞(𝑇) = 0 ⟺ 𝑞$ is a polynomial multiple of the minimal 
polynomial, we can conclude the statement.

$\square$

### 5B.26

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉)$, and $𝑈$ is a subspace of
$𝑉$ that is invariant under $𝑇$.
Prove that the set of eigenvalues of $𝑇$ equals the union
of the set of eigenvalues of $𝑇|𝑈$ and the set of eigenvalues of $𝑇/𝑈$.

**Proof**:

Let the minimal polynomial of $T$ be $s(z)$,
minimal polynomial of $𝑇|_𝑈$ is $p(z)$ and
minimal polynomial of $𝑇/𝑈$ is $q(z)$.

$\Rightarrow$

Assume $\lambda$ is a eigenvalue of $T$.
Then $\lambda$ is a zero of $s(z)$.
From the part (b) of exercise 5B.25, $p(z)q(z)$ is a multiple of $s(z)$,
then $p(\lambda)q(\lambda) = 0$, so $p(\lambda) = 0$ or $q(\lambda) = 0$.

Then from 5.27, $\lambda$ is either
an eigenvalue of $𝑇|𝑈$ or an eigenvalue of $𝑇/𝑈$.

$\Leftarrow$

From exercise 5A.38, we know an eigenvalue of $T/U$ is an eigenvalue of
$T$.

Assume $\lambda$ is an eigenvalue of $T|_U$, then we can find a $u \neq 0$
and $u \in U$ such that $T|_U(u) = \lambda u$.
Since $u \in U$, then $T(u) = T|_U(u) = \lambda u$.

So $\lambda$ is an eigenvalue of $T$.

$\square$

### 5B.27

Suppose $𝐅 = 𝐑$, $𝑉$ is finite-dimensional, and $𝑇 ∈ ℒ(𝑉)$.
Prove that the
minimal polynomial of $𝑇_𝐂$ equals the minimal polynomial of $𝑇$.
The complexification $𝑇_𝐂$ was defined in Exercise 33 of Section 3B.

**Proof**:

Let $p$ be the minimal polynomial of $T$ and $p'$ be
the minimal polynomial of $T_C$.

Note that $T_C(u+iv) = T(u) + iT(v)$, so

$$ 
\begin{align*}
T_C^n(u+iv) &=
T_C^{n-1}(T_C(u+iv)) \\
&= T_C^{n-1}(T(u) + iT(v)) \\
&= T_C^{n-2}(T_C(T(u) + iT(v))) \\
&= T_C^{n-2}(T^2(u) + iT^2(v)) \\
&\cdots \\
&= T^n(u) + iT^n(v) \\
\end{align*} 
$$

Then from the linearity of $T_C$, we can see

$$
\begin{align*}
q(T_C)(u+iv) &=
q(T)(u) + iq(T)(v)
\end{align*} 
$$

So given any $u+iv$ 

$$
\begin{align*}
0 &= p'(T_C)(u+iv) \\
&= p'(T)(u) + ip'(T)(v) \\
& \Rightarrow \\
p'(T)(u) = 0,&\qquad p'(T)(v) = 0
\end{align*} 
$$

So $p'$ is a multiple of $p$.

On the other hand

$$ 
\begin{align*}
0 &= p(T)(u) + ip(T)(v) \\
&=p(T_C)(u+iv) \\
\end{align*} 
$$

So $p$ is a multiple of $p'$.

Then $p = p'$

$\square$

### 5B.28

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$. Prove that the minimal
polynomial of $𝑇' ∈ ℒ(𝑉')$ equals the minimal polynomial of $𝑇$.

**Proof**:

One way to think this problem is consider the matrix of $T$ and $T'$.
They are transpose to each other.

But we will do another way. Note that given any linear functional
$\varphi_i \in V'$, we have

$$
\begin{align*}
(T')^n(\varphi_i)
&= (T')^{n-1} (T'(\varphi_i)) \\
&= (T')^{n-1} (\varphi_i \circ T) \\
&= (T')^{n-2} (T'(\varphi_i \circ T)) \\
&= (T')^{n-2} ((\varphi_i \circ T) \circ T) \\
&= (T')^{n-2} (\varphi_i \circ (T^2)) \\
&= \cdots \\
&= \varphi_i \circ T^n
\end{align*}  
$$ 

And then use the distribution law of the composition of the linear mapping,
we have $p(T')(\varphi_i) = \varphi_i \circ p(T)$ 

First assume $p(z)$ is the minimal polynomial of $𝑇$.
And assume $p'(z)$ is the minimal polynomial of $𝑇'$.

Then given any linear functional $\varphi$ and $v \in V$,

$$
\begin{align*}
(p(T')(\varphi))(v)
&= (\varphi \circ p(T))(v) \\
&= \varphi (p(T)(v)) \\
&= \varphi (0) \\
&= 0
\end{align*} 
$$ 

So $p$ is a multiple of $p'$.

Now assume $v_1, \cdots, v_m$ is a basis of $v$ and
$\varphi_1, \cdots, \varphi_m$ is the dual basis.
And assume
$$ 
p'(T)(v) = a_1 v_1 + \cdots + a_m v_m
$$

On one hand

$\varphi_i(a_1 v_1 + \cdots + a_m v_m) = a_1 \varphi_i(v_1) + \cdots + a_m \varphi_i(v_m) = a_i$

On the other hand

$$ 
\begin{align*}
\varphi_i((p'(T)) (v))
&= (\varphi_i \circ p'(T)) (v)\\
&= (p'(T')(\varphi_i))(v) \\
&= 0(v) \\
&= 0
\end{align*} 
$$

So $a_i = 0$, i.e. $p'(T)(v) = 0$.

So $p'$ is a multiple of $p$.

Based on this, $p = p'$.

$\square$

### 5B.29

Show that every operator on a finite-dimensional vector space of dimension
at least two has an invariant subspace of dimension two.

**Proof**:

Consider $T$ is the operator, and $p(z)$ is its minimal polynomial.

We distinguish the following cases:

case $1$: If $p(z) = z-\lambda$, then every vector is a eigenvector of 
$\lambda$. Since $\dim V \geq 2$, then we can pick two linear independent
vectors $u_1, u_2$. 
Then
$\text{span}(u_1, u_2)$ is invariant with dimension $2$.

case $2$: $\deg p(z) \geq 2$, 
we can assume $p(z) = (z^2+bz+c)q(z)$.
This is because if $\mathbb{F} = \mathbb{R}$, we can use
"4.16 factorization of a polynomial over $\mathbb{R}$".
If $\mathbb{F} = \mathbb{C}$, we can use
"4.13 fundamental theorem of algebra, second version".

Consider
$\text{range } q(T)$. It cannot be $\{0\}$ because otherwise $q(z)$ will
be the minimal polynomial.

Then assume we can find $u \in \text{range } q(T)$,
such that $u$ is not an eigenvector of
$T$, then $u, T(u)$ are linearly independent.
Furthermore, since $(T^2+bT+c)(u) = 0$, we have $T^2u = -bTu - cu$.
So $\text{span}(u, Tu)$ is invariant with dimension $2$.

Now assume all $u \in \text{range } q(T)$ are eigenvectors.
If for
all $u \in \text{range } q(T)$, $T(u) = \lambda u$, then
$(z- \lambda)q(z)$ will be the minimal polynomial, which is
contradictary to our assumption that $p(z)$ is the minimal polynomial.

So we can find $\lambda_1, \lambda_2$ which are 2 different eigenvalues
and we can find
2 eigenvectors $u_1, u_2$, such that
$T(u_1) = \lambda_1 u_1, T(u_2) = \lambda_2 u_2$.

From 5.11 linearly independent eigenvectors, we know $u_1, u_2$ are linear independent, then
$\text{span}(u_1, u_2)$ is invariant with dimension $2$.

$\square$

## Section 5C Upper-Triangular Matrices

### 5C.1

Prove or give a counterexample: If $𝑇 ∈ ℒ(𝑉)$ and $𝑇^2$ has an 
upper-triangular matrix with respect to some basis of $𝑉$,
then $𝑇$ has an upper-triangular matrix
with respect to some basis of $𝑉$.

**Solution**:

Consider $V = \mathbb{R}^2$. And $T$ be the linear operator that rotates
$V$ by $90$ degree counterclockwise.

Since $T$ does not have an eigenvalue, then $T$ does not have a 
1-dimensional subspace
that is invariant under $T$ w.r.t any basis of $V$.
Therefore, it's not possible that
$𝑇$ has an upper-triangular matrix w.r.t any basis of $V$.

On the other hand, the matrix of $T^2$ w.r.t the standard basis
is 

$$ 
\begin{bmatrix}
-1 & 0 \\
0 & -1 \\
\end{bmatrix}
$$

which is an upper-triangular matrix.

$\square$

### 5C.2

Suppose $𝐴$ and $𝐵$ are upper-triangular matrices of the same size, with
$𝛼_1, …, 𝛼_𝑛$ on the diagonal of $𝐴$ and $𝛽_1, …, 𝛽_𝑛$ on the 
diagonal of $𝐵$.

(a) Show that $𝐴 + 𝐵$ is an upper-triangular matrix with 
$𝛼_1 + 𝛽_1, …, 𝛼_𝑛 + 𝛽_𝑛$
on the diagonal.

**Proof**:

Let $C = A + B$, then the diagonal of $C$ on the $i$th row and $i$th
column is

$$
\begin{align*}
C_{i,i} &= A_{i,i} + B_{i,i} \\
&= 𝛼_i + 𝛽_i \
\end{align*}  
$$

$\square$

(b) Show that $𝐴𝐵$ is an upper-triangular matrix with
$𝛼_1 𝛽_1, …, 𝛼_𝑛 𝛽_𝑛$ on the diagonal.

**Proof**

Let $C = AB$, then the diagonal of $C$ on the $i$th row and $i$th
column is

$$ 
\begin{align*}
C_{i,i} &= \sum_{k = 1}^{n} a_{i, k} b_{k, i} \\
\end{align*} 
$$

Note that if $i > k, a_{i, k} = 0$, and if $i < k, b_{k, i} = 0$,
so $C_{i,i} = a_{i,i} b_{i,i} = 𝛼_i 𝛽_i$.

$\square$

### 5C.3

Suppose $𝑇 ∈ ℒ(𝑉)$ is invertible and $𝑣_1, …, 𝑣_𝑛$ is a basis of $𝑉$ 
with respect
to which the matrix of $𝑇$ is upper triangular, with $𝜆_1, …, 𝜆_𝑛$ on 
the diagonal.
Show that the matrix of $𝑇^{−1}$ is also upper triangular with respect to 
the basis $𝑣_1, …, 𝑣_𝑛$, with

$$ 
\frac{1}{𝜆_1} , …, \frac{1}{𝜆_𝑛} 
$$

on the diagonal.

**Proof**:

First, from "5.41 determination of eigenvalues from upper-triangular matrix",
$𝜆_1, …, 𝜆_𝑛$ are the eigenvalues of $T$. Since $T$ is invertible,
then $0$ is not an eigenvalue of $T$. So $𝜆_1, …, 𝜆_𝑛 \neq 0$.

Then $\frac{1}{𝜆_1} , …, \frac{1}{𝜆_𝑛}$ is well defined.

Next, we show if $U$ is invariant under $T$ and $T$ is invertible, then
$U$ is invariant under $T^{-1}$.

Let $u \in U$, and consider $T|_U$. Since $T$ is invertible,
then $T$ is injective, then $T|_U$ is also injective.
So $T|_U$ is invertible. Then we can find $w \in U$ such that
$T|_U(w) = u$. then we have $T(w) = u$.

So $T^{-1}(u) = T^{-1}(T(w)) = w \in U$.
Then $U$ is invariant under $T^{-1}$.

Now let $U_i = \text{span}(𝑣_1, \cdots, 𝑣_i)$.
From "5.39 conditions for upper-triangular matrix", $U_i$ is invariant under $T$,
then $U_i$ is also invariant under $T^{-1}$, then again use 5.39,
The matrix of $𝑇^{-1}$ with respect to $𝑣_1, …, 𝑣_𝑛$ is upper triangular.

Let $\eta_i$ on the diagonal. Note
$v_1 = T^{-1} (T v_1) = T^{-1} (\lambda_1 v_1) = \eta_1 \lambda_1 v_1$,
so $\eta_1 \lambda_1 = 1$, thne $\eta_1 = \frac{1}{\lambda_1}$.

For $i \geq 2$,

$$ 
T(v_i) = \lambda_i v_i + u_{i-1}
$$

Where $u_{i-1} \in U_{i-1}$, then

$$
\begin{align*}
v_i &= T^{-1} (T v_i) \\
&= T^{-1} (\lambda_i v_i) + T^{-1} (u_{i-1}) \\
&= \eta_i \lambda_i v_i + T^{-1} (u_{i-1}) \\
& \Rightarrow \\
0 = (1 - \eta_i \lambda_i) v_i + T^{-1} (u_{i-1}) \\
\end{align*} 
$$

Since $U_i$ is invariant under $T^{-1}$, then
$T^{-1} (u_{i-1}) \in U_{i-1} = \text{span}(𝑣_1, \cdots, 𝑣_{i-1})$.
Then we must have $1 - \eta_i \lambda_i = 0$, i.e.
$\eta_i = \frac{1}{\lambda_i}$.

$\square$

### 5C.4

Give an example of an operator whose matrix with respect to some basis
contains only $0$'s on the diagonal, but the operator is invertible.
This exercise and the exercise below show that 5.41 fails without the
hypothesis that an upper-triangular matrix is under consideration.

**Proof**:

Consider the vector space is $\mathbb{R}^2$, and the operator $T$ is
rotation counterclockwise by 90 degree.
And the basis is the standard basis, $e_1, e_2$.

$T(e_1) = e_2, T(e_2) = -e_1$. So

$$ 
\mathcal{M}(T) =
\begin{bmatrix}
0 & -1 \\
1 & 0 \\
\end{bmatrix}
$$

It's invertible because its inverse is rotation clockwise by 90 degree.

$\square$

### 5C.5

Give an example of an operator whose matrix with respect to some basis
contains only nonzero numbers on the diagonal, but the operator is not
invertible.

**Proof**:

Consider the vector space is $\mathbb{R}^2$, and the operator $T$ is
defined as

$$ 
T(e_1) = (1, 1) \\
T(e_2) = (1, 1) \\
$$

Since it's not injective, it's not invertible.

Also the 

$$ 
\mathcal{M}(T) =
\begin{bmatrix}
1 & 1 \\
1 & 1 \\
\end{bmatrix}
$$

$\square$

### 5C.6

Suppose $𝐅 = 𝐂$, $𝑉$ is finite-dimensional, and $𝑇 ∈ ℒ(𝑉)$. Prove that if
$𝑘 ∈ \{1, …, \dim 𝑉\}$, then $𝑉$ has a $𝑘$-dimensional subspace invariant under 
$𝑇$.

**Proof**:

Use "5.47 if 𝐅 = 𝐂, then every operator on 𝑉 has an upper-triangular matrix",
then for the operator $T$, we can find a basis $v_1, \cdots, v_n$, such that
$\mathcal{M}(T)$ is upper-triangular.

Then use "5.39 conditions for upper-triangular matrix", we know
$\text{span}(𝑣_1, \cdots, 𝑣_k)$ is invariant under $T$ and its dimension is $k$.

$\square$

### 5C.7

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉)$, and $𝑣 ∈ 𝑉$.

(a) Prove that there exists a unique monic polynomial $𝑝_𝑣$ of smallest degree
such that $𝑝_𝑣(𝑇)𝑣 = 0$.

**Proof**:

Let $n = \dim V$ and then the following $1+n$ vectors must be linear dependent

$$ 
v, Tv, \cdots, T^{n}v
$$

Then we can find the smallest $k$, such that $T^{k} v$ is the linear combination of
$v, \cdots, T^{k-1}v$ and then we find the $𝑝_𝑣$.

(b) Prove that the minimal polynomial of $𝑇$ is a polynomial multiple of $𝑝_𝑣$.

**Proof**:

Let $p$ be the minimal polynomial of $𝑇$.

Let $U = \text{span}(v, Tv, \cdots, T^{k-1}v)$. Then $U$ is invariant under $T$.
Then we can consider $T|_U$. Note that $p_v$ is the minimal polynomial of $T|_U$
from part (a).

Then from "5.21 minimal polynomial of a restriction operator", we know
$p$ is multiple of $𝑝_𝑣$.

$\square$

### 5C.8

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉)$, and there exists a nonzero
vector $𝑣 ∈ 𝑉$ such that $𝑇^2𝑣 + 2𝑇𝑣 = −2𝑣$.

(a) Prove that if $𝐅 = 𝐑$, then there does not exist a basis of $𝑉$ with respect
to which $𝑇$ has an upper-triangular matrix.

**Proof**:

Let $p$ the minimal polynomial of $T$ and $p_v(z) = z^2 + 2z + 2$.
Note that $p_v(z)$ does not have a real zero, which means $v$ is not an eigenvector.

Otherwise, if $T(v) = \lambda v$, then 
$0 = 𝑇^2𝑣 + 2𝑇𝑣 + 2𝑣 = \lambda^2𝑣 + 2\lambda𝑣 + 2𝑣 = (\lambda^2 + 2\lambda + 2)𝑣$, so $\lambda^2 + 2\lambda + 2 = 0$. No real $\lambda$ can satisfy this equation.

Then $p_v(z)$ satisfy the 5C.7(a), so $p$ is a multiple of $p_v$.
Since $p_v$ cannot be written in the form of $(z-a)(z-b), a,b \in \mathbb{R}$.

Then use "5.44 necessary and sufficient condition to have an upper-triangular matrix",
we know
there does not exist a basis of $𝑉$ with respect
to which $𝑇$ has an upper-triangular matrix.

$\square$

(b) Prove that if $𝐅 = 𝐂$ and $𝐴$ is an upper-triangular matrix that equals
the matrix of $𝑇$ with respect to some basis of $𝑉$ , then $−1 + 𝑖$ or $−1 − 𝑖$
appears on the diagonal of $𝐴$.

**Proof**:

Let $\lambda_1 = −1 + 𝑖$ and $\lambda_2 = −1 - 𝑖$, then it's possible that

$$
\begin{align*}
p_v(z) &= (z - \lambda_1) \\
p_v(z) &= (z - \lambda_2) \\
p_v(z) &= (z-\lambda_1)(z - \lambda_2) \\
\end{align*} 
$$.

Since $p$ is a multiple of $p_v$, then

either $\lambda_1$ or $\lambda_2$ or both are zeros of the $p$.
Then $\lambda_1$ or $\lambda_2$ or both are eigenvalues of $T$.

From "5.41 determination of eigenvalues from upper-triangular matrix",
we know $\lambda_1$ or $\lambda_2$ appears on the diagonal of $𝐴$.

$\square$

### 5C.9

Suppose $𝐵$ is a square matrix with complex entries.
Prove that there exists
an invertible square matrix $𝐴$ with complex entries such that
$𝐴^{−1}𝐵𝐴$ is an upper-triangular matrix.

**Proof**:

Let $B$ be an $n$ by $n$ matrix.
Consider $V = \mathbb{C}^n$. $T$ is an operator in $L(V)$ such that
$\mathcal{M}(T)$ under the standard basis is $B$, i.e.
$B = \mathcal{M}(T, (e_1, \cdots, e_n))$.

Use "5.47 if $𝐅 = 𝐂$, then every operator on 𝑉 has an upper-triangular 
matrix", then we know we can find a basis
$v_1, \cdots, v_n$ such that $D = \mathcal{M}(T, (v_1, \cdots, v_n))$
is a upper-triangular matrix.

Then we can directly apply "3.84 change-of-basis formula" and let

$$ 
A = \mathcal{M}(I,(v_1, \cdots, v_n),(e_1, \cdots, e_n))
$$

Then we have $D = A^{-1} B A$.

$\square$

### 5C.10

Suppose $𝑇 ∈ ℒ(𝑉)$ and $𝑣_1, …, 𝑣_𝑛$ is a basis of $𝑉$.
Show that the following are equivalent.

(a) The matrix of $𝑇$ with respect to $𝑣_1, …, 𝑣_𝑛$ is lower triangular.

(b) $\text{span}(𝑣_k, \cdots, 𝑣_n)$ is invariant under $𝑇$ for each
$𝑘 = 1, …, 𝑛$.

(c) $𝑇{𝑣_𝑘} ∈ \text{span}(𝑣_k, \cdots, 𝑣_n)$ for each $𝑘 = 1, …, 𝑛$.

A square matrix is called lower triangular if all entries above
the diagonal are $0$.

**Proof**:

$(a) \Rightarrow (b)$

Fix any $𝑘 = 1, …, 𝑛$ and $k \leq j \leq n$.

Since The matrix of $𝑇$ with respect to $𝑣_1, …, 𝑣_𝑛$ is lower triangular, then $𝑇{𝑣_j}$ is the linear combination of
$𝑣_j, \cdots, 𝑣_n$, so
$T v_j \in \text{span}(𝑣_j, \cdots, 𝑣_n) \subseteq \text{span}(𝑣_k, \cdots, 𝑣_n)$.

So $\text{span}(𝑣_k, \cdots, 𝑣_n)$ is invariant under $𝑇$.

$(b) \Rightarrow (c)$

$\text{span}(𝑣_k, \cdots, 𝑣_n)$ is invariant under $𝑇$, then
$𝑇{𝑣_𝑘} ∈ \text{span}(𝑣_k, \cdots, 𝑣_n)$.

$(c) \Rightarrow (a)$

$𝑇{𝑣_𝑘} ∈ \text{span}(𝑣_k, \cdots, 𝑣_n)$, then
$𝑇{𝑣_𝑘}$ is a linear combination of $𝑣_k, \cdots, 𝑣_n$.
Then the coefficients of $v_1, \cdots, v_{k-1}$ are all $0$.
This means the matrix of $𝑇$ with respect to $𝑣_1, …, 𝑣_𝑛$ is lower 
triangular.

$\square$

### 5C.11

Suppose $𝐅 = 𝐂$ and $𝑉$ is finite-dimensional.
Prove that if $𝑇 ∈ ℒ(𝑉)$, then
there exists a basis of $𝑉$ with respect to which $𝑇$ has a 
lower-triangular matrix.

**Proof**:

Use "5.47 if $𝐅 = 𝐂$, then every operator on 𝑉 has an upper-triangular 
matrix", then we can find a basis $v_1, \cdots, v_n$ such that
$\mathcal{M}(T)$ is a upper-triangular matrix.

Now use "5.39 conditions for upper-triangular matrix", we know
$\text{span}(𝑣_1, \cdots, 𝑣_k)$ is invariant under $T$
for $k = 1, \cdots, n$.

Now let $w_n = v_1, \cdots, w_1 = v_n$. We can see

$\text{span}(w_k, \cdots, w_n) = \text{span}(v_1, \cdots, v_{n-k+1})$ is invariant under $𝑇$.

Then apply exercise 5C.10 above, we get
$\mathcal{M}(T)$ is a lower-triangular matrix under the basis
$w_1, \cdots, w_n$.

$\square$

### 5C.12

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉)$ has an upper-triangular 
matrix with respect to some basis of $𝑉$, and $𝑈$ is a subspace of
$𝑉$ that is invariant under $𝑇$.

(a) Prove that $T|_U$ has an upper-triangular matrix with respect to some basis of $𝑈$.

**Proof**:

Let $p(z)$ be the minimal polynomial of $T$, and $q(z)$ be
the minimal polynomial of $T|_U$. 

From
"5.44 necessary and sufficient condition to have an
upper-triangular matrix", we know

$$ 
p(z) = (z-\lambda_1) \cdots (z-\lambda_m)
$$

Then from "5.31 minimal polynomial of a restriction operator",
$p(z)$ is a multiple of $q(z)$.

Then $q(z)$ has to be in the form of

$$ 
q(z) = (z-\alpha_1) \cdots (z-\alpha_l)
$$

Then again apply 5.44, we know
$T|_U$ has an upper-triangular matrix with respect to some basis of $𝑈$.

$\square$

(b) Prove that the quotient operator $𝑇/𝑈$ has an upper-triangular matrix 
with respect to some basis of $𝑉/𝑈$.

**Proof**: The logic is very similar to part (a).

Let $p(z)$ be the minimal polynomial of $T$, and $q(z)$ be
the minimal polynomial of $T/U$. 

From exercise 5B.25 part (a),
the minimal polynomial of $𝑇$ is a polynomial multiple of the
minimal polynomial of the quotient operator $𝑇/𝑈$.

Then the other part is exactly the same as part (a).

$\square$

### 5C.13

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$.
Suppose there exists
a subspace $𝑈$ of $𝑉$ that is invariant under $𝑇$ such that
$𝑇|_𝑈$ has an upper-triangular matrix with respect to some basis of $𝑈$ 
and also $𝑇/𝑈$ has an
upper-triangular matrix with respect to some basis of $𝑉/𝑈$.
Prove that $𝑇$ has
an upper-triangular matrix with respect to some basis of $𝑉$.

**Proof**:

Let $p(z)$ be the minimal polynomial of $T$, $q(z)$ be that of
$T|_U$ and $s(z)$ be that of $T/U$.

From
"5.44 necessary and sufficient condition to have an
upper-triangular matrix",

we have

$$ 
q(z) = (z-\alpha_1) \cdots (z-\alpha_l) \\
s(z) = (z-\beta_1) \cdots (z-\beta_m)
$$

From the exercise 5B.25 (b) we know that
(minimal polynomial of $𝑇|_𝑈$) $×$ (minimal polynomial of $𝑇/𝑈$)
is a polynomial multiple of the minimal polynomial of 𝑇.

Then due to unique factorization in $F[z]$ we have

$$ 
p(z) = (z-\gamma_1) \cdots (z-\gamma_k)
$$

Then again use 5.44, we know
$𝑇$ has
an upper-triangular matrix with respect to some basis of $𝑉$.

$\square$

### 5C.14

Suppose $𝑉$ is finite-dimensional and
$𝑇 ∈ ℒ(𝑉)$. Prove that $𝑇$ has an upper-
triangular matrix with respect to some basis of $𝑉$
if and only if the dual
operator $𝑇'$ has an upper-triangular matrix with respect to
some basis of the dual space $𝑉'$

**Proof**:

We use exercise 5B.28, which states
that the minimal
polynomial of $𝑇' ∈ ℒ(𝑉')$ equals the minimal polynomial of $𝑇$.

And then we can use
"5.44 necessary and sufficient condition to have an
upper-triangular matrix" again.

$\square$
.