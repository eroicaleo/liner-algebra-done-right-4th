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

And assume

### 3B.21

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉, 𝑊)$, and $𝑈$
is a subspace of $𝑊$.
Prove that $\{𝑣 ∈ 𝑉 ∶ 𝑇𝑣 ∈ 𝑈\}$ is a subspace of $𝑉$ and

$$ 
\dim 
\{
v \in 𝑉 ∶ 𝑇𝑣 ∈ 𝑈
=
\text{dim null } T +
\dim (𝑈 ∩ \text{range } T)
\}
$$

**Proof**:

We first show $\{𝑣 ∈ 𝑉 ∶ 𝑇𝑣 ∈ 𝑈\}$ is a subspace of $V$.

Let $A = \{𝑣 ∈ 𝑉 ∶ 𝑇𝑣 ∈ 𝑈\}$, $v_1, v_2 \in A$, then we can find
$Tv_1 = a_1 \in U, Tv_2 = a_2 \in U$, so $T(v_1 + v_2) = a_1 + a_2 \in U$.

$T(k v_1) = k T(v_1) = k a_1 \in U$.

So $A$ is a subspace of $V$.

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
