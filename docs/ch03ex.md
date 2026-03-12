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

### 3D.10

### 3D.17

Suppose 𝑉 is finite-dimensional and 𝑆 ∈ ℒ(𝑉).
Define 𝒜 ∈ ℒ(ℒ(𝑉)) by

$$ 
𝒜(𝑇) = 𝑆𝑇
$$

for 𝑇 ∈ ℒ(𝑉).

(a) Show that
$\text{dim null } 𝒜 = (\dim 𝑉)(\text{dim null } 𝑆)$.

**Proof:**

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
