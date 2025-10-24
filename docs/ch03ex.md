# Chapter 3 Linear Maps

## Section 3A Vector Space of Linear Maps

### 3A.1

Suppose $𝑏, 𝑐 ∈ 𝐑$. Define $𝑇 ∶ 𝐑^3 → 𝐑^2$ by

$$ 
𝑇(𝑥, 𝑦, 𝑧) = (2𝑥 − 4𝑦 + 3𝑧 + 𝑏, 6𝑥 + 𝑐𝑥𝑦𝑧).
$$

Show that $𝑇$ is linear if and only if $𝑏 = 𝑐 = 0$.

**Proof**:

$\Rightarrow$

$T(0) = (b, 0) = (0,0)$, so $b = 0$.

$T(2,2,2) = (2, 12 + 8c) = 2T(1,1,1) = 2(1, 6 + c)$

So $8c = 2c$, then $c = 0$.

$\square$

### 3A.2

Suppose $𝑏, 𝑐 ∈ 𝐑$. Define $𝑇 ∶ 𝒫(𝐑) → 𝐑^2$ by

$$ 
𝑇𝑝 = (3𝑝(4) + 5𝑝'(6) + 𝑏𝑝(1)𝑝(2), \int_{-1}^{2} 𝑥^3 𝑝(𝑥) 𝑑𝑥 + 𝑐 \sin 𝑝(0)).
$$

Show that $𝑇$ is linear if and only if $𝑏 = 𝑐 = 0$.

**Proof**:

Consider $p(x) = 1$, then

$$ 
3𝑝(4) + 5𝑝'(6) + 𝑏𝑝(1)𝑝(2) = 3 + 0 + b \\
3(2𝑝)(4) + 5(2𝑝)'(6) + 𝑏(2𝑝)(1)(2𝑝)(2) = 6 + 0 + 4b \\
$$

So $b = 0$.

Consider $p(x) = \pi / 4$, then

$$ 
T(2p)[1] = \int_{-1}^{2} 𝑥^3 2 (\frac{\pi}{4}) dx + c \cdot 1
$$

On the other hand

$$ 
T(2p)[1] = 2 T(p) [1] = 2 \int_{-1}^{2} 𝑥^3 (\frac{\pi}{4}) dx
+ c \cdot \frac{\sqrt[]{2}}{2}
$$

So $c = 0$.

$\square$

### 3A.3

Suppose that $𝑇 ∈ ℒ(𝐅^𝑛, 𝐅^𝑚)$. Show that there exist scalars $𝐴_{𝑗,𝑘} ∈ 𝐅$ for $𝑗 = 1, …, 𝑚$ and $𝑘 = 1, …, 𝑛$ such that

$$ 
𝑇(𝑥_1, …, 𝑥_𝑛) =
(𝐴_{1, 1} 𝑥_1 +⋯ + 𝐴_{1, 𝑛} 𝑥_𝑛, …, 𝐴_{𝑚, 1} 𝑥_1 +⋯ + 𝐴_{𝑚, 𝑛} 𝑥_𝑛)
$$

for every $(𝑥_1, …, 𝑥_𝑛) ∈ 𝐅_𝑛$.

**Proof**:

Let

$$ 
T(e_1) = (A_{1,1}, A_{2,1}, \cdots, A_{m,1}) \\
T(e_2) = (A_{1,2}, A_{2,2}, \cdots, A_{m,2}) \\
\cdots \\
T(e_n) = (A_{1,n}, A_{2,n}, \cdots, A_{m,n}) \\
$$

$\square$

### 3A.4

Suppose $𝑇 ∈ ℒ(𝑉, 𝑊)$ and $𝑣_1, …, 𝑣_𝑚$ is a list of vectors 
in $𝑉$ such that $𝑇𝑣_1, …, 𝑇𝑣_𝑚$ is a linearly independent 
list in $𝑊$. Prove that $𝑣_1, …, 𝑣_𝑚$ is linearly independent.

**Proof**:

Assume

$$ 
a_1 v_1 + \cdots + a_m v_m = 0
$$

Then

$$ 
T(a_1 v_1 + \cdots + a_m v_m) = a_1 Tv_1 + \cdots + a_m Tv_m = 0
$$

So $a_1 = \cdots = a_m = 0$.

$\square$

### 3A.5

### 3A.6

### 3A.7

Show that every linear map from a one-dimensional vector space to 
itself is multiplication by some scalar. More precisely, prove that 
if $\dim 𝑉 = 1$ and $𝑇 ∈ ℒ(𝑉)$, then there exists $𝜆 ∈ 𝐅$ such 
that $𝑇𝑣 = 𝜆𝑣$ for all $𝑣 ∈ 𝑉$.

**Proof**:

Assume $v_0$ is a basis of $V$. Let $w_0 = Tv_0 \in V$.
We can assume $w_0 = 𝜆 v_0$ 
Then assume $v = a v_0$.

$$ 
Tv = T a v_0 = a T v_0 = a 𝜆 v_0 = 𝜆 a v_0 = 𝜆 v
$$

$\square$

### 3A.8

Give an example of a function $𝜑 ∶ 𝐑^2 → 𝐑$ such that

$$ 
𝜑(𝑎𝑣) = 𝑎𝜑(𝑣)
$$

for all $𝑎 ∈ 𝐑$ and all $𝑣 ∈ 𝐑^2$ but $𝜑$ is not linear.

**Solution**:

Consider the norm function:

$$ 
𝜑(𝑣) = \left\| v \right\| = \sqrt[]{v_1^2 + v_2^2}
$$

$\square$

### 3A.9

Give an example of a function $𝜑 ∶ 𝐂 → 𝐂$ such that

$$ 
𝜑(𝑤 + 𝑧) = 𝜑(𝑤) + 𝜑(𝑧)
$$

for all $𝑤, 𝑧 ∈ 𝐂$ but $𝜑$ is not linear.
(Here $𝐂$ is thought of as a complex vector space.)

**Solution**:

Consider $𝜑(𝑤) = \overline{w}$.

Then let $w = i, a = i$.

$$ 
𝜑(a𝑤) = 𝜑(-1) = -1 \\
a 𝜑(𝑤) = i 𝜑(i) = i (-i) = 1 \\
$$

$\square$

### 3A.10

Prove or give a counterexample: If $𝑞 ∈ 𝒫(𝐑)$ and
$𝑇 ∶ 𝒫(𝐑) → 𝒫(𝐑)$ is defined by 𝑇𝑝 = 𝑞 ∘ 𝑝, then $𝑇$ is a 
linear map.

**Solution**: We provide a counterexample.

Let $q = x + 1, p = 1$.

$$ 
T(p)(0) = q(p(0)) = q(1) = 2 \\
T(2p)(0) = q(2p(0)) = q(2) = 3 \\
$$

$\square$

### 3A.11

Suppose $𝑉$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉)$.
Prove that 𝑇 is a scalar multiple of the identity if and only if 
$𝑆𝑇 = 𝑇𝑆$ for every $𝑆 ∈ ℒ(𝑉)$.

**Proof**:

$\Rightarrow$ is obvious. 

Given $v_1, \cdots, v_m$ is a basis with $m \geq 2$.
$T$ is not a zero map. Without loss of generality, assume

$$ 
T(v_1) = w_1 = a_1 v_1 + \cdots + a_m v_m \neq 0.
$$

Let $S(v_1) = v_1, S(v_i) = 0$ for $i \neq 1$.
Then

$$ 
TS(v_1) = T(v_1) = a_1 v_1 + \cdots + a_m v_m \\
ST(v_1) = S(a_1 v_1 + \cdots + a_m v_m)
= a_1 v_1
$$

So $T(v_1) = a_1 v_1$. For the same reason, $T(v_i) = a_i v_i$.

Now consider $S(v_1) = v_2, S(v_2) = v_1, S(v_i) = 0$ for all other
$i$.

$$ 
TS(v_1) = T(v2) = a_2 v_2 \\
ST(v_1) = S(a_1 v_1) = a_1 v_2 \\
$$

So $a_1 = a_2 = \cdots = a_n$.

$\square$

### 3A.12

Suppose $𝑈$ is a subspace of $𝑉$ with $𝑈 ≠ 𝑉$.
Suppose $𝑆 ∈ ℒ(𝑈, 𝑊)$ and $𝑆 ≠ 0$ (which means that
$𝑆𝑢 ≠ 0$ for some $𝑢 ∈ 𝑈$). Define $𝑇 ∶ 𝑉 → 𝑊$ by

$$ 
T v =
\begin{cases}
    S v &\text{if } v \in U \\
    0 &\text{if }  v \in V \text{ and } v \not\in U. \\
\end{cases}
$$

Prove that 𝑇 is not a linear map on 𝑉 .

**Proof**:

Consider $v \in U, S(v) \neq 0$, $w \not\in U$, then $v + w \not\in U$.

$$ 
0 = S(v + w) = S(v) + S(w) = S(v)
$$

So we have a contradition.

$\square$

### 3A.13

Suppose $𝑉$ is finite-dimensional. Prove that every linear map on a 
subspace of $𝑉$ can be extended to a linear map on $𝑉$ . In other 
words, show that if $𝑈$ is a subspace of $𝑉$ and $𝑆 ∈ ℒ(𝑈, 𝑊)$, 
then there exists $𝑇 ∈ ℒ(𝑉, 𝑊)$ such that
$𝑇𝑢 = 𝑆𝑢$ for all $𝑢 ∈ 𝑈$.

**Proof**:

Consider $U$ is a subspace, $u_1, \cdots, u_m$ is a basis of $U$.
Let $w_i = S(u_i)$. We can extend $u_1, \cdots, u_m$ to
$u_1, \cdots, u_m, v_1, \cdots, v_n$.

Let $T(u_i) = w_i, T(v_j) = 0$, then from 3.4 linear map lemma,
$T$ satisfy $𝑇𝑢 = 𝑆𝑢$ for all $𝑢 ∈ 𝑈$.

$\square$

### 3A.14

Suppose $𝑉$ is finite-dimensional with $\dim 𝑉 > 0$, and suppose 
$𝑊$ is infinite-dimensional. Prove that $ℒ(𝑉, 𝑊)$ is 
infinite-dimensional.

**Proof**:

Assume $\dim ℒ(𝑉, 𝑊) = n$,
and $v_1, \cdots, v_m$ is a basis of of $V$.

Also assume $w_1, \cdots, w_{n+1}$ is linear independent in $W$.

Let $T_1, \cdots, T_{n+1}$ are linear mappings such that
$T_i(v_1) = w_i$.

Since $\dim ℒ(𝑉, 𝑊) = n$, then $T_1, \cdots, T_{n+1}$ are linear
dependent, i.e.

$$ 
a_1 T_1 + \cdots + a_{n+1} T_{n+1} = 0, a_i \text{ are not all 0}
$$

Then

$$ 
(a_1 T_1 + \cdots + a_{n+1} T_{n+1})(v_1) = \\
a_1 w_1 + \cdots + a_{n+1} w_{n+1} = 0
$$

So $w_1, \cdots, w_{n+1}$ is linear dependent. We have a 
contradition.

### 3A.15

Suppose $𝑣_1, …, 𝑣_𝑚$ is a linearly dependent list of vectors in 
$𝑉$ . Suppose also that $𝑊 ≠ \{0\}$.
Prove that there exist $𝑤_1, …, 𝑤_𝑚 ∈ 𝑊$ such that no
$𝑇 ∈ ℒ(𝑉, 𝑊)$ satisfies $𝑇𝑣_𝑘 = 𝑤_𝑘$ for each
$𝑘 = 1, …, 𝑚$.

**Proof**:

We can find

$$ 
a_1 v_1 + \cdots + a_m v_m = 0, a_i \text{ are not all 0}
$$

Without loss of generality, assume $a_1 \neq 0$.

Then let $w_1 \neq 0, w_2 = \cdots = w_m = 0$.

If $𝑇𝑣_𝑘 = 𝑤_𝑘$ for each $𝑘 = 1, …, 𝑚$

Then

$$ 
0 = T(0) = T(a_1 v_1 + \cdots + a_m v_m) =
a_1 T(v_1) + \cdots + a_m T(v_m) = a_1 w_1 \neq 0
$$

So $T$ does not exist.

### 3A.16

Suppose $𝑉$ is finite-dimensional with $\dim 𝑉 > 1$. Prove that 
there exist $𝑆, 𝑇 ∈ ℒ(𝑉)$ such that $𝑆𝑇 ≠ 𝑇𝑆$.

**Proof**:

Consider $v_1, v_2, \cdots, v_m$ is a basis of $V$.

Let $T(v_1) = v_1, T(v_2) = 2 v_2$, $S(v_1) = v_2, S(v_2) = v_1$.
And $T(v_i) = S(v_i) = 0$ for all other $i \neq 1, 2$.

Then

$$ 
ST(v_1) = v_2 \\
TS(v_1) = T(v_2) = 2 v_2 \\
$$

Since $v_2 \neq 0$, then $ST(v_1) \neq TS(v_2)$.

$\square$

### 3A.17

Suppose $𝑉$ is finite-dimensional. Show that the only two-sided 
ideals of $ℒ(𝑉)$ are $\{0\}$ and $ℒ(𝑉)$.

A subspace $ℰ$ of $ℒ(𝑉)$ is called a two-sided ideal of $ℒ(𝑉)$ if
$𝑇𝐸 ∈ ℰ$ and $𝐸𝑇 ∈ ℰ$ for all $𝐸 ∈ ℰ$ and all $𝑇 ∈ ℒ(𝑉)$.

**Proof**: I cannot figure it out now.

$\square$
