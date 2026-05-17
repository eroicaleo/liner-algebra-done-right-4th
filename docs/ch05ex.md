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