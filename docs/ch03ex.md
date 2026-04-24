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

## Section 3B Null Spaces and Ranges

### 3B.1

Give an example of a linear map $𝑇$ with dim null $𝑇 = 3$ and dim range $𝑇 = 2$.

**Solution**:

Consider $T : \mathbb{R}^5 \longrightarrow \mathbb{R}^2$

$$
T(r_1, r_2, r_3, r_4, r_5) = (r_1, r_2)
$$

It is surjective, so dim range $𝑇 = 2$.

Note $(0, 0, 1, 0, 0), (0,0,0,1,0), (0,0,0,0,1)$ is a basis of $\text{null } T$,
so dim null $𝑇 = 3$.

$\square$

### 3B.2

Suppose $𝑆, 𝑇 ∈ ℒ(𝑉)$ are such that range $𝑆 ⊆ \text{null } T$. Prove that $(𝑆𝑇)^2 = 0$.

**Proof**:

Given any $v \in S$

$$
((𝑆𝑇)^2)(v) = (ST)((ST)(v)) =
S(T(S(T(v))))
$$

Note $S(T(v)) \in \text{range } S \subseteq \text{null } T$.

So $S(T(S(T(v)))) = S(0) = 0$.

$\square$

### 3B.3

Suppose $𝑣_1, …, 𝑣_𝑚$ is a list of vectors in $𝑉$.
Define $𝑇 ∈ ℒ(𝐅^𝑚 , 𝑉)$ by

$$
T (z_1, \cdots, z_m) = z_1 v_1 + \cdots + z_m v_m
$$

Anwser:

(a) What property of $𝑇$ corresponds to $v_1, \cdots, v_m$ spanning $𝑉$?

**Solution**:

When $T$ is surjective.

(b) What property of $𝑇$ corresponds to the list $v_1, \cdots, v_m$ being linearly
independent?

**Solution**:

When $T$ is injective.

### 3B.4

Show that $\{𝑇 ∈ ℒ(𝐑^5 , 𝐑^4) ∶ \text{dim null } T > 2\}$ is not a subspace of
$ℒ(\mathbb{R}^5, \mathbb{R}^4)$.

**Solution**:

Consider the following 2 maps:

$$
S(r_1, r_2, r_3, r_4, r_5) = (r_1, r_2, 0, 0) \\
T(r_1, r_2, r_3, r_4, r_5) = (0, 0, r_3, r_4) \\
$$

Then we have

$$
(S+T)(r_1, r_2, r_3, r_4, r_5) = (r_1, r_2, r_3, r_4)
$$

So $\text{dim null } (S+T) = 1$.

This set is not closed under addition.

$\square$

### 3B.5

Give an example of $𝑇 ∈ ℒ(𝐑^4)$ such that $\text{range } T = \text{null } T$.

**Solution**:

Consider

$$
T(r_1, r_2, r_3, r_4) = (0, 0, r_1, r_2)
$$

Then

$$
\text{null } T = \{(0, 0, r_3, r_4)\} = \text{range } T
$$

$\square$

### 3B.6

Prove that there does not exist $𝑇 ∈ ℒ(𝐑^5)$ such that $\text{range } T = \text{null } T$.

**Proof**:

From 3.21 fundamental theorem of linear maps,

$$
\text{dim null } T + \text{dim range } T = 5
$$

So

$$
\text{dim null } T \neq \text{dim range } T
$$

Then $\text{null } T \neq \text{range } T$.

$\square$

### 3B.7

Suppose $𝑉$ and $𝑊$ are finite-dimensional with $2 ≤ \dim 𝑉 ≤ \dim 𝑊$.
Show that $\{𝑇 ∈ ℒ(𝑉, 𝑊) ∶ 𝑇 \text{ is not injective}\}$
is not a subspace of $ℒ(𝑉, 𝑊)$.

**Proof**:

Let $v_1, \cdots, v_m$ is a basis of $V$ and
$w_1, \cdots, w_m$ is linear independent vector.

Let $T(v_1) = w_1, T(v_i) = 0$, $S(v_1) = 0, S(v_i) = w_i$.

So $(S+T)(v_i) = w_i$. $S+T$ is injective.

This set is not closed under addition.

$\square$

### 3B.8

Suppose $𝑉$ and $𝑊$ are finite-dimensional with $2 ≤ \dim W ≤ \dim V$.
Show that $\{𝑇 ∈ ℒ(𝑉, 𝑊) ∶ 𝑇 \text{ is not surjective}\}$
is not a subspace of $ℒ(𝑉, 𝑊)$.

**Proof**:

Let $w_1, \cdots, w_m$ is a basis of $W$ and
$v_1, \cdots, v_m$ is linear independent vector.

Let $T(v_1) = w_1, T(v_i) = 0$, $S(v_1) = 0, S(v_i) = w_i$.

So $(S+T)(v_i) = w_i$. $S+T$ is surjective.

This set is not closed under addition.

$\square$

### 3B.9

Suppose $𝑇 ∈ ℒ(𝑉, 𝑊)$ is injective and $v_1, \cdots, v_n$ is linearly independent in $𝑉$.
Prove that $𝑇𝑣_1, …, 𝑇𝑣_𝑛$ is linearly independent in 𝑊.

**Proof**:

If

$$
a_1 Tv_1 + \cdots + a_m Tv_m = 0
$$

Then

$$
T(a_1 v_1 + \cdots + a_m v_m) = 0
$$

Since $T$ is injective, so

$$
a_1 v_1 + \cdots + a_m v_m = 0
$$

Then $a_1 = \cdots = a_m = 0$. Thus $𝑇𝑣_1, …, 𝑇𝑣_𝑛$ is linearly independent in 𝑊.

$\square$

### 3B.10

Suppose $𝑣_1, …, 𝑣_𝑛$ spans $𝑉$ and $𝑇 ∈ ℒ(𝑉, 𝑊)$.
Show that $𝑇𝑣_1, …, 𝑇𝑣_𝑛$  spans $\text{range } T$.

**Proof**:

Let $w \in \text{range } T$, then $T(v) = w$.

Let $v = a_1 v_1 + \cdots + a_n v_n$, so

$$
T (a_1 v_1 + \cdots + a_n v_n) = a_1 Tv_1 + \cdots + a_n Tv_n = w
$$

$\square$

### 3B.11

Suppose that $𝑉$ is finite-dimensional and that 𝑇 ∈ ℒ(𝑉, 𝑊). Prove that there
exists a subspace 𝑈 of 𝑉 such that

$$
U \cap \text{null } T = \{0\}
\quad
\text{and}
\quad
\text{range } T = \{Tu : u \in U\}
$$

**Proof**:

Let $v_1, \cdots, v_m$ be a basis of $\text{null } T$, we can extend a basis of $V$
it to $v_1, \cdots, v_m, w_1, \cdots, w_n$.

Let $U = \text{span}(w_1, \cdots, w_n)$.

If $u \in \text{range } T$, and $T(v) = u$

$$
v = a_1 v_1 + \cdots + a_m v_m + b_1 w_1 + \cdots + b_n w_n
$$

So

$$
u = T(v) = T (a_1 v_1 + \cdots + a_m v_m + b_1 w_1 + \cdots + b_n w_n) \\
= T(a_1 v_1 + \cdots + a_m v_m) + T(b_1 w_1 + \cdots + b_n w_n) \\
= T(b_1 w_1 + \cdots + b_n w_n)
$$

$\square$

### 3B.12

Suppose $𝑇$ is a linear map from $𝐅^4$ to $𝐅^2$
such that

$$
\text{null } T
=
\{
(𝑥_1, 𝑥_2, 𝑥_3, 𝑥_4) ∈ 𝐅^4 ∶ 𝑥_1 = 5𝑥_2
\text{ and } 𝑥_3 = 7𝑥_4
\}
$$

Prove that $𝑇$ is surjective.

**Proof**:

Note

$$
v_1 = (5, 1, 0, 0) \\
v_2 = (0, 0, 7, 1) \\
$$

is a basis of $\text{null } T$,
so $\dim \text{range } T = 2$.

Then $𝑇$ is surjective.

### 3B.13

Suppose $𝑈$ is a three-dimensional subspace of
$𝐑^8$ and that $𝑇$ is a linear map
from $𝐑^8$ to $𝐑^5$ such that $\text{null } T = 𝑈$.
Prove that $𝑇$ is surjective.

**Proof**:

Note $\text{dim range } T = 5$, and $\dim R^5 = 5$.
So $𝑇$ is surjective.

### 3B.14

Prove that there does not exist a linear map from
$𝐅_5$ to $𝐅_2$ whose null space equals

$$
\{
(𝑥_1, 𝑥_2, 𝑥_3, 𝑥_4, 𝑥_5) ∈ 𝐅^5
∶
𝑥_1 = 3𝑥_2
\text{ and }
𝑥_3 = 𝑥_4 = 𝑥_5
\}
$$

**Proof**:

Assume $T$ exists. Note

$$
v_1 = (3, 1, 0, 0, 0) \\
v_2 = (0, 0, 1, 1, 1) \\
$$

is a basis of $\text{null } T$, so
$\text{dim range } T$ has to be $3$.

But $\mathbb{R}^2$ is only 2 dimensional.
So $T$ does not exist.

$\square$

### 3B.15

Suppose there exists a linear map on $𝑉$ whose null
space and range are both
finite-dimensional.
Prove that $𝑉$ is finite-dimensional.

**Proof**:

Assume otherwise, $u_1, \cdots, u_m$ is a basis
of $\text{null } T$ and $v_1, \cdots, v_n$ such
that $Tv_1, \cdots, Tv_n$ is a basis of
$\text{range } T$.

We can see $V = \text{null } T + \text{span}(𝑣_1, \cdots, 𝑣_n)$.

From 2.43 dimension of a sum, we can see

$$
\dim V \leq \text{dim null } T + \dim
\text{span}(𝑣_1, \cdots, 𝑣_n)
$$

$\square$

### 3B.16

Suppose 𝑉 and 𝑊 are both finite-dimensional. Prove that there
exists an injective linear map from 𝑉 to 𝑊 if and only if
dim 𝑉 ≤ dim 𝑊.

**Proof**:

$\Rightarrow$

It's the contrapositive of 3.22, i.e. linear map to a
lower-dimensional space is not injective.

$\Leftarrow$

Assume $\dim V = m$, and $v_1, \cdots, v_m$ is a basis of
$V$, and $w_1, \cdots, w_m$ is linearly independent in $W$.

Let $T$ be a linear map such that $T(v_i) = w_i$.
Then if

$$
T(a_1 v_1 + \cdots + a_m v_m) = 0 \\
\Rightarrow \\
a_1 Tv_1 + \cdots + a_m Tv_m \\
\Rightarrow \\
a_1 w_1 + \cdots + a_m w_m = 0 \\
\Rightarrow \\
a_1 = \cdots = a_m = 0
$$

So $\text{null } T = 0$, so $T$ is injective.

### 3B.17

Suppose 𝑉 and 𝑊 are both finite-dimensional. Prove that there
exists a surjective linear map from 𝑉 onto 𝑊 if and only if
dim 𝑉 ≥ dim 𝑊.

**Proof**:

$\Rightarrow$

It is the contrapositive of 3.24: linear map to a
higher-dimensional space is not surjective.

$\Leftarrow$

Assume $w_1, \cdots, w_m$ is a basis of $W$. $v_1, \cdots, v_m$
is linear independent in $V$. Extend it to a basis of $V$ by
adding $u_1, \cdots, u_n$.

Let $T v_i = w_i, T u_j = 0$. This map is surjective.

$\square$

### 3B.18

Suppose 𝑉 and 𝑊 are finite-dimensional and that 𝑈 is a
subspace of 𝑉 .
Prove that there exists 𝑇 ∈ ℒ(𝑉, 𝑊) such that null 𝑇 = 𝑈 if
and only if dim 𝑈 ≥ dim 𝑉 − dim 𝑊.

**Proof**:

$\Rightarrow$

$$
\dim V = \text{dim null } T + \text{dim range } T \\
\Rightarrow \\
\dim U = \dim V - \text{dim range } T \\
\Rightarrow \\
\dim U \geq  \dim V - \dim W \\
$$

$\Leftarrow$

Let $u_1, \cdots, u_m$ be a basis of $U$, extend it to a basis
of $V$ by adding $v_1, \cdots, v_n$.

Since $\dim U \geq  \dim V - \dim W$, then $\dim W \geq n$.
We can find $w_1, \cdots, w_n \in W$ such that they are independent
in $W$.

Let $T u_i = 0, T v_j = w_j$.

$\square$

### 3B.19

Suppose 𝑊 is finite-dimensional and 𝑇 ∈ ℒ(𝑉, 𝑊). Prove that 𝑇
is injective
if and only if there exists 𝑆 ∈ ℒ(𝑊, 𝑉) such that 𝑆𝑇 is the
identity operator on 𝑉 .

**Proof**:

$\Rightarrow$

First, since $T$ is injective, $V$ has to be finite-dimensional
because of 3.22.

Assume $v_1, \cdots, v_m$ is a basis of $V$.

Also assume

$$
a_1 Tv_1 + \cdots + a_m Tv_m = 0 \\
\Rightarrow \\
T(a_1 v_1 + \cdots + a_m v_m) = 0 \\
\Rightarrow \\
a_1 v_1 + \cdots + a_m v_m \in \text{null } T \\
\Rightarrow \text{ T is injective } \\
a_1 v_1 + \cdots + a_m v_m = 0 \\
\Rightarrow \\
a_1 = \cdots = a_m = 0 \\
\Rightarrow \\
Tv_1, \cdots, Tv_m \text{ is independent }
$$

Then extend $Tv_1, \cdots, Tv_m$ to a basis of $W$ by adding
$w_1, \cdots, w_n$. Consider $S$ as $S(T v_i) = v_i, S(w_j) = 0$.

Then we have $ST$ is the identity operator on 𝑉.

$\Leftarrow$

If $T(v) = 0$, then $v = ST(v) = S(0) = 0$.
So $T$ is injective.

$\square$

### 3B.20

Suppose 𝑊 is finite-dimensional and 𝑇 ∈ ℒ(𝑉, 𝑊). Prove that 𝑇
is surjective
if and only if there exists 𝑆 ∈ ℒ(𝑊, 𝑉) such that 𝑇𝑆 is the
identity operator on 𝑊.

**Proof**:

$\Rightarrow$

$w_1, \cdots, w_m$ is a basis of $W$, and $T(v_i) = w_i$.

$$
a_1 v_1 + \cdots + a_m v_m = 0 \\
\Rightarrow \\
T(a_1 v_1 + \cdots + a_m v_m) = 0 \\
\Rightarrow \\
a_1 Tv_1 + \cdots + a_m Tv_m = 0 \\
\Rightarrow \\
a_1 w_1 + \cdots + a_m w_m = 0 \\
\Rightarrow \\
a_1 = \cdots = a_m = 0 \\
\Rightarrow \\
v_1, \cdots, v_m \text{ is linear independent.}
$$

Let $S(w_i) = v_i$, then if $w = a_1 w_1 + \cdots + a_m w_m$,
then

$$
TS(w) = T(a_1 Sw_1 + \cdots + a_m Sw_m) \\
= T(a_1 v_1 + \cdots + a_m v_m) \\
= a_1 Tv_1 + \cdots + a_m Tv_m \\
= a_1 w_1 + \cdots + a_m w_m \\
= w
$$

$\Leftarrow$

If $TS$ is the identity operator. For any given $w$,
$TS(w) = w$, $S(w) \in V$. So $T$ is surjective.

$\square$

### 3B.21

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉, 𝑊)$, and $𝑈$
is a subspace of $𝑊$.
Prove that $\{𝑣 ∈ 𝑉 ∶ 𝑇𝑣 ∈ 𝑈\}$ is a subspace of $𝑉$ and

$$
\dim
\{
v \in 𝑉 ∶ 𝑇𝑣 ∈ 𝑈
\}
=
\text{dim null } T +
\dim (𝑈 ∩ \text{range } T)
$$

**Proof**:

We first show $\{𝑣 ∈ 𝑉 ∶ 𝑇𝑣 ∈ 𝑈\}$ is a subspace of $V$.

Let $A = \{𝑣 ∈ 𝑉 ∶ 𝑇𝑣 ∈ 𝑈\}$, $v_1, v_2 \in A$, then we can find
$Tv_1 = a_1 \in U, Tv_2 = a_2 \in U$, so $T(v_1 + v_2) = a_1 + a_2 \in U$.

$T(k v_1) = k T(v_1) = k a_1 \in U$.

So $A$ is a subspace of $V$.

Consider the linear mapping that limits $T$ on $A$ and call it $T|_A$.

$$
\dim A = \text{dim null } T|_A + \text{dim range } T|_A
$$

Note that $\text{null } T \subseteq A$, so $\text{dim null } T = \text{dim null } T|_A$.

Also $\text{range } T|_A = 𝑈 ∩ \text{range } T$, so

$$
\text{dim range } T|_A = \dim (𝑈 ∩ \text{range } T)
$$

$\square$

### 3B.22

Suppose 𝑈 and 𝑉 are finite-dimensional vector spaces and 𝑆 ∈ ℒ(𝑉, 𝑊) and
𝑇 ∈ ℒ(𝑈, 𝑉). Prove that

$$
\text{dim null } ST \leq \text{dim null } S + \text{dim null } T
$$

**Proof**:

Use the exercise 3B.21, Let $B = \text{null } S$, then

$$
\text{null } ST = \{u: Tu \in B\} = C
$$

So

$$
\dim C = \text{dim null } T + \dim (B \cap \text{range } T)
$$

And $\dim (B \cap \text{range } T) \leq \dim B = \text{dim null } S$.

$\square$

### 3B.23

Suppose 𝑈 and 𝑉 are finite-dimensional vector spaces and 𝑆 ∈ ℒ(𝑉, 𝑊) and
𝑇 ∈ ℒ(𝑈, 𝑉). Prove that

$$
\text{dim range } ST \leq \min \{\text{dim range } S, \text{dim range } T\}
$$

**Proof**:

If $w \in \text{range } ST$, then we can find $u$ such that $ST(u) = w$, i.e. $S(T(u)) = w$,
$w \in \text{range } S$. So $\text{range } ST \subseteq \text{range } S$.

Limit $S$ on $\text{range } T$.

$$
\text{dim range } T = \text{dim null } S|_{\text{range } T}
+ \text{dim range } S|_{\text{range } T}
\geq
\text{dim range } S|_{\text{range } T}
$$

Also $\text{range } S|_{\text{range } T} = \text{range } ST$.

So $\text{dim range } T \geq \text{dim range } ST$.

$\square$

### 3B.24

(a) Suppose dim 𝑉 = 5 and 𝑆, 𝑇 ∈ ℒ(𝑉) are such that 𝑆𝑇 = 0.
Prove that dim range 𝑇𝑆 ≤ 2.

**Proof**:

$\text{dim null } ST = 5$. So
$\text{dim null } T + \text{dim null } S \geq 5$.

So $\max \{\text{dim null } T , \text{dim null } S\} \geq 3$,
$\min \{\text{dim range } T , \text{dim range } S\} \leq 2$.

So $\text{dim range } TS \leq 2$.

$\square$

(b) Give an example of 𝑆, $𝑇 ∈ ℒ(𝐅^5)$ with 𝑆𝑇 = 0 and
dim range 𝑇𝑆 = 2.

**Solution**:

Consider $T(x_1, x_2, x_3, x_4, x_5) = (0, 0, 0, x_1, x_2)$,
$S(x_1, x_2, x_3, x_4, x_5) = (x_1, x_2, 0, 0, 0)$

$TS(x_1, x_2, x_3, x_4, x_5) = T(x_1, x_2, 0, 0, 0) = (0, 0, 0, x_1, x_2)$

$\square$

### 3B.25

Suppose that 𝑊 is finite-dimensional and 𝑆, 𝑇 ∈ ℒ(𝑉, 𝑊). Prove that
null 𝑆 ⊆ null 𝑇 if and only if there exists 𝐸 ∈ ℒ(𝑊) such that 𝑇 = 𝐸𝑆.

**Proof**:

$\Rightarrow$

Assume $Tv_1, \cdots, Tv_m$ is a basis of $\text{range } T$.
Then $v_1, \cdots, v_m$ is independent in $V$.

Then $Sv_1, \cdots, Sv_m$ is independent in $W$. This is because
assume

$$
a_1 Sv_1 + \cdots + a_m Sv_m = 0
$$

Then $a_1 v_1 + \cdots + a_m v_m \in \text{null } S \subseteq \text{null } T$

Then

$$
a_1 Tv_1 + \cdots + a_m Tv_m = 0
$$

So $a_1 = \cdots = a_m = 0$.

Then extend $Sv_1, \cdots, Sv_m$ to a basis of $\text{range } S$
by adding $Sr_1, \cdots, Sr_n$.

Consider

$$
A = \text{span}(𝑣_1, \cdots, 𝑣_𝑚, r_1, \cdots, r_n)
$$

First $𝑣_1, \cdots, 𝑣_𝑚, r_1, \cdots, r_n$ are independent:

$$
a_1 v_1 + \cdots + a_m v_m +
b_1 r_1 + \cdots + b_n r_n =
0 \\
\Rightarrow \\
a_1 Sv_1 + \cdots + a_m Sv_m +
b_1 Sr_1 + \cdots + b_n Sr_n =
0 \\
\Rightarrow \\
a_1 = \cdots = a_m = b_1 = \cdots = b_n = 0
$$

Note that we have $S|_A$ is injective. Because

$$
\dim A = m + n = \text{dim range } S = \text{dim range } S|_A \\
\Rightarrow \\
\text{dim null } S|_A = 0
$$

Then we have

$$
V = A \oplus \text{null } S
$$

Now, consider $T|_A$ We also have

$$
\dim A =
\text{dim range } T|_A + \text{dim null } T|_A \\
= \text{dim range } T + \text{dim null } T \cap A
$$

So we can find a basis of $\text{null } T \cap A$, i.e.,
$q_1, \cdots, q_n$, such that

$$
A = \text{span}(𝑣_1, \cdots, 𝑣_𝑚, q_1, \cdots, q_n)
$$

Note that $Sv_1, \cdots, Sv_m, Sq_1, \cdots, Sq_n$
are also independent in $W$ because $S|_A$ is injective.

Now, we can construct $E$ this way. We extend
$Sv_1, \cdots, Sv_m, Sq_1, \cdots, Sq_n$ to a basis of $W$ by
adding $w_1, \cdots, w_k$. Let
$E(Sv_i) = T v_i, E(Sq_j) = E(w_j) = 0$.

Given $v \in V$, we can right it as

$$
v =
(a_1 v_1 + \cdots + a_m v_m) +
(b_1 q_1 + \cdots + b_n q_n) + c
$$

Where $c \in \text{null } S$.

Then

$$
ES(v) =
(a_1 ESv_1 + \cdots + a_m ESv_m) +
(b_1 ESr_1 + \cdots + b_n ESr_n) + ESc \\
= a_1 Tv_1 + \cdots + a_m Tv_m
$$

On the other hand

$$
T(v) =
(a_1 Tv_1 + \cdots + a_m Tv_m) +
(b_1 Tq_1 + \cdots + b_n Tq_n) + Tc \\
= a_1 Tv_1 + \cdots + a_m Tv_m
$$

So $T = ES$.

$\Leftarrow$

If $v \in \text{null } S$, then $T(v) = ES(v) = E(0) = 0$.
So $v \in \text{null } T$. So
$\text{null } S \subseteq \text{null } T$

$\square$

### 3B.26

Suppose that 𝑉 is finite-dimensional and 𝑆, 𝑇 ∈ ℒ(𝑉, 𝑊). Prove
that range 𝑆 ⊆ range 𝑇 if and only if there exists 𝐸 ∈ ℒ(𝑉)
such that 𝑆 = 𝑇𝐸.

**Proof**:

$\Rightarrow$

Consider $w_1, \cdots, w_m$ is a basis of $\text{range } S$.
We can find

$$
Tv_1 = w_1, \cdots, Tv_m = w_m \\
Su_1 = w_1, \cdots, Su_m = w_m \\
$$

It's easy to prove $V = \text{span}(u_1, \cdots, u_𝑚) \oplus \text{null } S$.

Then let $p_1, \cdots, p_n$ be a basis of $\text{null } S$.
Together $u_1, \cdots, u_m, p_1, \cdots, p_n$ is a basis
of $V$.

Define $E(u_i) = v_i, E(p_j) = 0$.

Given $v \in V$, then

$$
v =
a_1 u_1 + \cdots + a_m u_m +
b_1 p_1 + \cdots + b_n p_n \\
\Rightarrow \\
S(v) =
a_1 Su_1 + \cdots + a_m Su_m +
b_1 Sp_1 + \cdots + b_n Sp_n \\
= a_1 Su_1 + \cdots + a_m Su_m \\
= a_1 w_1 + \cdots + a_m w_m
$$

Also

$$
TE(v) =
a_1 TEu_1 + \cdots + a_m TEu_m +
b_1 TEp_1 + \cdots + b_n TEp_n \\
= a_1 Tv_1 + \cdots + a_m Tv_m \\
= a_1 w_1 + \cdots + a_m w_m
$$

So $S = TE$.

$\Leftarrow$

Assume $w \in \text{range } S$, and assume $S(v) = w$, then
$TE(v) = w$, so $w \in \text{range } T$. Then
$\text{range } S ⊆ \text{range } T$.

$\square$

### 3B.27

Suppose 𝑃 ∈ ℒ(𝑉) and $𝑃^2 = 𝑃$. Prove that
$𝑉 = \text{null } P ⊕ \text{range } P$.

**Proof**:

Consider $v \in P$, then $v - P(v) \in \text{null } P$.

So $V = \text{null } P + \text{range } P$.

Assume $v \in \text{null } P \cap \text{range } P$.

Let $P(u) = v$. So $P^2(u) = P(P(u)) = P(v) = 0$.

On the other hand, $P^2(u) = P(u) = v$, so $v = 0$.

$\square$

### 3B.28

Suppose 𝐷 ∈ ℒ(𝒫(𝐑)) is such that deg 𝐷𝑝 = (deg 𝑝) − 1 for
every non-constant polynomial 𝑝 ∈ 𝒫(𝐑). Prove that 𝐷 is
surjective.

The notation 𝐷 is used above to remind you of the differentiation
map that sends a polynomial 𝑝 to 𝑝′

**Proof**:

Given a $p$ such that $\deg Dp = 0$, so $Dp = c \neq 0$.
Then $D \frac{1}{c} p = 1$.

Then we can also find $p$ such that $Dp = x$ and so on.

So $D$ is surjective.

$\square$

### 3B.29

Suppose 𝑝 ∈ 𝒫(𝐑). Prove that there exists a polynomial
𝑞 ∈ 𝒫(𝐑) such that 5𝑞″ + 3𝑞′ = 𝑝.
This exercise can be done without linear algebra, but it’s more fun
to do it using linear algebra.

**Proof**:

Note that $Dq = 5𝑞″ + 3𝑞'$ satisfies 3B.28. So $D$ is surjective.

$\square$

### 3B.30

Suppose 𝜑 ∈ ℒ(𝑉, 𝐅) and 𝜑 ≠ 0. Suppose 𝑢 ∈ 𝑉 is not in
null 𝜑. Prove that 𝑉 = null 𝜑 ⊕ {𝑎𝑢 ∶ 𝑎 ∈ 𝐅}.

**Proof**:

Assume $\varphi u = c \neq 0$.

Give $v \in V$ and $\varphi (v) = b$.

Then

$$
𝜑(v - \frac{b}{c}u) = 𝜑(v) - \frac{b}{c} 𝜑(u) = b - b = 0
$$

So $v - \frac{b}{c}u \in \text{null } 𝜑$.

Thus $𝑉 = \text{null } 𝜑 + \{𝑎𝑢 ∶ 𝑎 ∈ 𝐅\}.$

Assume $v \in \text{null } 𝜑 \cap \{𝑎𝑢 ∶ 𝑎 ∈ 𝐅\}$,

Then $0 = 𝜑(v) = 𝜑(au) = a 𝜑(u) = ac = 0$, so $a = 0 \cdot c^{-1} = 0$.

Then $v = 0$.

So $𝑉 = \text{null } 𝜑 ⊕ \{𝑎𝑢 ∶ 𝑎 ∈ 𝐅\}.$

$\square$

### 3B.31

Suppose 𝑉 is finite-dimensional, 𝑋 is a subspace of 𝑉 , and 𝑌 is
a finite-dimensional subspace of 𝑊. Prove that there exists
𝑇 ∈ ℒ(𝑉, 𝑊) such that
null 𝑇 = 𝑋 and range 𝑇 = 𝑌 if and only if dim 𝑋 + dim 𝑌 = dim 𝑉 .

**Proof**:

$\Rightarrow$

From 3.21 fundamental theorem of linear maps

$$
\dim V = \dim \text{null } T + \text{dim range } T
$$

Since $\text{null } T = X$ and $\text{range } T = Y$,
then

$$
\dim 𝑋 + \dim 𝑌 = \dim 𝑉
$$

$\Leftarrow$

Let $w_1, \cdots, w_m$ be a basis of $Y$.
$v_1, \cdots, v_n$ is a basis of $X$, and we can extend
it to a basis of $V$ by adding $m$ elements $u_1, \cdots, u_m$.

Define $T(v_i) = 0, T(u_j) = w_j$.

$\square$

### 3B.32

Suppose 𝑉 is finite-dimensional with dim 𝑉 > 1.
Show that if 𝜑 ∶ ℒ(𝑉) → 𝐅
is a linear map such that 𝜑(𝑆𝑇) = 𝜑(𝑆)𝜑(𝑇) for all
𝑆, 𝑇 ∈ ℒ(𝑉), then 𝜑 = 0.

Hint: The description of the two-sided ideals of ℒ(𝑉) given by
Exercise 17 in Section 3A might be useful.

**Proof**:

Consider the $\text{null } 𝜑$, for all $T \in ℒ(𝑉)$ and all
$E \in \text{null } \varphi$,

$$
𝜑(E𝑇) = 𝜑(E) 𝜑(T) = 0 𝜑(T) = 0 = 𝜑(T) 0 = 𝜑(T) 𝜑(E) = 𝜑(ET)
$$

So $ET \in \text{null } \varphi$ and $TE \in \text{null } \varphi$.

$\text{null } \varphi$ is a two-sided ideal.

Since 𝑉 is finite-dimensional with $\dim 𝑉 > 1$,
then $\dim ℒ(V) > 1$. Since the following 2 linear maps are
linearly independent.

$$
T_1(v_1) = v_1, T_1(v_2) = v_2 \\
T_2(v_1) = v_2, T_2(v_2) = v_1 \\
$$

Also note $\dim F = 1$.
So from 3.22 linear map to a lower-dimensional space is not injective
and 3.15 injectivity ⟺ null space equals {0}.

Then $\text{null } \varphi \neq \{0\}$, so
$\text{null } \varphi = ℒ(V)$, then 𝜑 = 0.

$\square$

### 3B.33

Suppose that 𝑉 and 𝑊 are real vector spaces and 𝑇 ∈ ℒ(𝑉, 𝑊).
Define $𝑇_𝐂 ∶ 𝑉_𝐂 → 𝑊_𝐂$ by

$$
𝑇_𝐂 (𝑢 + 𝑖𝑣) = 𝑇𝑢 + 𝑖𝑇𝑣
$$

for all 𝑢, 𝑣 ∈ 𝑉.

(a) Show that $𝑇_𝐂$ is a (complex) linear map from $𝑉_𝐂$ to $𝑊_𝐂$.

**Proof**:

$$
T_C((a + 𝑖b) + (c + di)) =
T_C ((a+c)+i(b+d)) \\
=
T(a+c) + iT(b+d) \\
= (T(a) + iT(b)) + (T(c) + iT(d)) \\
= T_C(a + 𝑖b) + T_C(c+id)
$$

Also

$$
T_C((x+iy)(a+ib)) = \\
T_C((ax-by) + i(xb + ya)) \\
= T(xa - yb) + i T(ya + xb) \\
= xTa - yT(b) + i yT(a) + i x T(b) \\
= (x+iy) (T(a) + iT(b)) \\
= (x+iy) T(a + ib) \\
$$

$\square$

(b) Show that $𝑇_𝐂$ is injective if and only if 𝑇 is injective.

**Proof**:

$\Rightarrow$

$𝑇_𝐂$ is injective

Assume $T(u) = 0$, then $T_C(u + ui) = 0$.

So $u + iu = 0$, so $u = 0$.

$\Leftarrow$

$T$ is injective.

Assume $T_C(u + iv) = 0$, then
$T(u) + i T(v) = 0$, so $T(u) = T(v) = 0$, then $u = v = 0$.

$\square$

(c) Show that range $𝑇_𝐂 = 𝑊_𝐂$ if and only if range 𝑇 = 𝑊.

**Proof**:

$\Rightarrow$

Given $w \in W$, since $T_C$ is surjective, then
we can find $T_C(a + ib) = w + 0i$, i.e.
$T(a) = w$.

$\Leftarrow$

Given $w = a + ib$, we can fine $T(u) = a, T(v) = b$,
then $T(u+iv) = a + ib$.

$\square$

## Section 3C Matrices

### 3C.1

Suppose 𝑇 ∈ ℒ(𝑉, 𝑊). Show that with respect to each choice of
bases of 𝑉 and 𝑊, the matrix of 𝑇 has at least dim range 𝑇 nonzero entries.

**Proof**:

Consider the matrix for $T$ is $A$.

Then let $k = \text{dim null } T, n = \text{dim range } T$,
then $k + n = \dim V$. If only $m < n$ entries are nonzero,
then it means the matrix has more than $k$ columns are $0$.

That means $\text{dim null } T > k$, we reach a contradition.

$\square$

###

### 3C.5

Suppose 𝑉 and 𝑊 are finite-dimensional and 𝑇 ∈ ℒ(𝑉, 𝑊). Prove
that there exist a basis of 𝑉 and a basis of 𝑊 such that with
respect to these bases, all entries of ℳ(𝑇) are 0 except that the
entries in row 𝑘, column 𝑘, equal 1 if 1 ≤ 𝑘 ≤ dim range 𝑇.

**Proof**:

Let $m = \text{dim range } T$, and $w_1, \cdots, w_m$ is a
basis of $\text{range } T$.

Assume $v_1, \cdots, v_m \in V$ such that
$Tv_1 = w_1, \cdots, Tv_m = w_m$.

Assume $p = n - m = \text{dim null } T$, then expand
$v_1, \cdots, v_m$ with $u_1, \cdots, u_p \in \text{null } T$.

With these 2 basis of $V$ and $W$, $ℳ(𝑇)$ is what we want.

$\square$

### 3C.6

Suppose $v_1, \cdots, v_m$ is a basis of 𝑉 and 𝑊 is
finite-dimensional. Suppose 𝑇 ∈ ℒ(𝑉, 𝑊). Prove that there exists
a basis $w_1, \cdots, w_n$ of 𝑊 such that all
entries in the first column of ℳ(𝑇) [with respect to the bases
$v_1, \cdots, v_m$ and $w_1, \cdots, w_n$] are $0$ except for
possibly a $1$ in the first row, first column.

In this exercise, unlike Exercise 5, you are given the basis of 𝑉
instead of being able to choose a basis of 𝑉 .

**Proof**:

Let $w_1 = T v_1$ and extend $w_1$ to a basis of $W$ by adding
$w_2, \cdots, w_m$.

Then $M(T)$ is desired matrix.

$\square$

### 3C.7

Suppose $w_1, \cdots, w_m$ is a basis of 𝑊 and 𝑉 is
finite-dimensional. Suppose 𝑇 ∈ ℒ(𝑉, 𝑊). Prove that there exists
a basis $v_1, \cdots, v_n$ of 𝑉 such that all
entries in the first row of ℳ(𝑇) [with respect to the bases
$v_1, \cdots, v_n$ and
$w_1, \cdots, w_m$] are 0 except for possibly a $1$ in the first
row, first column.

In this exercise, unlike Exercise 5, you are given the basis of 𝑊
instead of being able to choose a basis of 𝑊.

**Proof**:

Let $v_1, \cdots, v_n \in V$ is a basis of $V$. Assume the
matrix $\mathcal{M}(T) = [A_{i, j}]$. If $A_{1, .} = 0$, then
then $v_1, \cdots, v_m$ satisfies the requirement.

If $A_{1, .} \neq 0$, then $A_{1, j} \neq 0$ for some $j$.
We can swap $v_1$ and $v_j$. Then $A_{1, 1} \neq 0$.
Let $v_1' = \frac{1}{A_{1, 1}}v_1$, then $A_{1, 1} = 1$.

For any $v_j$ such that $A_{1, j} \neq 0$, let

$$
v_j' = v_j - A_{1, j}v_1'
$$

With $v'_1, \cdots, v'_n$, the first row of $\mathcal{M}(T)$,
$A_{1, .} = [1, 0, \cdot, 0]$, as required.

$\square$

### 3C.16

Suppose $𝐴$ is an $𝑚$-by-$𝑛$ matrix with $𝐴 ≠ 0$.
Prove that the rank of $𝐴$ is 1
if and only if there exist $(𝑐_1, …, 𝑐_𝑚) ∈ 𝐅^𝑚$ and $(𝑑_1, …, 𝑑_𝑛) ∈ 𝐅^𝑛$ such that
$A_{j, k} = 𝑐_𝑗 𝑑_𝑘$ for every $𝑗 = 1, …, 𝑚$ and every $𝑘 = 1, …, 𝑛$.

**Proof**:

$\Rightarrow$

From 3.56 column–row factorization, since the
rank of $A$ is $1$, we can find a $m$-by-$1$ matrix
$C$ and $1$-by-$n$ matrix $R$ such that $A = CR$.

Then $C$ and $R$ are what we need.

$\Leftarrow$

We have

$$
A =
\begin{pmatrix}
c_1 \\
\vdots \\
c_m
\end{pmatrix}
(𝑑_1, …, 𝑑_𝑛)
$$

So from 3.50 and 3.51, we have

$$
A_{., j} = C d_j
$$

That means the columns of $A$ are the scalar of
$C$. So $A$'s rank is 1.

$\square$

### 3C.17

Suppose $𝑇 ∈ ℒ(𝑉)$, and $u_1, \cdots, u_n$ and
$v_1, \cdots, v_n$ are bases of $𝑉$. Prove that
the following are equivalent.

(a) $𝑇$ is injective.

(b) The columns of $ℳ(𝑇)$ are linearly independent in
$𝐅^{𝑛, 1}$.

(c) The columns of $ℳ(𝑇)$ span $𝐅^{𝑛, 1}$.

(d) The rows of $ℳ(𝑇)$ span $𝐅^{𝑛, 1}$.

(e) The rows of $ℳ(𝑇)$ are linearly independent in
$𝐅^{𝑛, 1}$.

**Proof**:

Our strategy is to prove

$$
(a) \Leftrightarrow
(b) \\
(b) \Rightarrow
(c) \Rightarrow
(d) \Rightarrow
(e)
\\
(e) \Rightarrow
(d) \Rightarrow
(c) \Rightarrow
(b)
$$

$(a) \Leftrightarrow (b)$.

If $T$ is injective, then $\text{dim null } T = 0$.

Assume $A = \mathcal{M}(T)$, and there are $A b = 0$, where
$b = F^{n,1}$, i.e.

$$
0 = A_{., 1} b_1 + \cdots + A_{., n} b_n
$$

Then consider

$$
T(b_1 v_1 + \cdots + b_n v_n) = \\
b_1 Tv_1 + \cdots + b_n Tv_n = \\
(Tv_1, \cdots, Tv_m)
\begin{pmatrix}
b_1 \\
\vdots \\
b_n
\end{pmatrix} \\
= ((w_1, \cdots, w_n)A)b \\
= (w_1, \cdots, w_n) (Ab) \\
= (w_1, \cdots, w_n) \cdot 0 \\
= 0
$$

Then $b_1 v_1 + \cdots + b_n v_n \in \text{null } T$,
so $b_1 v_1 + \cdots + b_n v_n = 0$,
i.e. $b_1 = \cdots = b_n = 0$.

On the other hand, if

$$
b_1 v_1 + \cdots + b_n v_n \in \text{null } T
$$

Then

$$
0 = T(b_1 v_1 + \cdots + b_n v_n) = \\
b_1 Tv_1 + \cdots + b_n Tv_n = \\
(Tv_1, \cdots, Tv_m)
\begin{pmatrix}
b_1 \\
\vdots \\
b_n
\end{pmatrix} \\
= ((w_1, \cdots, w_n)A)b \\
= (w_1, \cdots, w_n) (Ab)
$$

Since $w_1, \cdots, w_n$ is linearly independent,
we have $Ab = 0$.

Since

$$
Ab = A_{., 1} b_1 + \cdots + A_{., n} b_n
$$

And $A_{., 1}, \cdots, A_{., n}$ are linearly independent,
we must have $b_1 = \cdots = b_n = 0$.

Then we have $\text{null } T = \{0\}$.

This completes the proof of $(a) \Leftrightarrow (b)$.

$(b) \Rightarrow (c)$

Since $A_{., 1}, \cdots, A_{., n}$ are linearly
independent, and $\dim F^{n,1} = n$, then
$A_{., 1}, \cdots, A_{., n}$ is a basis
of $F^{n,1}$, so it spans $F^{n,1}$.

$(c) \Rightarrow (d)$

Since $A_{., 1}, \cdots, A_{., n}$ spans
$F^{n,1}$, the column rank of $A$ is $n$.
Since the column rank of $A$ is $n$, the row rank
is also $n$. Then
$A_{1, .}, \cdots, A_{n, .}$ spans $F^{1,n}$.

$(d) \Rightarrow (e)$

$A_{1, .}, \cdots, A_{n, .}$ spans $F^{1,n}$,
and the dimension of $F^{1,n}$ is $n$,
then $A_{1, .}, \cdots, A_{n, .}$ is a basis of
$F^{1,n}$, then
$A_{1, .}, \cdots, A_{n, .}$
are linearly independent.

The reverse direction is similar.

$\square$

## Section 3D Invertibility and Isomorphisms

### 3D.1

Suppose 𝑇 ∈ ℒ(𝑉, 𝑊) is invertible. Show that $𝑇^{−1}$ is invertible and

$$
(𝑇^{−1})^{-1} = T
$$

**Proof**:

This is because

$$
𝑇^{−1} T = I \\
T 𝑇^{−1} = I \\
$$

So

$$
(𝑇^{−1})^{-1} = T
$$

$\square$

### 3D.2

Suppose 𝑇 ∈ ℒ(𝑈, 𝑉) and 𝑆 ∈ ℒ(𝑉, 𝑊) are both invertible
linear maps.
Prove that 𝑆𝑇 ∈ ℒ(𝑈, 𝑊) is invertible and that
$(𝑆𝑇)^{−1} = 𝑇^{−1}𝑆^{−1}$.

**Proof**:

This is because

$$
𝑇^{−1}𝑆^{−1} (ST) = I \\
(ST) 𝑇^{−1}𝑆^{−1} = I \\
$$

$\square$

### 3D.3

Suppose 𝑉 is finite-dimensional and 𝑇 ∈ ℒ(𝑉).
Prove that the following are equivalent.

(a) 𝑇 is invertible.

(b) $Tv_1, \cdots, Tv_n$ is a basis of 𝑉 for every
basis $v_1, \cdots, v_n$  of 𝑉 .

(c) $Tv_1, \cdots, Tv_n$ is a basis of 𝑉 for some
basis $v_1, \cdots, v_n$ of 𝑉 .

**Proof**:

Our order is

$$
(a) \Rightarrow (b) \Rightarrow (c)
\Rightarrow (a)
$$

$(a) \Rightarrow (b)$

If 𝑇 is invertible. Then $T$ is surjective.

Given any basis $v_1, \cdots, v_n$,
$Tv_1, \cdots, Tv_n$ spans $V$.
So $Tv_1, \cdots, Tv_n$ is a basis of $V$.

$(b) \Rightarrow (c)$ is obvious.

$(c) \Rightarrow (a)$

If $Tv_1, \cdots, Tv_n$ is a basis of 𝑉, then
$T$ is surjective, so $𝑇$ is invertible.

$\square$

### 3D.4

Suppose 𝑉 is finite-dimensional and dim 𝑉 > 1.
Prove that the set of
noninvertible linear maps from 𝑉 to itself is not a
subspace of ℒ(𝑉).

**Proof**:

Assume $\dim V = 2$. $v_1, v_2$ is a basis of $V$.

Let $T(v_1) = v_1, T(v_2) = 0, S(v_1) = 0, S(v_2) = v_2$.

Since $T, S$ are not injective, they are not invertible.

But $T_1 + T_2 = I$.

$\square$

### 3D.5

Suppose 𝑉 is finite-dimensional, 𝑈 is a subspace of 𝑉 , and
𝑆 ∈ ℒ(𝑈, 𝑉).
Prove that there exists an invertible linear map 𝑇 from 𝑉 to
itself such that 𝑇𝑢 = 𝑆𝑢 for every 𝑢 ∈ 𝑈 if and only if 𝑆 is
injective.

**Proof**:

$\Rightarrow$

If $Su = Tu = 0$, since $T$ is injective, then $u = 0$,
so $S$ is injective.

$\Leftarrow$

If $S$ is injective, and $u_1, \cdots, u_m$ is a basis of
$U$. We can extend it to a basis of $V$ by adding
$v_1, \cdots, v_n$.

Let $Tu_i = Su_i$. $Tu_i$ is linear independent since $S$ is
injective. Extend $Tu_i$ to a basis of $V$ by adding
$w_1, \cdots, w_n$, then let $Tv_i = w_i$.

Now assume $Tu = 0$, let

$$
u = a_1 u_1 + \cdots + a_m u_m +
b_1 v_1 + \cdots + b_n v_n
$$

Then

$$
0 = a_1 Tu_1 + \cdots + a_m Tu_m +
b_1 Tv_1 + \cdots + b_n Tv_n \\
\Rightarrow \\
a_1 = \cdots = a_m = b_1 = \cdots = b_n = 0
$$

So $u = 0$ and $T$ is invertible.

$\square$

### 3D.6

Suppose that 𝑊 is finite-dimensional and 𝑆, 𝑇 ∈ ℒ(𝑉, 𝑊).
Prove that null 𝑆 = null 𝑇 if and only if there exists an
invertible 𝐸 ∈ ℒ(𝑊) such that 𝑆 = 𝐸𝑇.

**Proof**:

$\Rightarrow$

Assume null 𝑆 = null 𝑇, let $u_1, \cdots, u_m$ be a basis
of $\text{null } T$.

Extend $u_1, \cdots, u_m$ with $v_1, \cdots, v_n$ so they
become a basis of $V$.

So $Tv_1, \cdots, Tv_n$ is basis of $\text{range } T$ since
$\text{dim range } T = (n+m)-m = n$.

For the same reason,
$Sv_1, \cdots, Sv_n$ is basis of $\text{range } S$

Let $ETv_i = Sv_i$.

$\square$

$\Leftarrow$

Assume $v \in \text{null } T$, then $S(v) = ET(v) = E(0) = 0$.
So $\text{null } T \subseteq \text{null } S$.

Assume $w in \text{null } S$, then $ET(w) = 0$, since
$E$ is injective, then $T(w) = 0$.
So $\text{null } S \subseteq \text{null } T$.

$\square$

### 3D.7

Suppose that 𝑉 is finite-dimensional and 𝑆, 𝑇 ∈ ℒ(𝑉, 𝑊).
Prove that range 𝑆 = range 𝑇 if and only if there exists an
invertible 𝐸 ∈ ℒ(𝑉) such that 𝑆 = 𝑇𝐸.

**Proof**:

$\Rightarrow$

Assume $w_1, \cdots, w_m$ is a basis of $\text{range } S$.

$Sv_1 = w_1, \cdots, Sv_m = w_m$ and
$Tu_1 = w_1, \cdots, Tu_m = w_m$.

Let $x_1, \cdots, x_n$ be a basis of $\text{null } S$.
Let $y_1, \cdots, y_n$ be a basis of $\text{null } T$.

$$
a_1 v_1 + \cdots + a_m v_m
+
b_1 x_1 + \cdots + b_n x_n = 0 \\
\Rightarrow \\
S(
a_1 v_1 + \cdots + a_m v_m
+
b_1 x_1 + \cdots + b_n x_n) = 0 \\
\Rightarrow \\
a_1 Sv_1 + \cdots + a_m Sv_m
+
b_1 Sx_1 + \cdots + b_n Sx_n = 0 \\
\Rightarrow \\
a_1 = \cdots = a_m = b_1 = \cdots = b_n = 0
$$

So $v_1, \cdots, v_m, x_1, \cdots, x_n$ is a basis of $V$.
Also
$u_1, \cdots, u_m, y_1, \cdots, y_n$ is a basis of $U$.

Let $Eu_i = v_i, Ey_j = x_j$.

$E$ is an isomorphism and $S = TE$.

$\Leftarrow$

$S = TE$, assume $w \in \text{range } T$ then $T(v) = w$.
Since $E$ is surjective, we can find $u$ such that
$E(u) = v$, then $S(u) = TE(u) = Tv = w$.

On the other hand,
assume $w in \text{range } S$, then $w = S(u) = TE(u) = T(E(u))$,
so $w \in \text{range } T$.

$\square$

### 3D.8

Suppose 𝑉 and 𝑊 are finite-dimensional and 𝑆, 𝑇 ∈ ℒ(𝑉, 𝑊).
Prove that there exist invertible $𝐸_1 ∈ ℒ(𝑉)$ and $𝐸_2 ∈ ℒ(𝑊)$
such that $𝑆 = 𝐸_2𝑇𝐸_1$ if and only if
$\text{dim null } T = \text{dim null } S$.

**Proof**:

$\Leftarrow$

If $\text{dim null } T = \text{dim null } S$, then
$\text{null } T$ and $\text{null } S$ are isomorphic.

Assume $E_1: \text{null } S \longrightarrow \text{null } T$
is an isomorphism and we can extend it to
$E_1: S \longrightarrow T$.

If $u \in \text{null } S
\Rightarrow
E_1(u) \in \text{null } T
\Rightarrow
T E_1(u) = 0$.

If $u \in \text{null } T E_1
\Rightarrow
E_1 u \in \text{null } T
\Rightarrow
u \in \text{null } S
$

Therefore $\text{null } TE_1 = \text{null } S$

Apply exercise 3D.6, we can have $E_2 \in \mathcal{L}(W)$,
such that $S = E_2 T E_1$.

$\Rightarrow$

Consider the subspace $E_1(\text{null } S)$.

Assume $u \in \text{null } S$, then
$E_2 T E_1 (u) = 0$, since $E_2$ is injective, $E_1u \in \text{null } T$.

So $E_1(\text{null } S) \subseteq \text{null } T$.

Assume $v \in \text{null } T$, $E_1$ is injective,
then we can find $u$, $E_1(u) = v$, then
$S(u) = E_2 T E_1 (u) = E_2 T v = 0$, i.e.
$\text{null } T \subseteq E_1(\text{null } S)$.

So $\text{null } T = \subseteq E_1(\text{null } S)$.
We have $\text{dim null } T = \text{dim null } S$ as required.

$\square$

### 3D.9

Suppose 𝑉 is finite-dimensional and 𝑇 ∶ 𝑉 → 𝑊 is a surjective
linear map of 𝑉 onto 𝑊. Prove that there is a subspace 𝑈 of 𝑉
such that $𝑇|_𝑈$ is an isomorphism of 𝑈 onto 𝑊.

**Proof**:

Let $w_1, \cdots, w_m$ be a basis of $W$.
And $v_1, \cdots, v_m$ such that
$Tv_1 = w_1, \cdots, Tv_m = w_m$.

$v_1, \cdots, v_m$ is independent.

Let $U = \text{span}(𝑣_1, \cdots, 𝑣_𝑚)$, $𝑇|_𝑈$ is
an isomorphism.

$\square$

### 3D.10

Suppose 𝑉 and 𝑊 are finite-dimensional and 𝑈 is a subspace of
𝑉. Let

$$
ℰ = \{ 𝑇 ∈ ℒ(𝑉, 𝑊) ∶ 𝑈 ⊆ null 𝑇 \}.
$$

Prove the following

(a) Show that ℰ is a subspace of ℒ(𝑉, 𝑊).

**Proof**:

If $T_1, T_2 \in ℰ$ and $u \in U$, then

$$
(T_1 + T_2)(u) = T_1(u) + T_2(u) = 0 + 0 = 0
$$

So $T_1 + T_2 \in ℰ$.

Same for $kT_1$.

$\square$

(b) Find a formula for dim ℰ in terms of dim 𝑉 , dim 𝑊, and dim 𝑈.

Hint: Define $Φ ∶ ℒ(𝑉, 𝑊) → ℒ(𝑈, 𝑊)$ by $Φ(𝑇) = 𝑇|_𝑈$.
What is null $Φ$? What is range $Φ$?

**Proof**:

If $T \in \text{null } Φ$, then $Φ(T) = T|_U = 0$, i.e.
for $u \in U, T(u) = 0$, then $U \subseteq \text{null } T$.
So $\text{null } Φ \subseteq ℰ$.

On the other hand, if $T \in ℰ$, then $Φ(T) = T|_U = 0$,
so $ℰ \subseteq \text{null } Φ$.

So $ℰ = \text{null } Φ$

$Φ$ is surjective because for any $S \in \mathcal{L}(U, W)$,
we can find $T$ such that $Φ(T) = T|_U = S$.

Then

$$
\dim \mathcal{L}(V, W) = \dim V \times \dim W \\
\text{dim range } Φ = \dim \mathcal{L}(U, W)
= \dim U \times \dim W \\
\dim ℰ = \text{dim null } Φ = (\dim V - \dim U) \times \dim W
$$

### 3D.11

Suppose 𝑉 is finite-dimensional and 𝑆, 𝑇 ∈ ℒ(𝑉). Prove that

$$
ST \text{ is invertible }
\Longleftrightarrow
\text{𝑆 and 𝑇 are invertible.}
$$

**Proof**:

$\Rightarrow$

$ST$ is invertible, then $ST$ is injective.
So if $v_1 \neq v_2$ then $STv_1 \neq STv_2$.
That means $Tv_1 \neq Tv_2$, so $T$ is injective, so
$T$ is invertible.

$ST$ is invertible, then $ST$ is surjective.
Given any $v$ we can find $u$, such that $STu - v$,
so $S(Tu) = v$. So $S$ is surjective, then it's invertible.

$\Leftarrow$

𝑆 and 𝑇 are invertible, then

$$
T^{-1}S^{-1} ST = 1 \\
ST T^{-1}S^{-1} = 1
$$

So $T^{-1}S^{-1}$ is the inverse of $ST$.

$\square$

### 3D.12

Suppose 𝑉 is finite-dimensional and 𝑆, 𝑇, 𝑈 ∈ ℒ(𝑉) and
𝑆𝑇𝑈 = 𝐼. Show that 𝑇 is invertible and that $𝑇^{−1} = 𝑈𝑆$.

**Proof**:

From 3.68, $STU = I$ then $TUS = I$. Then use 3.68 again
$(US)T = I$.

$\square$

### 3D.13

Show that the result in Exercise 12 can fail without the hypothesis
that 𝑉 is finite-dimensional.

**Solution**:

Consider $V = \mathbf{F}^{\infty }$, $S$ is the identity mapping.
And

$$
T: (x_1, x_2, x_3, \cdots) \longrightarrow (x_2, x_3, \cdots) \\
U: (x_1, x_2, x_3, \cdots) \longrightarrow (0, x_1, x_2, x_3, \cdots) \\
$$

We know from the second example of 3.64 that $T$ is not
invertible, but $TUS = I$.

$\square$

### 3D.14

Prove or give a counterexample: If 𝑉 is a finite-dimensional
vector space and 𝑅, 𝑆, 𝑇 ∈ ℒ(𝑉) are such that 𝑅𝑆𝑇 is
surjective, then 𝑆 is injective.

**Proof**:

$RST$ is surjective, then it's invertible.
From exercise 3D.11, $ST$ is invertible.
Again use 3D.11, $S$ is invertible, then $S$ is injective.

$\square$

### 3D.15

Suppose 𝑇 ∈ ℒ(𝑉) and $v_1, \cdots, v_m$ is a list in 𝑉 such that
$𝑇𝑣_1, …, 𝑇𝑣_𝑚$ spans 𝑉 .
Prove that $𝑣_1, …, 𝑣_𝑚$ spans 𝑉 .

**Proof**:

Since $𝑇𝑣_1, …, 𝑇𝑣_𝑚$ spans $V$, then $V$ is finite dimension.
So $T$ is surjective means $T$ is invertible.
Let $v \in V, S = T^{-1}$, and assume

$$
Tv = a_1 Tv_1 + \cdots + a_m Tv_m \\\
\Rightarrow \\
STv = S(a_1 Tv_1 + \cdots + a_m Tv_m) \\
\Rightarrow \\
v = a_1 STv_1 + \cdots + a_m STv_m \\
\Rightarrow  (\text{$ST$ is identity operator and $S$ is linear})  \\
v = a_1 v_1 + \cdots + a_m v_m
$$

$\square$

### 3D.16

Prove that every linear map from $\mathbf{F}^{n, 1}$ to
$\mathbf{F}^{m, 1}$ is given by a matrix
multiplication. In other words, prove that if
$𝑇 ∈ ℒ(\mathbf{F}^{n, 1}, \mathbf{F}^{m, 1})$,
then there exists an
𝑚-by-𝑛 matrix 𝐴 such that $𝑇𝑥 = 𝐴𝑥$ for every
$𝑥 ∈ \mathbf{F}^{n, 1}$.

**Proof**:

Given $𝑇 ∈ ℒ(\mathbf{F}^{n, 1}, \mathbf{F}^{m, 1})$,
consider

$$
A = \mathcal{M}(T, (e_1, \cdots, e_n), (e_1, \cdots, e_m))
$$

Then

$$
T(x) = T(x_1 e_1 + \cdots + x_n e_n) \\
= x_1 Te_1 + \cdots + x_n Te_n \\
= x_1 A_{.,1} + \cdots + x_n A_{.,n} \\
= Ax
$$

The 2nd $=$ is because $T$ is linear.
The 3rd $=$ is from the definitions of $ℳ(𝑇)$.
The last equality is from 3.50.

$\square$

### 3D.17

Suppose 𝑉 is finite-dimensional and 𝑆 ∈ ℒ(𝑉).
Define 𝒜 ∈ ℒ(ℒ(𝑉)) by

$$
𝒜(𝑇) = 𝑆𝑇
$$

for 𝑇 ∈ ℒ(𝑉).

(a) Show that
$\text{dim null } 𝒜 = (\dim 𝑉)(\text{dim null } 𝑆)$.

**Proof**:

Consider this subspace of $ℒ(ℒ(𝑉))$:

$$
T : V \rightarrow \text{null } S
$$

It's the $\text{null } 𝒜$. And its dimension is
$(\dim 𝑉)(\text{dim null } 𝑆)$.

(b) Show that
$\text{dim range } 𝒜 = (\dim 𝑉)(\text{dim range } 𝑆)$.

**Proof**:

Note $𝒜$ is a linear map from $ℒ(𝑉) \rightarrow ℒ(𝑉)$, so

$$
\text{dim range } 𝒜 + \text{dim null } 𝒜 = \dim ℒ(𝑉) =
\dim 𝑉 \times \dim 𝑉
$$

Then

$$
\text{dim range } 𝒜 = \dim 𝑉 \times \dim 𝑉 -
(\dim 𝑉)(\text{dim null } 𝑆) = (\dim 𝑉)(\text{dim range } 𝑆)
$$

as required.

$\square$

### 3D.18

Show that 𝑉 and ℒ(𝐅, 𝑉) are isomorphic vector spaces.

**Proof**:

Given $v \in V$, define this map from
$T: 𝑉 \longrightarrow ℒ(𝐅, 𝑉), T(v) = S_v, S_v(1) = v$.

We first show $T$ is injective.

If $T(v) = 0$, then $v = S_v(1) = 0(1) = 0$. So $T$ is surjective.

Next we show $T$ is surjective.

Assume $S \in ℒ(𝐅, 𝑉)$ and $S(1) = v$, then given any
$a \in 𝐅$,

$$
S(a) = S (a \cdot 1) = a S(1) = a v = a S_v(1) = S_v(a) \\
\Rightarrow \\
S = S_v = T(v)
$$

So $T$ is surjective.

In summary, $T$ is an isomorphism.

$\square$

### 3D.19

Suppose 𝑉 is finite-dimensional and 𝑇 ∈ ℒ(𝑉). Prove that 𝑇 has
the same matrix with respect to every basis of 𝑉 if and only if 𝑇
is a scalar multiple of the identity operator.

**Proof**:

$\Rightarrow$

We first consider when $\dim V = 2$ and consider 2 basis:
$v_1, v_2$ and $v_2, v_1$. Assume this same matrix
is

$$
A =
\begin{bmatrix}
a & b \\
c & d \\
\end{bmatrix}
$$

From 3.84 change-of-basis formula

$$
𝐶 = ℳ(𝐼, (v_1, v_2), (v_2, v_1)) \\
=
\begin{bmatrix}
0 & 1 \\
1 & 0 \\
\end{bmatrix}
$$

Then we have

$$
C A = A C \\
\begin{bmatrix}
c & d \\
a & b \\
\end{bmatrix} =
\begin{bmatrix}
b & a \\
d & c \\
\end{bmatrix}
$$

So we must have $a = d, b = c$.
Then

$$
A =
\begin{bmatrix}
a & b \\
b & a \\
\end{bmatrix}
$$

Then we consider

$$
𝐶 = ℳ(𝐼, (v_1 + v_2, v_2), (v_1, v_2)) \\
=
\begin{bmatrix}
1 & 0 \\
1 & 1 \\
\end{bmatrix}
$$

Then we have

$$
C A = A C \\
\begin{bmatrix}
a & b \\
a+b & a+b \\
\end{bmatrix} =
\begin{bmatrix}
a+b & b \\
a+b & a \\
\end{bmatrix}
$$

So we must have $b = 0$, then

$$
A =
\begin{bmatrix}
a & 0 \\
0 & a \\
\end{bmatrix}
$$

We next consider when $\dim V = 3$ Assume this same matrix is:

$$
A =
\begin{bmatrix}
a & b & c \\
d & e & f \\
g & h & i \\
\end{bmatrix}
$$

and consider 2 basis:
$v_1, v_2, v_3$ and $v_2, v_1, v_3$.

$$
C =
\begin{bmatrix}
0 & 1 & 0 \\
1 & 0 & 0 \\
0 & 0 & 1 \\
\end{bmatrix}
$$

Then

$$
CA = AC \\
\begin{bmatrix}
d & e & f \\
a & b & c \\
g & h & i \\
\end{bmatrix}
=
\begin{bmatrix}
b & a & c \\
e & d & f \\
h & g & i \\
\end{bmatrix}
$$

So we have $a = e, d = b, c = f, g = h$

$$
A =
\begin{bmatrix}
a & b & c \\
b & a & c \\
g & g & i \\
\end{bmatrix}
$$

Next consider
$v_1, v_2, v_3$ and $v_3, v_2, v_1$.

$$
C =
\begin{bmatrix}
0 & 0 & 1 \\
0 & 1 & 0 \\
1 & 0 & 0 \\
\end{bmatrix}
$$

$$
CA = AC \\
\begin{bmatrix}
g & g & i \\
b & a & c \\
a & b & c \\
\end{bmatrix}
=
\begin{bmatrix}
c & b & a \\
c & a & b \\
i & g & g \\
\end{bmatrix}
$$

Then we have $a = i, b = c = g$.

$$
A =
\begin{bmatrix}
a & b & b \\
b & a & b \\
b & b & a \\
\end{bmatrix}
$$

Next consider $v_1+v_2, v_2, v_3$ and $v_1, v_2, v_3$.

$$
C =
\begin{bmatrix}
1 & 0 & 0 \\
1 & 1 & 0 \\
0 & 0 & 1 \\
\end{bmatrix}
$$

$$
CA = AC \\
\begin{bmatrix}
a   & b   & b \\
b+a & a+b & b+b \\
b & b & a \\
\end{bmatrix} =
\begin{bmatrix}
a+b & b & b \\
b+a & a & b \\
b+b & b & a \\
\end{bmatrix}
$$

Then $b = 0$.

We have

$$
A =
\begin{bmatrix}
a & 0 & 0 \\
0 & a & 0 \\
0 & 0 & a \\
\end{bmatrix}
$$

For other dimensions, it's similar.
So, we finished one direction.

$\Leftarrow$

Now assume if 𝑇
is a scalar multiple of the identity operator.
Then $T(v) = av$, so $\mathcal{M}(T) = a I$.
as required.

$\square$

### 3D.20

Suppose 𝑞 ∈ 𝒫(𝐑). Prove that there exists a polynomial
𝑝 ∈ 𝒫(𝐑) such that

$$
𝑞(𝑥) = (𝑥^2 + 𝑥)𝑝''(𝑥) + 2𝑥𝑝'(𝑥) + 𝑝(3)
$$

for all 𝑥 ∈ 𝐑.

**Proof**:

First note if $p(x) = ax+b$, then $q(x) = 2ax + 3a + b \neq 0$.
Then $ax+b \not\in \text{null } T$

Assume $p(x) = a x^n + b x^{n-1} + r(x), r(x) \in
𝒫_{n-2}(𝐑), p(x) \in \text{null } T
$, then $n > 1$.

Then we have

$$
p'(x) = an x^{n-1} + b(n-1) x^{n-2} + r'(x)\\
p''(x) = an(n-1) x^{n-2} + b(n-1)(n-2) x^{n-3} + r''(x) \\
2x p'(x) = 2 an x^n + 2b (n-1) x^{n-1} \\
(x^2 + x) p''(x) = an(n-1) x^n + b(n-1)(n-2)x^{n-1}
+ an(n-1) x^{n-1} + b(n-1)(n-2)x^{n-2}
$$

So we have

$$
2an + an(n-1) = 0 \Rightarrow \\
an(n+1) = 0 \\
\Rightarrow \\
a = 0
2b (n-1) + b(n-1)(n-2) + an(n-1) = 0 \\
\Rightarrow \\
bn(n-1) = 0 \\
\Rightarrow \\
b = 0
$$

Then we have a contradition. So $\text{null } T = \{0\}$.

Then $T$ is surjective, we can find $p$ for $q$.

$\square$

### 3D.21

Suppose 𝑛 is a positive integer and $A_{j, k} ∈ 𝐅$ for all
$𝑗, 𝑘 = 1, …, 𝑛$. Prove that
the following are equivalent (note that in both parts below, the
number of equations equals the number of variables).

(a) The trivial solution
$𝑥_1 = ⋯ = 𝑥_𝑛 = 0$ is the only solution to the
homogeneous system of equations

$$
\sum_{k=1}^{n} A_{1, k} x_k = 0 \\
\vdots \\
\sum_{k=1}^{n} A_{n, k} x_k = 0. \\
$$

And

(b) For every $𝑐_1, …, 𝑐_𝑛 ∈ 𝐅$, there exists a solution to the system of equations

$$
\sum_{k=1}^{n} A_{1, k} x_k = c_1 \\
\vdots \\
\sum_{k=1}^{n} A_{n, k} x_k = c_n. \\
$$

**Proof**:

We can have 2 perspectives.

(i) Let $A = [A_{j, k}]$ then view $A$ as a liner map from
$\mathbb{F}^{n,1}$ to $\mathbb{F}^{n,1}$ by mapping $x$ to $Ax$.

Then (a) says $A$ is injective and (b) says $A$ is surjective.
So they are equivalent.

(ii) We can treat $A_{., k}$ as a vector in $\mathbb{F}^{n,1}$.

Then (a) says $A_{., k}$ are independent and (b) says
$A_{., k}$ spans the $\mathbb{F}^{n,1}$. From the fundamental
theorem of linear mapping, they are equivalent.

$\square$

### 3D.22

Suppose 𝑇 ∈ ℒ(𝑉) and $𝑣_1, …, 𝑣_𝑛$ is a basis of 𝑉.
Prove that

$$
ℳ(𝑇, (𝑣_1, …, 𝑣_𝑛)) \text{ is invertible}
\Longleftrightarrow
T \text{ is invertible}
$$

**Proof**:

$\Rightarrow$

Let $A = ℳ(𝑇, (𝑣_1, …, 𝑣_𝑛))$ and $B$ be its inverse matrix.
Let $S$ be the linear map that $B = ℳ(S, (𝑣_1, …, 𝑣_𝑛))$.

Then

$$
ℳ(𝑇S, (𝑣_1, …, 𝑣_𝑛)) = ℳ(𝑇, (𝑣_1, …, 𝑣_𝑛))ℳ(S, (𝑣_1, …, 𝑣_𝑛)) = AB = I
$$

Then $TS = I$, from 3.68, we have $ST = I$.

$\Leftarrow$

Assume $TS = ST = I$, then

$$
ℳ(𝑇, (𝑣_1, …, 𝑣_𝑛))ℳ(S, (𝑣_1, …, 𝑣_𝑛)) =\\
ℳ(𝑇S, (𝑣_1, …, 𝑣_𝑛)) = \\
ℳ(I, (𝑣_1, …, 𝑣_𝑛)) = I
$$

$\square$

### 3D.23

Suppose that $u_1, \cdots, u_n$  and $𝑣_1, …, 𝑣_𝑛$ are bases of
$𝑉$. Let 𝑇 ∈ ℒ(𝑉) be such that
$𝑇𝑣_𝑘 = 𝑢_𝑘$ for each $𝑘 = 1, …, 𝑛$. Prove that

$$
ℳ(𝑇, (𝑣_1, …, 𝑣_𝑛)) = ℳ(𝐼, (𝑢_1, …, 𝑢_𝑛), (𝑣_1, …, 𝑣_𝑛))
$$

**Proof**:

Since $𝑇𝑣_𝑘 = 𝑢_𝑘$, so

$$
ℳ(T, (v_1, …, v_𝑛), (u_1, …, u_𝑛)) = I
$$

Then from

$$
ℳ(T, (v_1, …, v_𝑛), (u_1, …, u_𝑛))
ℳ(I, (u_1, …, u_𝑛), (v_1, …, v_𝑛)) =\\
ℳ(T, (𝑣_1, …, 𝑣_𝑛))
$$

So we proved.

$\square$

### 3D.24

Suppose 𝐴 and 𝐵 are square matrices of the same size and
𝐴𝐵 = 𝐼. Prove that 𝐵𝐴 = 𝐼.

**Proof**:

Let $A, B$ are $n$ by $n$ square matrices.
Each of them induces a linear map from $\mathbb{F}^{n,1}$ to
$\mathbb{F}^{n,1}$, say they are $T, S$. And their matrices
w.r.t the standard basis $(e_1, …, e_n)$ are $A, B$.

Since $AB = I$, then $TS = I$. From 3.68, we have $ST = I$.

From 3.81,

$$
ℳ(𝑆𝑇, (e_1, …, e_n), (e_1, …, e_n)) = \\
ℳ(𝑆, (e_1, …, e_𝑛), (e_1, …, e_n))ℳ(𝑇, (e_1, …, e_n), (e_1, …, e_𝑛)).
$$

i.e.

$$
ℳ(I, (e_1, …, e_n)) = \\
ℳ(𝑆, (e_1, …, e_𝑛))ℳ(𝑇, (e_1, …, e_n)).
$$

Then we have $I = BA$ as required.

$\square$

## Section 3E Products and Quotients of Vector Spaces

### 3E.2

Suppose that $V_1, \cdots, V_m$ are vector spaces such that
$𝑉_1 × ⋯ × 𝑉_𝑚$ is finite-dimensional.
Prove that $𝑉_𝑘$ is finite-dimensional for each
$𝑘 = 1, …, 𝑚$.

**Proof**:

Since $𝑉_1 × ⋯ × 𝑉_𝑚$ is finite-dimensional, then assume it
can be spanned by $n$ vectors.

Take the 1st component from these $n$ vectors and they can span
$V_1$. So $V_1$ is finite-dimensional.

$\square$

### 3E.3

Suppose $𝑉_1, …, 𝑉_𝑚$ are vector spaces.
Prove that $ℒ(𝑉_1 × ⋯ × 𝑉_𝑚, 𝑊)$ and
$ℒ(𝑉_1, 𝑊) × ⋯ × ℒ(𝑉_𝑚, 𝑊)$ are isomorphic vector spaces.

**Proof**:

Assume

$$ 
T \in ℒ(𝑉_1 × ⋯ × 𝑉_𝑚, 𝑊)
$$

Let

$$ 
\tau_1 : T \longrightarrow T_1
$$

Let $T_1$ be a mapping, such that

$$ 
T_1(v) = T((v, 0, \cdots, 0))
$$

It's easy to see, $T_1 \in ℒ(𝑉_1, 𝑊)$.

Then we can have this mapping

$$ 
\tau: T \longrightarrow (\tau_1(T), \cdots, \tau_n(T)) = (T_1, \cdots, T_m)
$$

To see it's injective, assume

$T_1 = \cdots = T_m = 0$, then

$$ 
T((v_1, \cdots, v_m)) = T((v_1, \cdots, 0)) + \cdots
+ T((0, \cdots, v_m)) = T_1 v_1 + \cdots + T_m v_m = 0 \\
\Rightarrow \\
T = 0
$$

To see it's surjective, given
$(T_1, \cdots, T_m)$, and let

$$ 
T((v_1, \cdots, v_m)) = T_1 v_1 + \cdots + T_m v_m
$$

It's easy to see $T$ is a linear map.

We also have

$$ 
\tau_1(T)(v_1) = T(v_1, \cdots, 0) = T_1 v_1 \\
\Rightarrow \\
\tau_1(T) = T_1
$$

so $\tau$ is surjective.

Then $T$ is an isomorphism.

$\square$

### 3E.4

Suppose $𝑊_1, …, 𝑊_𝑚$ are vector spaces.
Prove that $ℒ(𝑉, 𝑊_1 × ⋯ × 𝑊_𝑚)$ and
$ℒ(𝑉, 𝑊_1) × ⋯ × ℒ(𝑉, 𝑊_𝑚)$ are isomorphic vector spaces.

**Proof**:

Given $T \in ℒ(𝑉, 𝑊_1 × ⋯ × 𝑊_𝑚)$, let
$\tau_1 : T \longrightarrow T_1 \in ℒ(𝑉, 𝑊_1)$.

$$
T(v) = (\tau_1(T)(v), \cdots, \tau_m(T)(v))
$$

$$ 
\tau(T) = (\tau_1(T)(v), \cdots, \tau_m(T)(v))
$$

$\square$

### 3E.5

Suppose that $𝑣, 𝑥$ are vectors in $𝑉$ and that $𝑈, 𝑊$ are subspaces of 
$𝑉$ such that $𝑣 + 𝑈 = 𝑥 + 𝑊$. Prove that $𝑈 = 𝑊$.

**Proof**:

Since $U, W$ are subspaces, then $0 \in U, W$.
So $v \in x + W, x \in v + U$. Then we can assume

$$ 
v = x + w_0 \\
x = v + u_0
$$

Then given $u \in U$, we have $v + u = x + w_1$, i.e.

$$ 
(x + w_0) + u = x + w_1 \\
\Rightarrow \\
u = w_1 - w_0 \in W \\
\Rightarrow \\
U \subseteq W
$$

For the same reason, $W \subseteq U$, i.e. $U = W$.

$\square$

### 3E.9

Prove that a nonempty subset 𝐴 of 𝑉 is a translate of some subspace of 𝑉 if
and only if 𝜆𝑣 + (1 − 𝜆)𝑤 ∈ 𝐴 for all 𝑣, 𝑤 ∈ 𝐴 and all 𝜆 ∈ 𝐅.

**Proof**:

$\Rightarrow$

Assume $A = u + U$ where $U$ is a subspace of $V$. And if $𝑣, 𝑤 ∈ 𝐴$,
then

$$ 
v = u + u_0 \\
w = u + u_1 \\
$$

Then we have

$$ 
\lambda 𝑣 + (1 − \lambda )𝑤 = \lambda  (u + u_0) + (1 - \lambda ) (u + u_1)
= u + (\lambda u_0 + (1 - \lambda) u_1) \in A
$$

$\Leftarrow$

We will prove $-v + A$ is a subspace.

If $a, b \in -v + A$.

$$ 
a = -v + 𝑣_a \\
b = -v + 𝑣_b \\
a + b = -v + (v_a + v_b - v)
= -v + 2(\frac{1}{2}v_a + \frac{1}{2}v_b) - v
$$

Note $w = \frac{1}{2}v_a + \frac{1}{2}v_b \in A$, then $2w - v \in A$.
So $a + b \in -v + A$.

Similarly,

$$ 
ka = k (-v + v_a) = -v + k v_a - (k-1)v \in -v + A
$$

$\square$

### 3E.10

Suppose $𝐴_1 = 𝑣 + 𝑈_1$ and $𝐴_2 = 𝑤 + 𝑈_2$ for some $𝑣, 𝑤 ∈ 𝑉$ and some
subspaces $𝑈_1, 𝑈_2$ of $𝑉$. Prove that the intersection $𝐴_1 ∩ 𝐴_2$ is either a
translate of some subspace of 𝑉 or is the empty set.

**Proof**:

Assume $𝐴_1 ∩ 𝐴_2 \neq \emptyset, a \in 𝐴_1 ∩ 𝐴_2$.

Let $A = 𝐴_1 ∩ 𝐴_2, U = -a + A$.

Assume $v_1, v_2 \in U$, then
$v_1 = -a + a_1, v_2 = -a + a_2, a_1 \in A, a_2 \in A$.

We will show $v_1 + v_2 \in U$.

$$ 
v_1 = -a + v + u_1 = -(v + u_0) + v + u_1 \\
v_2 = -a + v + u_2 = -(v + u_0) + v + u_2 \\
\Rightarrow \\
v_1 + v_2 = u_1 + u_2 - 2 u_0 = - (v + u_0) + (v + u_0) + (u_1 + u_2 - 2 u_0) \\
= -a + v + (u_1 + u_2 - u_0) \\
\Rightarrow \\
v_1 + v_2 + a = v + (u_1 + u_2 - u_0) \in A_1
$$

For the same reason, $v_1 + v_2 + a \in A_2$.
Then $v_1 + v_2 + a \in 𝐴_1 ∩ 𝐴_2$, i.e. $v_1 + v_2 \in -a + A$.

Now consider $k v_1 = -k a + k a_1 = k (-(v + u_0) + v + u_1) = k (u_1 - u0)$.

$$ 
a + k (u_1 - u0) = v + u_0 + k(u_1 - u0) \in A_1
$$

So $k v_1 \in U$.

Then $U$ is a subspace.

$\square$

### 3E.11

Suppose $𝑈 = \{(𝑥_1, 𝑥_2, … ) ∈ 𝐅^∞ ∶ 𝑥_𝑘 ≠ 0
\text{ for only finitely many } 𝑘\}$.

(a) Show that $𝑈$ is a subspace of $𝐅^∞$

**Proof**:

Assume $a, b \in U$, then assume for all $n > N_a, a_n = 0$
and $n > N_b, b_n = 0$.

Then $a+b$ has only finite non-zero items. So $a+b \in U$.

Similarly, $ka \in U$.

$\square$

(b) Prove that $𝐅^∞ /𝑈$ is infinite-dimensional.

**Proof**:

We prove by contradition. Assume it's finite-dimensional, and the
dimension is $N$, all we need to do is to find $N+1$ independent vectors
in $𝐅^∞ /𝑈$.

Consider the following group of vectors

$$ 
v_{1,i} =\begin{cases}
    1 &\text{ if } i = k(N+1)+1, k = 0, 1, 2, \cdots \\
    0 &\text{ otherwise}\\
\end{cases} \\
v_{2,i} =\begin{cases}
    1 &\text{ if } i = k(N+1)+2, k = 0, 1, 2, \cdots \\
    0 &\text{ otherwise}\\
\end{cases} \\
v_{N+1,i} =\begin{cases}
    1 &\text{ if } i = k(N+1)+(N+1), k = 0, 1, 2, \cdots \\
    0 &\text{ otherwise}\\
\end{cases} \\
$$

Any linear combination of them cannot have finite non-zero items.

Anything example is

$$ 
v_{1,i} =\begin{cases}
    1 &\text{ if } p | 2 \\
    0 &\text{ otherwise}\\
\end{cases} \\
v_{2,i} =\begin{cases}
    1 &\text{ if } p | 3 \\
    0 &\text{ otherwise}\\
\end{cases} \\
\cdots 
$$

$\square$

### 3E.12

Suppose $𝑣_1, …, 𝑣_𝑚 ∈ 𝑉$ . Let

$$
A = \{
\lambda_1 v_1 + \cdots + \lambda_m v_m
:
\lambda_1, \cdots, \lambda_m \in F
\text{ and }
\lambda_1 + \cdots + \lambda_m = 1
\}
$$

(a) Prove that $𝐴$ is a translate of some subspace of $𝑉$.

**Proof**:

We will prove $-v_1 + A$ is a subspace.

$$ 
(-v_1 + a) + (-v_1 + a') = \\
(-v_1 + \lambda_1 v_1 + \cdots + \lambda_m v_m) +
(-v_1 + \lambda'_1 v_1 + \cdots + \lambda'_m v_m) \\
= -v_1 + (\lambda_1 + \lambda'_1 - 1) v_1 + \cdots + (\lambda_m + \lambda'_m) v_m
$$

Note that

$$ 
(\lambda_1 + \lambda'_1 - 1) + \cdots + (\lambda_m + \lambda'_m) = 1
$$

So $(-v_1 + a) + (-v_1 + a') \in -v_1 + A$.

Next

$$ 
k(-v_1 + a) = k (-v_1 + \lambda_1 v_1 + \cdots + \lambda_m v_m) \\
= -v_1 + ((1-k)v_1 + k\lambda_1 v_1 + \cdots + k\lambda_m v_m)
$$

Note that

$$ 
(1-k) + k\lambda_1 + \cdots + k\lambda_m = (1-k) + k = 1
$$

So $k(-v_1 + a) \in -v_1 + A$, then $-v_1 + A$ is a subspace.

$\square$

(b) Prove that if $𝐵$ is a translate of some subspace of $𝑉$ and
$\{𝑣_1, …, 𝑣_𝑚\} ⊆ 𝐵$, then $𝐴 ⊆ 𝐵$.

**Proof**:

Assume $B = u + U$ and $U$ is a subspace. Then $v_i - u \in U$ and

$$ 
\lambda_1 (v_1-u) + \cdots + \lambda_m (v_m-u) \\
=
(\lambda_1 v_1 + \cdots + \lambda_m v_m)
- (\lambda_1 + \cdots + \lambda_m) u \\
= 
(\lambda_1 v_1 + \cdots + \lambda_m v_m) - u \in U
$$

Then $\lambda_1 v_1 + \cdots + \lambda_m v_m \in B$. So $𝐴 ⊆ 𝐵$.

$\square$

(c) Prove that $𝐴$ is a translate of some subspace of $𝑉$ of dimension less
than $𝑚$.

**Proof**:

Now consider the space spanned by $v_2-v_1, \cdots , v_m - v_1$ and call it
$U$.

For any $u \in U, u = \lambda_2 (v_2-v_1) + \cdots + \lambda_m (v_m-v_1)$,

Consider $v_1 + u = v_1 + \lambda_2 (v_2-v_1) + \cdots + \lambda_m (v_m-v_1)$,
then

$$ 
v_1 + u = (1 - \lambda_2 - \cdots - \lambda_m) v_1 +
\lambda_2 v_2 + \cdots + \lambda_m v_m \in A
$$

So $v_1 + U \subseteq A$.

On the other hand, for any $\lambda_1 v_1 + \cdots + \lambda_m v_m \in A$,
we have

$$ 
\lambda_1 v_1 + \cdots + \lambda_m v_m \\
= v_1 + \lambda_2 (v_2-v_1) + \cdots + \lambda_m (v_m-v_1)
$$

So $A \subseteq v_1+ U$, i.e. $A = v_1 + U$.

Since $U = \text{span}(𝑣_2-v_1, \cdots, 𝑣_𝑚-v_1)$, $\dim U < m$.

$\square$

### 3E.13

Suppose $𝑈$ is a subspace of $𝑉$ such that $𝑉/𝑈$ is finite-dimensional. 
Prove that $𝑉$ is isomorphic to $𝑈 × (𝑉/𝑈)$.

**Proof**:

Given $v \in V$, and $w_1+U, \cdots, w_m+U$ is a basis of $V/U$.
Assume $v+U = a_1 (w_1+U) + \cdots + a_m (w_m+U)$, and let
$u = v - (a_1 w_1 + \cdots + a_m w_m) \in U$. We have a map:

$$ 
T: v \rightarrow (u, v + U)
$$

It's easy to verify it's linear.

injective: if $T(v) = 0 = (0, 0 + U)$, then $u = 0 + 0 = 0$.

surjective: Given $(u, v+U)$, Then $T(v+u) = (u, v+U)$.

So $T$ is an isomorphism.

$\square$

### 3E.14

Suppose $𝑈$ and $𝑊$ are subspaces of $𝑉$ and $𝑉 = 𝑈 ⊕ 𝑊$.
Suppose $𝑤_1, …, 𝑤_𝑚$
is a basis of $𝑊$. Prove that $𝑤_1 + 𝑈, …, 𝑤_𝑚 + 𝑈$ is
a basis of $𝑉/𝑈$.

**Proof**:

Assume $v \in V$, and $v = u + w, u \in U, w \in W$.
Then $v + U = w+U$, because $v-w \in U$.
Then $v+U = a_1 (w_1+U) + \cdots + a_m (w_m+U)$. So $𝑤_1 + 𝑈, …, 𝑤_𝑚 + 𝑈$
spans $V/U$.

Now if $a_1 (w_1+U) + \cdots + a_m (w_m+U) = 0 + U$, then
$$
a_1 w_1 + \cdots + a_m w_m \in U \\
a_1 w_1 + \cdots + a_m w_m \in W \\
$$

Since $U \cap W = 0$, then $a_1 w_1 + \cdots + a_m w_m = 0$,
then $a_1 = \cdots = a_m = 0$.

So $𝑤_1 + 𝑈, …, 𝑤_𝑚 + 𝑈$ is a basis of $𝑉/𝑈$.

$\square$

### 3E.15

Suppose $𝑈$ is a subspace of $𝑉$ and $𝑣_1 + 𝑈, …, 𝑣_𝑚 + 𝑈$ is a basis of
$𝑉/𝑈$ and $𝑢_1, …, 𝑢_𝑛$ is a basis of $𝑈$. Prove that
$𝑣_1, …, 𝑣_𝑚, 𝑢_1, …, 𝑢_𝑛$ is a basis of $𝑉$.

**Proof**:

Given $w \in V$, then $w+U \in V/U$, then

$$ 
w+U = a_1 (v_1+U) + \cdots + a_m (v_m+U)
$$

So

$$ 
w - (a_1 v_1 + \cdots + a_m v_m) \in U \\
\Rightarrow \\
w - (a_1 v_1 + \cdots + a_m v_m) = b_1 u_1 + \cdots + b_n u_n
$$

Then $𝑣_1, …, 𝑣_𝑚, 𝑢_1, …, 𝑢_𝑛$ spans $V$.

Assume

$$ 
a_1 v_1 + \cdots + a_m v_m +
b_1 u_1 + \cdots + b_n u_n = 0
$$

Then $a_1 v_1 + \cdots + a_m v_m \in U$, then

$$ 
(a_1 v_1 + \cdots + a_m v_m) + U = \\
a_1 (v_1+U) + \cdots + a_m (v_m+U) = 0 + U \\
\Rightarrow \\
a_1 = \cdots = a_m = 0
$$

Then we have $b_1 = \cdots = b_n = 0$.

Then $𝑣_1, …, 𝑣_𝑚, 𝑢_1, …, 𝑢_𝑛$ are independent.

$\square$

### 3E.16

Suppose $𝜑 ∈ ℒ(𝑉, 𝐅)$ and $𝜑 ≠ 0$. Prove that

$$
\dim V / \text{null } \varphi = 1
$$ 

**Proof**:

Assume $u, v \not\in \text{null } \varphi$.

Then $\varphi (u) \neq 0, \varphi (v) \neq 0$.

Then we can find $k \neq 0$ such that
$\varphi (u) = k \varphi (v)$, so
$\varphi (u - kv) = 0$.

Then $u - kv \in \text{null } \varphi$.

Then we have $u + \text{null } \varphi = kv + \text{null } \varphi = k (v + \text{null } \varphi)$.

Since $u$ is arbitary, then any $u + \text{null } \varphi$
can be represented
by a scalar of $v + \text{null } \varphi$.

So

$$ 
\dim V / \text{null } \varphi = 1
$$

$\square$

### 3E.17

Suppose $𝑈$ is a subspace of $𝑉$ such that $\dim 𝑉/𝑈 = 1$.
Prove that there exists
$𝜑 ∈ ℒ(𝑉, 𝐅)$ such that $\text{null } \varphi = 𝑈$.

**Proof**:

Since $\dim V/U = 1$, let $v + U$ be a basis of $V/U$.

For any $w \in V$, we have $w + U = k(v+U)$. Then $\mathcal{M}(w) = k$.

Then we can consider $\varphi = \mathcal{M} \circ \pi$.

If $w \in \text{null } \varphi$, then $\mathcal{M}(\pi(w)) = 0$,
so $\pi(w) = 0 + U$, i.e. $w \in U$. So $\text{null } \varphi = U$.

$\square$

### 3E.18

Suppose that $𝑈$ is a subspace of $𝑉$ such that $𝑉/𝑈$ is 
finite-dimensional.

(a) Show that if $𝑊$ is a finite-dimensional subspace of $𝑉$ and
$𝑉 = 𝑈 + 𝑊$, then $\dim 𝑊 ≥ \dim 𝑉/𝑈$.

**Proof**:

All we need to prove is that the basis $w_1+U, \cdots, w_m+U$ of $W$ spans
$V/U$.

Assume $v \in V$, we can write $v = u + w = u + (a_1 w_1 + \cdots + a_m w_m)$.
Then $v - w \in U$, so $v + U = w + U$.

So $w_1+U, \cdots, w_m+U$ of $W$ spans $V/U$. Then $\dim 𝑊 ≥ \dim 𝑉/𝑈$.

$\square$

(b) Prove that there exists a finite-dimensional subspace $𝑊$ of $𝑉$ such 
that $\dim 𝑊 = \dim 𝑉/𝑈$ and $𝑉 = 𝑈 ⊕ 𝑊$.

**Proof**:

Let $w_1+U, \cdots, w_m+U$ be a basis of $V/U$, then
consider the $W = \text{span}(w_1, \cdots, w_𝑚)$.

If $u \in U$ and $u = a_1 w_1 + \cdots + a_m w_m$, then
$a_1 w_1 + \cdots + a_m w_m \in U$, then

$$ 
a_1 (w_1+U) + \cdots + a_m (w_m+U) = 0 + U
$$

So $a_1 = \cdots = a_m = 0$, then $u = 0$.

So $U + W = 𝑈 ⊕ 𝑊$.

If $v \in V$, then $v + U = a_1 (w_1+U) + \cdots + a_m (w_m+U)$.
Then $v - (a_1 w_1 + \cdots + a_m w_m) \in U$.

So $V = U + W$.

Combine these 2 parts, we have $V = 𝑈 ⊕ 𝑊$.

$\square$

### 3E.19

Suppose $𝑇 ∈ ℒ(𝑉, 𝑊)$ and $𝑈$ is a subspace of $𝑉$.
Let $𝜋$ denote the quotient
map from $𝑉$ onto $𝑉/𝑈$. Prove that there exists $𝑆 ∈ ℒ(𝑉/𝑈, 𝑊)$
such that
$𝑇 = 𝑆 ∘ 𝜋$ if and only if $𝑈 ⊆ \text{null } 𝑇$.

**Proof**:

$\Rightarrow$

Assume $u \in U$, then $\pi (u) = 0 + U$, so $S(\pi (u)) = 0$.

So $𝑈 ⊆ \text{null } 𝑇$.

$\Leftarrow$

If $v \in V$, then let $S(v + U) = T(v)$.

It's well defined, because if $v_1 + U = v_2 + U$, then

$$ 
S((v_1+U)-(v_2+U)) = S((v_1-v_2)+U) = T(v_1-v_2) = 0 \\
\Rightarrow (\because v_1-v_2 \in U \And U \subseteq \text{null } T) \\
S(v_1 + U) = S(v_2 + U)
$$

Next, we show it's linear.

$$ 
S((v_1+U)+(v_2+U)) = S((v_1+v_2) + U) = T(v_1+v_2) = T(v_1) + T(v_2) \\
= S(v_1+U) + S(v_2+U) \\
S(k(v_1+U)) = S(k v_1 + U) = T(k v_1) = k T(v_1) = k S(v_1 + U)
$$

$\square$

## Section 3F Duality

### 3F.1

Explain why each linear functional is surjective or is the zero map.

**Proof**:

Assume $\varphi \in V'$, if $\varphi(v) = c \neq 0$.

Then for any $d \in F$

$$ 
\varphi ((d/c) v) = (d/c) \varphi(v) = d/c \cdot c = d
$$

So $\varphi$ is surjective.

$\square$

### 3F.2

Give three distinct examples of linear functionals on $𝐑^{[0, 1]}$.

**Proof**:

$f(0), f(1), f(1/2)$

$\square$

### 3F.3

Suppose $𝑉$ is finite-dimensional and $𝑣 ∈ 𝑉$ with $𝑣 ≠ 0$.
Prove that there exists $\varphi ∈ 𝑉'$ such that $\varphi(𝑣) = 1$.

**Proof**:

Extend $v$ to a basis of $V$, then its dual basis satisfies $\varphi(𝑣) = 1$.

$\square$

### 3F.4

Suppose $𝑉$ is finite-dimensional and $𝑈$ is a subspace of $𝑉$ such that
$𝑈 ≠ 𝑉$.
Prove that there exists $\varphi ∈ 𝑉'$ such that $\varphi(𝑢) = 0$ for
every $𝑢 ∈ 𝑈$ but $\varphi ≠ 0$.

**Proof**:

$$ 
\dim U^0 = \dim V - \dim U > 0
$$

So $U^0 \neq 0$, then pick any $\varphi \in U^0$.

$\square$

### 3F.5

Suppose 𝑇 ∈ ℒ(𝑉, 𝑊) and $𝑤_1, …, 𝑤_𝑚$ is a basis of range $𝑇$. Hence 
for each $𝑣 ∈ 𝑉$ , there exist unique numbers
$\varphi_1(𝑣), …, \varphi_𝑚(𝑣)$ such that 

$$ 
Tv = \varphi_1(v) w_1 + \cdots + \varphi_m(v) w_m
$$

thus defining functions $\varphi_1, …, \varphi_𝑚$ from 𝑉 to 𝐅. Show that 
each of the functions $\varphi_1, …, \varphi_𝑚$ is a linear functional on 
$𝑉$.

**Proof**:

Let $\psi_1, \cdots, \psi_m$ be the dual basis of $𝑤_1, …, 𝑤_𝑚$.
Then 

$$ 
T'(\psi_i)(v) = \psi_i(T(v)) = \varphi_i(v) \psi_i(w_i) = \varphi_i(v)
$$

So $T'(\psi_i) = \varphi_i$, which is a linear functional on $V$.

$\square$

### 3F.6

Suppose 𝜑, 𝛽 ∈ 𝑉′ . Prove that null 𝜑 ⊆ null 𝛽 if and only if there exists
𝑐 ∈ 𝐅 such that 𝛽 = 𝑐𝜑.

**Proof**:

$\Leftarrow$

Assume $v \in \text{null } \varphi$, then

$$ 
\beta (v) = c \varphi (v) = c 0 = 0
$$

So $\text{null } \varphi \subseteq \text{null } \beta$

$\Rightarrow$

If $\beta = 0$, then $c = 0$ can satisfy $\beta = c \varphi$.

If $\beta \neq 0$, then
$\text{null } \varphi \subseteq \text{null } \beta \subset V$,

we can find $u \in V$ such that $\varphi (u) \neq 0$.

Then $V = \text{null } \varphi \oplus \text{span}(u)$.

If $\beta (u) = 0$, then $\text{null } \beta = V$, we have a contradition.

So $\beta (u) \neq 0$. Then let $c = \beta (u) / \varphi (u)$.

$\square$

### 3F.7

Suppose that $V_1, \cdots, V_m$ are vector spaces. Prove that
$(𝑉_1 × ⋯ × 𝑉_𝑚)'$ and
$𝑉_1' × ⋯ × 𝑉_𝑚'$ are isomorphic vector spaces.

**Proof**:

Note $V_i' = \mathcal{L}(V_i, R)$, then we just need to apply
exercise 3E.3 by replacing $W$ with $R$.

$\square$

### 3F.8

Suppose $𝑣_1, …, 𝑣_𝑛$ is a basis of 𝑉 and $\varphi_1, …, \varphi_𝑛$ is 
the dual basis of $𝑉'$. Define $\Gamma ∶ 𝑉 → 𝐅^𝑛$ and
$Λ ∶ 𝐅^𝑛 → 𝑉$ by

$$ 
\Gamma(𝑣) = (\varphi_1(𝑣), …, \varphi_𝑛(𝑣)),
\Delta(a_1, \cdots, a_n) = a_1 v_1 + \cdots + a_n v_n.
$$

Explain why $\Gamma$ and $\Delta$ are inverses of each other.

**Proof**:

First, we need to prove $\Gamma (\Delta (a_1, \cdots, a_n)) = (a_1, \cdots, a_n)$.

$$ 
\Gamma (\Delta (a_1, \cdots, a_n)) =\\
\Gamma (a_1 v_1 + \cdots + a_n v_n) = \\
(\varphi_1(a_1 v_1 + \cdots + a_n v_n), \cdots, 
\varphi (a_1 v_1 + \cdots + a_n v_n)) = \\
(a_1, \cdots, a_n)
$$

Secondly, we need to prove $\Delta(\Gamma(v)) = v$

$$ 
\Delta(\Gamma(v)) = \Delta(\varphi_1(𝑣), …, \varphi_𝑛(𝑣)) \\
= \varphi_1(v) v_1 + \cdots + \varphi_n(v) v_n \\
= v
$$

The last equation is from 3.114.

$\square$

### 3F.9

Suppose $𝑚$ is a positive integer. Show that the dual basis of the basis
$1, 𝑥, …, 𝑥_𝑚$ of $𝒫_𝑚(𝐑)$ is $\varphi_0, \varphi_1, …, \varphi_𝑚$, 
where

$$ 
\varphi_k(p) = \frac{p^{(k)}(0)}{k!}
$$

**Proof**:

$$ 
\varphi_k(x^{j}) =
\begin{cases}
    0 &\text{ if } k > j \\
    1 &\text{ if } k = j \\
    x^{j-k} = 0 &\text{ if } k < j \\
\end{cases} 
$$

$\square$

### 3F.10

Suppose $𝑚$ is a positive integer.

(a) Show that $1, 𝑥 − 5, …, (𝑥 − 5)^𝑚$ is a basis of $𝒫_{m}(\mathbf{R})$.

**Proof**:

$$ 
a_0 \cdot 1 + a_1 \cdot (x-5) + \cdots + a_m \cdot (x-5)^m = 0 \\
\Rightarrow \\
a_m = 0 \\
\Rightarrow \\
a_{m-1} = 0 \\
\Rightarrow \\
\cdots \\
\Rightarrow \\
a_0 = 0
$$

$\square$

(b) What is the dual basis of the basis in (a)?

**Solution**:

$$ 
\varphi_k(p) = \frac{p^{(k)}(5)}{k!}
$$

$\square$

### 3F.11

Suppose $𝑣_1, …, 𝑣_𝑛$ is a basis of $𝑉$ and $\varphi_1, …, \varphi_𝑛$ is 
the corresponding dual basis of $𝑉'$ . Suppose $\psi ∈ 𝑉'$. Prove that

$$
\psi = \psi(𝑣_1)\varphi_1 +⋯ + \psi(𝑣_𝑛)\varphi_𝑛.
$$

**Proof**:

For all $j$,

$$ 
(\psi(𝑣_1)\varphi_1 +⋯ + \psi(𝑣_𝑛)\varphi_𝑛)(v_j) \\
\psi(𝑣_1)\varphi_1(v_j) +⋯ + \psi(𝑣_𝑛)\varphi_𝑛(v_j) \\
= \psi(v_j) \varphi (v_j) = \psi (v_j)
$$

So

$$ 
\psi = \psi(𝑣_1)\varphi_1 +⋯ + \psi(𝑣_𝑛)\varphi_𝑛.
$$

$\square$

### 3F.12

Suppose $𝑆, 𝑇 ∈ ℒ(𝑉, 𝑊)$. 

(a) Prove that $(𝑆 + 𝑇)' = 𝑆' + 𝑇'$

**Proof**:

Assume $\varphi \in W'$ and $v \in V$.

$$ 
\begin{align*}
(𝑆 + 𝑇)'(\varphi)(v)
&= (\varphi \circ (S+T))(v) & \text{ (definition of dual mapping) } \\
&= \varphi((S+T)(v)) & \text{ (definition of composition) } \\
&= \varphi (S(v) + T(v))
& \text{ (the definition of addition of linear maps in } L(V, W)) \\
&= \varphi (S(v)) + \varphi (T(v)) 
& \varphi \text{ is linear map of  } W'\\
&= (S'(\varphi)) (v) + (T'(\varphi)) (v) 
& \text{ (definition of dual mapping) } \\
&= (S'(\varphi) + T'(\varphi)) (v)
& \text{ the definition of addition of linear maps in } V'\\
&= ((S' + T')(\varphi)) (v)
& \text{ the definition of addition of linear maps in } ℒ(W', V') \\
\end{align*}
$$

So $(𝑆 + 𝑇)' = 𝑆' + 𝑇'$.

$\square$

(b) Prove that $(\lambda 𝑇)' = \lambda 𝑇'$ for all $𝜆 ∈ 𝐅$.

**Proof**:

Assume $\varphi \in W'$ and $v \in V$.

$$ 
\begin{align*}
((\lambda 𝑇)'(\varphi))(v)
&= (\varphi \circ (\lambda 𝑇))(v)
& \text{ (definition of dual mapping) } \\
&= \varphi ((\lambda 𝑇)(v))
& \text{ (definition of composition)} \\
&= \varphi (\lambda 𝑇(v))
& \text{ definition of scalar multiplication in } L(V, W)\\
&= \lambda (\varphi(T(v)))
& \varphi \text{ is a linear map in } W' \\
&= \lambda ((T'(\varphi))(v))
& \text{ (definition of dual mapping) } \\
&= (\lambda T'(\varphi))(v)
& \text{ definition of scalar multiplication in V'} \\
&= ((\lambda T')(\varphi))(v)
& \text{ definition of scalar multiplication in } ℒ(W', V') \\
\end{align*} 
$$

$$
\begin{align*}
\end{align*} 
$$

So $(\lambda 𝑇)' = \lambda 𝑇'$

$\square$

### 3F.13

Show that the dual map of the identity operator on $𝑉$ is the identity operator
on $𝑉'$.

**Proof**:

Let $i$ be the identity operator, and $\varphi$ be a linear map in $V'$.

$i'(\varphi) = \varphi \circ i = \varphi$.

So $i'$ is the identity operator on $𝑉'$.

$\square$

### 3F.14

Define $𝑇 ∶ 𝐑^3 → 𝐑^2$ by

$$ 
𝑇(𝑥, 𝑦, 𝑧) = (4𝑥 + 5𝑦 + 6𝑧, 7𝑥 + 8𝑦 + 9𝑧).
$$

Suppose $\varphi_1, \varphi_2$ denotes the dual basis of the standard basis of 
$𝐑^2$ and $\psi_1, \psi_2, \psi_3$ denotes the dual basis of the standard basis of $𝐑^3$

(a) Describe the linear functionals $𝑇'(\varphi_1)$ and $𝑇'(\varphi_2)$.

**Solution**:

$$ 
T'(\varphi_1) = \varphi_1 \circ T = 4x+5y+6z \\
T'(\varphi_2) = \varphi_2 \circ T = 7x+8y+9z \\
$$

$\square$

(b) Write $𝑇'(\varphi_1)$ and $𝑇'(\varphi_2)$ as linear combinations
$\psi_1, \psi_2, \psi_3$.

**Solution**:

$$ 
T'(\varphi_1) = \varphi_1 \circ T = 4x+5y+6z = 4\psi_1+5\psi_2+6\psi_3 \\
T'(\varphi_2) = \varphi_2 \circ T = 7x+8y+9z = 7\psi_1+8\psi_2+9\psi_3 \\
$$

$\square$

### 3F.15

Define $𝑇 ∶ 𝒫(𝐑) → 𝒫(𝐑)$ by

$$ 
(𝑇𝑝)(𝑥) = 𝑥^2𝑝(𝑥) + 𝑝''(𝑥)
$$

for each $𝑥 ∈ 𝐑$.

(a) Suppose $\varphi ∈ 𝒫(𝐑)'$ is defined by $\varphi(𝑝) = 𝑝'(4)$.
Describe the linear functional $𝑇' (\varphi)$ on $𝒫(𝐑)$.

**Solution**:

$$ 
(𝑇' (\varphi))(p(x)) = (\varphi \circ T)(p(x)) \\
= \varphi (T(p(x))) \\
= \varphi (𝑥^2p(𝑥) + p''(𝑥)) \\
= x^2 p'(x) + 2x p(x) + p'''(x) |_4 \\
= 16 p'(4) + 8 p(4) + p'''(4)
$$

$\square$

(b) Suppose $\varphi ∈ 𝒫(𝐑)'$ is defined by
$\varphi(𝑝) = \int_{0}^{1} 𝑝$. Evaluate $(𝑇'(\varphi))(𝑥^3)$.

**Solution**:

$$
(𝑇' (\varphi))(x^3) = (\varphi \circ T)(x^3) \\
= \varphi (T(x^3)) \\
= \varphi (x^5 + 6x) \\
= \frac{1}{6} x^6 + 3x^2 \bigg|_0^1 \\
= 3 \frac{1}{6}
$$

$\square$

### 3F.16

Suppose $𝑊$ is finite-dimensional and $𝑇 ∈ ℒ(𝑉, 𝑊)$. Prove that

$$ 
T'=0 \Longleftrightarrow T = 0
$$

**Proof**:

Assume $w_1, \cdots, w_m$ is a basis of $W$,
$\varphi_1, \cdots, \varphi_m$ is the dual basis in $W'$, then

$\Rightarrow$

$$ 
\begin{align*}
T(v)
&= \varphi_1(T(v)) w_1 + \cdots + \varphi_m(T(v)) w_m 
&\text{ (3.114) } \\
&= T'(\varphi_1)(v) w_1 + \cdots + T'(\varphi_m)(v) w_m
&\text{ (3.118 definition: dual map) } \\
&= 0
&(T' = 0) \\
\end{align*} 
$$

$\Leftarrow$

$$ 
\begin{align*}
T'(\varphi ) (v)
&= \varphi (T(0))
&\text{ (3.118 definition: dual map) } \\
&=0
&(T=0) \\
&\Rightarrow T'(\varphi ) = 0 \text{ for any } \varphi \\
&\Rightarrow T' = 0
\end{align*} 
$$

Another way to prove

$$ 
\begin{align*}
T' = 0
& \Longleftrightarrow
\text{null } T' = W' \\
& \Longleftrightarrow
\text{dim range } T' = 0
&\text{ (3.21 fundamental theorem of linear maps) } \\
& \Longleftrightarrow
\text{dim range } T = 0
&\text{ (3.130 (a)) } \\
& \Longleftrightarrow
\text{dim null } T = \dim V
&\text{ (3.21 fundamental theorem of linear maps) } \\
& \Longleftrightarrow
\text{null } T = V \\
& \Longleftrightarrow
T = 0 \\
\end{align*} 
$$

$\square$

### 3F.17

Suppose 𝑉 and 𝑊 are finite-dimensional and 𝑇 ∈ ℒ(𝑉, 𝑊).
Prove that 𝑇 is invertible if and only if 𝑇′ ∈ ℒ(𝑊′, 𝑉′) is invertible.

**Proof**:

$\Rightarrow$

Since $T$ is invertible, we can find $S \in \mathcal{L}(W, V)$ such that $ST = I, TS = I$.

$$
\begin{align*}
I
&= I' &\text{ (ex. 3F.13) } \\
&= (ST)' \\
&= T' S'
&\text{ (3.120 algebraic properties of dual maps) }
\end{align*} 
$$

For the same reason $S'T' = I$. So $T'$ is invertible.

$\Leftarrow$

We can use a different way: $T'$ is invertible then, $W', V'$ are the same dimension, so are the $W, V$.

$$
\begin{align*}
T' \text{ is invertible }
&\Rightarrow T' \text{ is injective }
&\text{ (3.63) } \\
&\Rightarrow T \text{ is surjective }
&\text{ (3.129) } \\
&\Rightarrow T \text{ is invertible }
&(\text{ 3.65 and } \dim W = \dim V) \\
\end{align*} 
$$

$\square$

### 3F.18

Suppose 𝑉 and 𝑊 are finite-dimensional. Prove that the map that takes
𝑇 ∈ ℒ(𝑉, 𝑊) to 𝑇′ ∈ ℒ(𝑊′ , 𝑉′) is an isomorphism of ℒ(𝑉, 𝑊) onto ℒ(𝑊′ , 𝑉′).

**Proof**:

Since $𝑉$ and $𝑊$ are finite-dimensional, we just need to prove this map is injective is enough.
From exercise 3F.16, it's indeed the case.

$\square$

### 3F.19

Suppose $𝑈 ⊆ 𝑉$. Explain why

$$ 
U^0 =  \{\varphi ∈ 𝑉' ∶ 𝑈 ⊆ \text{null } \varphi \}.
$$

**Proof**:

Let $W = \{\varphi ∈ 𝑉' ∶ 𝑈 ⊆ \text{null } \varphi \}$.

If $\varphi \in W$, then for $u \in U$, $\varphi (u) = 0$, so
$\varphi \in U^0$. So $W \subseteq U^0$.

If $\varphi \in U^0$, then for $u \in U$, $\varphi (u) = 0$, so
$U \subseteq \text{null } \varphi$. So $\varphi \in W$. So
$U^0 \subseteq W$.

In summary $U^0 = W$.

$\square$

### 3F.20

Suppose $𝑉$ is finite-dimensional and $𝑈$ is a subspace of $𝑉$. Show that

$$ 
𝑈 = \{𝑣 ∈ 𝑉 ∶ \varphi(𝑣) = 0 \text{ for every } \varphi ∈ 𝑈^0\}.
$$

**Proof**

Let $W = \{𝑣 ∈ 𝑉 ∶ \varphi(𝑣) = 0 \text{ for every } \varphi ∈ 𝑈^0\}$.

$\Rightarrow$

If $u \in U$, then for every $\varphi \in U^0$, $\varphi(u) = 0$.
So $u \in W$, i.e. $U \subseteq W$.

$\Leftarrow$

Let $\dim U = m, \dim V = n$. $u_1, \cdots, u_m$ be a basis of $U$.

For $w \in W$, we consider $U' = \text{span}(u_1, \cdots, u_𝑚, w)$.

Given $\varphi \in U^0$, and any $u' \in U'$, $\varphi (u') = 0$, so
$U^0 \subseteq U'^0$.

Then $\dim U' = \dim V - \dim U'^0 \leq \dim V - \dim U^0 = \dim U$.

So $U = U'$, then $w \in U$, so $W \subseteq U$.

In summary, $U = W$.

$\square$

### 3F.21

Suppose $𝑉$ is finite-dimensional and $𝑈$ and $𝑊$ are subspaces of $𝑉$.

(a) Prove that $𝑊^0 ⊆ 𝑈^0$ if and only if $𝑈 ⊆ 𝑊$.

**Proof**:

$\Rightarrow$

Assume $u \in U$, and give any $\varphi \in W^0$, since $\varphi \in U^0$,
then $\varphi (u) = 0$. Then from ex 3F.20, we have $u \in W$.

$\Leftarrow$

Given $\varphi \in W^0$, and any $u \in U$, since $u \in W$,
$\varphi (u) = 0$, so $\varphi \in U^0$.
So $𝑊^0 ⊆ 𝑈^0$.

$\square$

### 3F.22

Suppose $𝑉$ is finite-dimensional and $𝑈$ and $𝑊$ are subspaces of $𝑉$.

(a) Show that $(𝑈 + 𝑊)^0 = 𝑈^0 ∩ 𝑊^0$.

**Proof**:

$\subseteq$

if $\psi \in (U+W)^0$, then given $u \in U$ then $u \in U+W$, so
$\psi (u) = 0$. Then $\psi \in U^0$. Similarly, $\psi \in W^0$.
So $\psi \in 𝑈^0 ∩ 𝑊^0$. Then $(𝑈 + 𝑊)^0 \subseteq 𝑈^0 ∩ 𝑊^0$.

$\supseteq$

If $\psi \in 𝑈^0 ∩ 𝑊^0$, then $\psi \in U^0$ and $\psi \in W^0$.
Given $u+w \in U+W$

$$ 
\begin{align*}
\psi (u+w)
&= \psi (u) + \psi (w) \\
&= 0+0 \\
&= 0 \\
&\Rightarrow
\psi \in (U+W)^0 \\
&\Rightarrow
(𝑈 + 𝑊)^0 \supseteq 𝑈^0 ∩ 𝑊^0
\end{align*} 
$$

$\square$

### 3F.23

Suppose $𝑉$ is finite-dimensional and $\varphi_1, …, \varphi_𝑚 ∈ 𝑉'$ . 
Prove that the following three sets are equal to each other.

(a) $\text{span}(\varphi_1, \cdots, \varphi_𝑚)$ 

(b) $((\text{null } \varphi_1) \cap \cdots \cap (\text{null } \varphi_m))^0$ 

(c) $\{\varphi \in V' : (\text{null } \varphi_1) \cap \cdots \cap
(\text{null } \varphi_m) \subseteq \text{null } \varphi\}$ 

**Proof**:

The equivalence of $(b)$ and $(c)$ is the result from ex 3F.19.

From ex 3F.22 (b)

$$ 
\begin{align*}
((\text{null } \varphi_1) \cap \cdots \cap (\text{null } \varphi_m))^0
&= (\text{null } \varphi_1)^0 + \cdots + (\text{null } \varphi_m)^0
\end{align*} 
$$

$\varphi_i \in (\text{null } \varphi_i)^0$

$$
\begin{align*}
\text{dim} (\text{null } \varphi_i )^0
&= \dim V - \text{dim null } \varphi_i \\
&= \dim V - (\dim V - \text{dim range } \varphi_i) \\
&= \dim V - (\dim V - 1) \\
&= 1 \\
&\Rightarrow
\text{span}(\varphi_i) = (\text{null } \varphi_i)^0 \\
&\Rightarrow
(\text{null } \varphi_1)^0 + \cdots + (\text{null } \varphi_m)^0
=
\text{span}(\varphi_1, \cdots, \varphi_𝑚)
\end{align*} 
$$

So we proved (a) and (b) are equivalent.

$\square$

### 3F.24

Suppose $𝑉$ is finite-dimensional and $𝑣_1, …, 𝑣_𝑚 ∈ 𝑉$.
Define a linear map

$$ 
\Gamma ∶ 𝑉' → 𝐅^𝑚 \text{ by } \Gamma(\varphi) =
(\varphi(𝑣_1), …, \varphi(𝑣_𝑚)).
$$

(a) Prove that $𝑣_1, …, 𝑣_𝑚$ spans $𝑉$ if and only if $\Gamma$ is 
injective.

**Proof**:

$\Rightarrow$

If $\Gamma (\varphi) = 0$, then

$$ 
\varphi(𝑣_1) = … = \varphi(𝑣_𝑚) = 0
$$

Then $\varphi (v) = 0$, so $\varphi = 0$.

Then $\Gamma$ is injective.

$\Leftarrow$

If $\Gamma$ is injective, and let $U = \text{span}(𝑣_1, \cdots, 𝑣_𝑚)$.
If $\varphi \in U^0$, then
$\Gamma(\varphi)=(\varphi(𝑣_1), …, \varphi(𝑣_𝑚)) = 0$.

Then $\varphi = 0$, that means $U^0 = \{0\}$, i.e. $U = V$.

$\square$

(b) Prove that $𝑣_1, …, 𝑣_𝑚$ is linearly independent if and only if 
$\Gamma$ is surjective.

**Proof**:

$\Rightarrow$

Let $\varphi_1, \cdots, \varphi_m$ be the dual basis, then
$\Gamma (\varphi_i) = e_i$ which is a standard basis of $𝐅^𝑚$.
So $\Gamma$ is surjective.

$\Leftarrow$

Since $\Gamma$ is surjective, let $\varphi_i$ be the mapping such that
$\Gamma (\varphi_i) = e_i$, so $\varphi_i(v_i) = 1, \varphi_i(v_j) = 0$.

Let

$$
\begin{align*}
0 = a_1 v_1 + \cdots + a_m v_m
& \Rightarrow
\varphi_i (a_1 v_1 + \cdots + a_m v_m) = 0 \\
& \Rightarrow
a_i \varphi_i (v_i) = 0 \\
& \Rightarrow
a_i = 0
\end{align*} 
$$

So $𝑣_1, …, 𝑣_𝑚$ is linearly independent. 

$\square$

Now we try a different approach. First, we consider the following isomorphism
from $F^n \rightarrow (F^n)'$ 

$$ 
i : (x_1, \cdots, x_m) \rightarrow x_1 \psi_1 + \cdots + x_m \psi_m
$$

Where $\psi_i$ is the dual basis of the standard basis $e_i$.

Let $\Gamma' = i \circ \Gamma$, so $\Gamma' \in (F^n)'$ 

Also consider $\gamma$ from $F^n \mapsto V$

$$ 
\gamma : (x_1, \cdots, x_m) \rightarrow x_1 v_1 + \cdots + x_m v_m
$$

Let $\varphi \in V'$, then

$$
\begin{align*}
(\varphi \circ \gamma) (x_1, \cdots, x_m)
&= x_1 \varphi(v_1) + \cdots + x_m \varphi(v_m)
\end{align*} 
$$

On the other hand,

$$
\begin{align*}
\Gamma'(\varphi)(x_1, \cdots, x_m)
&= (\varphi(v_1) \psi_1 + \cdots +  \varphi(v_m) \psi_m)
(x_1, \cdots, x_m) \\
&= x_1 \varphi(v_1) + \cdots + x_m \varphi(v_m)
\end{align*} 
$$

This shows $\Gamma'$ is dual map of $\gamma$.

Now coming back the problem.

$$
\begin{align*}
\text{span}(𝑣_1, \cdots, 𝑣_𝑚) = V
&\Longleftrightarrow
\gamma \text{ is surjective} \\
&\Longleftrightarrow
\Gamma' \text{ is injective}
&\text{ (3.131) } \\
&\Longleftrightarrow
\Gamma \text{ is injective}
\end{align*} 
$$

Also

$$
\begin{align*}
𝑣_1, …, 𝑣_𝑚 \text{ is linearly independent }
&\Longleftrightarrow
\gamma \text{ is injective} \\
&\Longleftrightarrow
\Gamma' \text{ is surjective}
&\text{ (3.129) } \\
&\Longleftrightarrow
\Gamma \text{ is surjective}
\end{align*} 
$$

$\square$

### 3F.25

Suppose $𝑉$ is finite-dimensional and $\varphi_1, …, \varphi_𝑚 ∈ 𝑉'$. 
Define a linear map

$\Gamma ∶ 𝑉 → 𝐅^𝑚$ by $\Gamma(𝑣) = (\varphi_1(𝑣), …, \varphi_𝑚(𝑣))$.

(a) Prove that $\varphi_1, …, \varphi_𝑚$
spans $𝑉'$ if and only if $Γ$ is injective.

**Proof**:

$\Rightarrow$

Consider $\text{null } \Gamma$, note $\varphi_i \in (\text{null } \Gamma )^0$,
so $(\text{null } \Gamma )^0 = V'$, then from $\text{null } \Gamma = \{0\}$.
$\Gamma$ is injective.

$\Leftarrow$

If $\Gamma$ is injective, then we consider
$\text{span}(\varphi_1, \cdots, \varphi_𝑚)$. From 23.b we know

$$ 
\text{span}(\varphi_1, \cdots, \varphi_𝑚) =
((\text{null } \varphi_1) \cap \cdots \cap (\text{null } \varphi_n))^0
$$

Since $\Gamma$ is injective, then

$$ 
(\text{null } \varphi_1) \cap \cdots \cap (\text{null } \varphi_n) = \{0\}
$$

Then $\{0\}^0 = V'$.

$\square$

(b) Prove that $\varphi_1, …, \varphi_𝑚$ is linearly independent if and only
if $Γ$ is surjective.

**Proof**

$\Leftarrow$

Since $Γ$ is surjective, we can find $\Gamma(v_i) = e_i$.

$$ 
\begin{align*}
a_1 v_1 + \cdots + a_m v_m = 0
&\Rightarrow 
a_1 \Gamma(v_1) + \cdots + a_m \Gamma(v_m) = 0 \\
&\Rightarrow 
a_1 e_1 + \cdots + a_m e_m = 0 \\
&\Rightarrow 
a_1 = \cdots = a_m = 0
\end{align*}
$$

Then $\varphi_i$ is the dual basis $v_i$.
Then $\varphi_1, …, \varphi_𝑚$ is linearly independent.

I cannot prove the other side easily.

So we consider the dual map of
$\Gamma ' : (F^m)' \rightarrow V'$, and $\psi_1, \cdots, \psi_m$ is
the dual basis of the standard basis of $e_i$.

$$ 
\Gamma'(\psi_i)(v) = \psi_i (\Gamma(v)) = \psi_i (\varphi_1(𝑣), …, \varphi_𝑚(𝑣)) = \varphi_i(v)
$$

So $\Gamma'(\psi_i) = \varphi_i$.

$$ 
\begin{align*}
\text{span}(\varphi_1, \cdots, \varphi_𝑚) = V'
&\Longleftrightarrow
\Gamma' \text{ is surjective } \\
&\Longleftrightarrow
\Gamma \text{ is injective } \\
\end{align*} 
$$

Also

$$ 
\begin{align*}
\varphi_1, \cdots, \varphi_𝑚 \text{ is independent }
&\Longleftrightarrow
\Gamma' \text{ is injective } \\
&\Longleftrightarrow
\Gamma \text{ is surjective } \\
\end{align*} 
$$

$\square$

### 3F.26

Suppose $𝑉$ is finite-dimensional and $Ω$ is a subspace of $𝑉'$ . Prove that

$$ 
\Omega = \{
v \in V : \varphi (v) = 0 \text{ for every } \varphi \in \Omega 
\}^0
$$

**Proof**:

Let

$$ 
U = \{
v \in V : \varphi (v) = 0 \text{ for every } \varphi \in \Omega 
\}
$$

And $\varphi_1, \cdots, \varphi_m$ be a basis of $\Omega$.

Then

$$ 
U = \{
\text{null } \varphi_1 \cap \cdots \cap \text{null } \varphi_m
\}
$$

Then from ex 2.22

$$ 
U^0 = \text{span}(\varphi_1, \cdots, \varphi_𝑚) = \Omega
$$

$\square$

### 3F.28

Suppose $𝑉$ is finite-dimensional and $\varphi_1, …, \varphi_𝑚$ is a 
linearly independent list in $𝑉'$. Prove that

$$ 
\dim ( (\text{null } \varphi_1) \cap \cdots \cap (\text{null } \varphi_m) )
=
(\dim V) - m
$$

**Proof**:

Let

$$ 
U = (\text{null } \varphi_1) \cap \cdots \cap (\text{null } \varphi_m)
$$

From ex 3F.23, $U^0 = \text{span}(\varphi_1, \cdots, \varphi_𝑚)$.
Since $\varphi_1, …, \varphi_𝑚$ is a linearly independent list,
$\dim U^0 = m$.

Then $\dim U = \dim V - m$.

$\square$

### 3F.29

Suppose 𝑉 and 𝑊 are finite-dimensional and 𝑇 ∈ ℒ(𝑉, 𝑊).

(a) Prove that if $\varphi ∈ 𝑊'$ and
$\text{null } 𝑇' = \text{span}(\varphi)$, then
$\text{range } 𝑇 = \text{null } \varphi$.

**Proof**:

$$
\begin{align*}
(\text{range } T)^0
&= \text{null } T' \\
&= \text{span}(\varphi) \\
\end{align*}
$$

If $w \in \text{range } T$, since $\varphi \in (\text{range } T)^0$ 
then $\varphi (w) = 0$, $w \in \text{null } \varphi$.

On the other hand,

$$
\begin{align*}
\dim (\text{range } T)^0
&= \dim \text{span}(\varphi) \\
&\Rightarrow \text{dim range } T = \dim W - 1 \\
&\Rightarrow \text{dim range } T = \text{dim null } \varphi \\
&\Rightarrow \text{range } T = \text{null } \varphi \\
\end{align*}
$$

$\square$

(b) Prove that if $\psi ∈ 𝑉'$ and range $𝑇' = \text{span }(\psi)$, then
$\text{null } 𝑇 = \text{null } \psi$.

**Proof**:

$$ 
(\text{null } T)^0 = \text{range } 𝑇' = \text{span }(\psi)
$$

If $v \in \text{null } T$, since $\psi \in (\text{null } T)^0$,
$\psi(v) = 0$. Then $v \in \text{null } \psi$.

$$
\begin{align*}
\text{dim null } T 
&= \dim V - \dim (\text{null } T)^0 \\
&= \dim V - 1 \\
\text{dim null } \psi
&= \dim V - 1
\end{align*}
$$

So $\text{null } 𝑇 = \text{null } \psi$.

$\square$

### 3F.30

Suppose $𝑉$ is finite-dimensional and $\varphi_1, \cdots, \varphi_m$
is a basis of $𝑉'$ . Show that
there exists a basis of $𝑉$ whose dual basis is
$\varphi_1, \cdots, \varphi_m$.

**Proof**:

We will use ex 3F.26.

Let $\Omega_1 = \text{span}(\varphi_2, \cdots, \varphi_𝑚)$.

$$ 
U_1 = \{
v \in V : \varphi (v) = 0 \text{ for every } \varphi \in \Omega_1 
\}
$$

$U_1^0 = \Omega_1$.

$$
\dim U_1^0 =
\dim \Omega_1 = n-1
$$

So $\dim U_1 = 1$, assume $v \in U_1$. If $\varphi_1 (v_1) = 0$, then
$\varphi_1 \in U_1^0 = \Omega_1$, we have a contradition.

So let $\varphi_1(v_1) \neq 0$. Assume $\varphi_1(v_1) = 1$.

The repeat this process, we can find the rest of $v_i$.

$\square$
