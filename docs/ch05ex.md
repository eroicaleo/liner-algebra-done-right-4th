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
