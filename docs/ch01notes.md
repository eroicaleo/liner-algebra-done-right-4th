# Chapter 1 Vector Spaces

## 1B Definition of Vector Space

### 1.24 notation $F^S$

* If $𝑆$ is a set, then $𝐅^𝑆$ denotes the set of functions from 
  $𝑆$ to $𝐅$.
* For $𝑓, 𝑔 ∈ 𝐅^𝑆$, the sum $𝑓 + 𝑔 ∈ 𝐅^𝑆$ is the function 
  defined by

$$ 
(f+g)(x) = f(x) + g(x)
$$

for all $𝑥 ∈ 𝑆$.

* For $𝜆 ∈ 𝐅$ and $𝑓 ∈ 𝐅^𝑆$, the product $𝜆 𝑓 ∈ 𝐅^𝑆$ is 
  the function defined by

$$
(𝜆𝑓)(𝑥) = 𝜆 𝑓 (𝑥)
$$

for all $𝑥 ∈ 𝑆$.

### 1.25 example: $𝐅^𝑆$ is a vector space

* If $𝑆$ is a nonempty set, then $𝐅^𝑆$ (with the operations of 
  addition and scalar multiplication as defined above) is a vector space over $𝐅$.

**commutativity**:

**Proof**:

$$ 
(f+g)(x) = f(x) + g(x) = g(x) + f(x) = (g+f)(x)
$$

**associativity**:

**Proof**:

$$ 
((f+g)+h)(x) = (f+g)(x) + h(x) = (f(x) + g(x)) + h(x) \\
=f(x) + (g(x) + h(x)) = f(x) + (g+h)(x) \\
= (f + (g+h))(x)
$$

$$ 
((ab)f)(x) = (ab) f(x) = a (bf(x)) = a ((bf)(x)) = (a(bf))(x)
$$

$\square$

**additive identity**:

**Proof**:

Define $0(x) = 0, \forall x \in S$.

$$ 
(f+0)(x) = f(x) + 0(x) = f(x) + 0 = f(x)
$$

$\square$

**additive inverse**:

**Proof**:

Define $g(x) = -f(x)$, then

$$ 
(f+g)(x) = f(x) + g(x) = f(x) + (-f(x)) = 0
$$

**multiplicative identity**:

**Proof**:

$$
(1 \cdot f)(x) = 1 \cdot f(x) = f(x)
$$

$\square$

**distributive properties**:

$$ 
(𝜆(𝑓+g))(𝑥) = 𝜆 ((𝑓+g)(x)) = 𝜆 (f(x) + g(x)) \\
= 𝜆f(x) + 𝜆g(x) = (𝜆f)(x) + (𝜆g)(x) = (𝜆f + 𝜆f)(x)
$$

$$ 
((𝜆 + μ)f)(x) = (𝜆 + μ) f(x) = 𝜆f(x) + μf(x) \\
= (𝜆f)(x) + (μf)(x) = (𝜆f + μf)(x)
$$

$\square$

* The additive identity of $𝐅^𝑆$ is the function $0 ∶ 𝑆 → 𝐅$ 
  defined by

$$ 
0(x) = 0
$$

for all $𝑥 ∈ 𝑆$.

Already proved above.

* For $𝑓 ∈ 𝐅^𝑆$, the additive inverse of $𝑓$ is the function $− 𝑓 ∶ 𝑆 → 𝐅$ defined by

$$ 
(-f)(x) = -f
$$

for all $𝑥 ∈ 𝑆$.

Already proved above.

The vector space $𝐅^𝑛$ is a special case
of the vector space 𝐅𝑆 because each
$(𝑥_1, …, 𝑥_𝑛) ∈ 𝐅^𝑛$ can be thought of as
a function $𝑥$ from the set $\{1, 2, …, 𝑛\}$ to $𝐅$.

### 1.26 unique additive identity

### 1.27 unique additive inverse

### 1.30 the number 0 times a vector

$$ 
0𝑣 = 0, \forall v \in V
$$

### 1.31 a number times the vector 0

$$ 
𝑎0 = 0, \forall a \in F
$$

### 1.32 the number −1 times a vector

$$ 
(−1)𝑣 = −𝑣, \forall v \in V
$$

## 1C Subspaces

### 1.33 definition: subspace

A subset $𝑈$ of $𝑉$ is called a subspace of $𝑉$ if $𝑈$ is also 
a vector space with the same additive identity, addition, and 
scalar multiplication as on $𝑉$ .

### 1.34 conditions for a subspace

A subset $𝑈$ of $𝑉$ is a subspace of $𝑉$ if and only if $𝑈$ satisfies the following three conditions.

**additive identity**:

$$ 
0 ∈ 𝑈.
$$

**closed under addition**:

𝑢, 𝑤 ∈ 𝑈 implies 𝑢 + 𝑤 ∈ 𝑈.

**closed under scalar multiplication**:

𝑎 ∈ 𝐅 and 𝑢 ∈ 𝑈 implies 𝑎𝑢 ∈ 𝑈.

### 1.35 example: subspaces

(a) If $𝑏 ∈ 𝐅$, then

$$ 
\{(𝑥_1, 𝑥_2, 𝑥_3, 𝑥_4) ∈ 𝐅^4 ∶ 𝑥_3 = 5𝑥_4 + 𝑏\}
$$

is a subspace of $𝐅^4$ if and only if $𝑏 = 0$.

**Proof**:

Let $U = \{(𝑥_1, 𝑥_2, 𝑥_3, 𝑥_4) ∈ 𝐅^4 ∶ 𝑥_3 = 5𝑥_4 + 𝑏\}$.
If $U$ is a subspace, then $0 \in U$, then

$$ 
0 = 5 \cdot 0 + b \Rightarrow b = 0
$$

Conversely, assume $b = 0$. Then $0 \in U$.

If $x = (𝑥_1, 𝑥_2, 𝑥_3, 𝑥_4), y = (y_1, y_2, y_3, y_4) \in U$, 
then

$$ 
𝑥_3 = 5𝑥_4, y_3 = 5y_4 \\
\Rightarrow \\
𝑥_3 + y_3 = 5 (𝑥_4 + y_4)
$$

So $x+y \in U$.

Also we have

$$ 
𝑥_3 = 5𝑥_4 \\
\Rightarrow \\
a𝑥_3 = a5𝑥_4 = 5 (a𝑥_4) \\
$$

So $ax \in U$.

$\square$

(b) The set of continuous real-valued functions on the interval 
$[0, 1]$ is a subspace of $𝐑^{[0, 1]}$.

**additive identity**:

Since $0$ is a continuous function, so

$$ 
0 ∈ 𝑈.
$$

**closed under addition**:

If $f, g$ are continuous function, then $f+g$ is also
continuous function on $[0,1]$.

**closed under scalar multiplication**:

If $f$ is continuous and $a \in \mathbb{R}$, then
$af$ is also continuous.

$\square$

(c) The set of differentiable real-valued functions on 𝐑 is a subspace of $𝐑^𝐑$.

**additive identity**:

Since $0$ is a differentiable function, so

$$ 
0 ∈ 𝑈.
$$

**closed under addition**:

If $f, g$ are differentiable function, then $f+g$ is also
differentiable function on $\mathbb{R}$.

**closed under scalar multiplication**:

If $f$ is differentiable and $a \in \mathbb{R}$, then
$af$ is also differentiable.

$\square$

(d) The set of differentiable real-valued functions $𝑓$ on the 
interval $(0, 3)$ such that $𝑓' (2) = 𝑏$ is a subspace of
$𝐑^(0, 3)$ if and only if $𝑏 = 0$.

$\Rightarrow$

Since $0 \in U$, and $0'(2) = 0$ then $b = 0$.

$\Leftarrow$ 

$0$ is differentiable and $0'(2) = 0 = b$.
So $0 \in U$.

If $f,g$ are differentiable and $f'(2) = g'(2) = 0$, then

$$ 
(f+g)'(2) = f'(2) + g'(2) = 0 + 0 = 0
$$

If $f$ is differentiable and $f'(2) = 0$, then

$$ 
(af)'(2) = a (f'(2)) = a 0 = 0
$$

$\square$

(e) The set of all sequences of complex numbers with limit 0 is a 
subspace of $𝐂^∞$ .

**Proof**:

First, $(0, 0, 0, \dots) \rightarrow 0$.
So $0 \in U$.

Then if $(a_n), (b_n) \rightarrow 0$, then

$$ 
\lim_{n \to \infty} (a_n+b_n) =
\lim_{n \to \infty} a_n + \lim_{n \to \infty} b_n =
0
$$

Lastly,

$$ 
\lim_{n \to \infty} a b_n = a \lim_{n \to \infty} b_n = 0
$$

$\square$

* The subspaces of $𝐑^2$ are precisely $\{0\}$, all lines in 
  $𝐑^2$ containing the origin, and $𝐑^2$ .
* The subspaces of $𝐑^3$ are precisely $\{0\}$, all lines in 
  $𝐑^3$ containing the origin, all planes in $𝐑^3$ containing 
  the origin, and $𝐑^3$ .

### Sums of Subspaces

### 1.36 definition: sum of subspaces

Suppose $𝑉_1, \cdots, 𝑉_𝑚$ are subspaces of 𝑉 . The sum of 
$𝑉_1, \cdots, 𝑉_𝑚$, denoted by $𝑉_1 + ⋯ + 𝑉_𝑚$, is the set of all possible sums of elements of $𝑉_1, \cdots, 𝑉_𝑚$. More
precisely,

$$ 
V_1 + \cdots + V_m =
\{
v_1 + \cdots + v_m :
v_1 \in V_1, \cdots, v_m \in V_m
\}.
$$

### 1.37 example: a sum of subspaces of $𝐅^3$

Suppose $𝑈$ is the set of all elements of $𝐅^3$ whose second and 
third coordinates equal $0$, and 𝑊 is the set of all elements of 
$𝐅^3$ whose first and third coordinates equal 0:

$$ 
𝑈 = \{(𝑥, 0, 0) ∈ 𝐅^3 ∶ 𝑥 ∈ 𝐅\}
\quad \text{and} \quad
W = \{(0, y, 0) ∈ 𝐅^3 ∶ 𝑥 ∈ 𝐅\}
$$

Show that $U+W = \{(𝑥, 𝑦, 0) ∈ 𝐅^3 ∶ 𝑥, 𝑦 ∈ 𝐅\}$.

**Proof**:

Let $V = \{(𝑥, 𝑦, 0) ∈ 𝐅^3 ∶ 𝑥, 𝑦 ∈ 𝐅\}$.

If $u = (x,0,0), w = (0,y,0)$, then
$u+w = (x,y,0) \in V$. So $U+W \subseteq V$.

Let $v = (x,y,0) \in V$, then let
$u = (x,0,0) \in U, w = (0,y,0) \in W$,
so $v = u+w \in U+W$, i.e. $V \subseteq U+W$.

So $U+W = V$.

$\square$

### 1.40 sum of subspaces is the smallest containing subspace

Suppose $V_1, \cdots, V_m$ are subspaces of 𝑉. Then
$V_1 + \cdots + V_n$ is the smallest
subspace of 𝑉 containing $V_1, \cdots, V_m$.

**Proof**:

Let $U = V_1 + \cdots + V_n$, we first prove
$U$ is a subspace.

First $0 \in V_i, i = 1, \cdots, m$, so
$0 \in U$.

Secondly, given $a, b \in U$, then

$$ 
a = a_1 + \cdots + a_m \\
b = b_1 + \cdots + b_m \\
\Rightarrow \\
a+b = (a_1 + b_1) + \cdots + (a_n + b_n) \in U
$$

Finally, if $a \in F, u \in U$, then

$$ 
u = v_1 + \cdots + v_m \\
\Rightarrow \\
au = a(v_1 + \cdots + v_m)
= av_1 + \cdots + av_m \in U
$$

So $U$ is a subspace of $V$.

Then assume $V_i \subseteq U', i = 1, \cdots, m$.
Let $u \in V_1 + \cdots + V_n$, so

$$ 
u = v_1 + \cdots + v_m \\
\Rightarrow \\
v_i \in V_i \subseteq U' \\
\Rightarrow \\
u \in U'
$$ 

So $V_1 + \cdots + V_n \subseteq U$.

$\square$

### Direct Sums

### 1.41 definition: direct sum, $⊕$

Suppose $V_1, \cdots, V_m$ are subspaces of $𝑉$.

* The sum $V_1 + \cdots + V_m$ is called a direct sum if each 
  element of $V_1 + \cdots + V_m$ can be written in only one 
  way as a sum $v_1 + \cdots + v_m$, where each
  $𝑣_𝑘 ∈ 𝑉_𝑘$.

* If $V_1 + \cdots + V_m$ is a direct sum, then
  $V_1 ⊕ \cdots ⊕ V_m$ denotes $V_1 + \cdots + V_m$,
  with the $⊕$ notation serving as an indication that this is 
  a direct sum.

### 1.42 example: a direct sum of two subspaces

$$
𝑈 = \{(𝑥, 𝑦, 0) ∈ 𝐅^3 ∶ 𝑥, 𝑦 ∈ 𝐅\}
\quad \text{and} \quad
𝑊 = \{(0, 0, 𝑧) ∈ 𝐅^3 ∶ 𝑧 ∈ 𝐅\}.
$$

Then $𝐅^3 = 𝑈 ⊕ 𝑊$.

> The symbol $⊕$, which is a plus sign
> inside a circle, reminds us that we are
> dealing with a special type of sum of
> subspaces—each element in the direct
> sum can be represented in only one way
> as a sum of elements from the specified
> subspaces.

### 1.44 example: a sum that is not a direct sum

Suppose

$$ 
𝑉_1 = \{(𝑥, 𝑦, 0) ∈ 𝐅^3 ∶ 𝑥, 𝑦 ∈ 𝐅\}, \\
𝑉_2 = \{(0, 0, 𝑧) ∈ 𝐅^3 ∶ 𝑧 ∈ 𝐅\}, \\
𝑉_3 = \{(0, 𝑦, 𝑦) ∈ 𝐅^3 ∶ 𝑦 ∈ 𝐅\}. \\
$$

Note we have

$$ 
(0, 0, 0) = (0, 1, 0) + (0, 0, 1) + (0, −1, −1) \\
(0, 0, 0) = (0, 0, 0) + (0, 0, 0) + (0, 0, 0)
$$

$\square$

### 1.45 condition for a direct sum

Suppose $V_1, \cdots, V_m$ are subspaces of $𝑉$.
Then $V_1 + \cdots + V_m$ is a direct sum if
and only if the only way to write $0$ as a sum
$𝑣_1 +⋯ + 𝑣_𝑚$, where each $𝑣_𝑘 ∈ 𝑉_𝑘$,
is by taking each $𝑣_𝑘$ equal to $0$.

**Proof**:

$\Rightarrow$

By definition, if $V_1 + \cdots + V_m$ is a direct sum,
then $0$ can be written in only one way,
since $0 + \cdots + 0 = 0$, then it is the only way.

$\Leftarrow$

Assume 

$$ 
v = v_1 + \cdots + v_m \\
v = v_1' + \cdots + v_m' \\
$$

Then

$$ 
0 = v - v = (v_1 - v_1') + \cdots + (v_m - v_m')
$$

Then

$$ 
v_1 = v_1', \cdots, v_m = v_m'
$$

So $V_1 + \cdots + V_m$ is a direct sum.

$\square$

### 1.46 direct sum of two subspaces

Suppose $𝑈$ and $𝑊$ are subspaces of $𝑉$. Then

$$ 
U+W \text{ is a direct sum} \Longleftrightarrow
𝑈 ∩ 𝑊 = \{0\}.
$$

**Proof**:

$\Rightarrow$

If $U+W$ is a direct sum, and assume $u \in 𝑈 ∩ 𝑊$,
then $-u \in 𝑈 ∩ 𝑊$. So

$$ 
u + (-u) = 0
$$

Then $u = 0$. So $𝑈 ∩ 𝑊 = \{0\}$.

$\Leftarrow$

If $u + w = 0, u \in U, w \in W$, then $w = -u \in U$.
So $w \in 𝑈 ∩ 𝑊 \Rightarrow w = 0$. So $u = 0$.
Then from 1.45, $U+W$ is a direct sum.

$\square$

> Sums of subspaces are analogous to
unions of subsets. Similarly, direct
sums of subspaces are analogous to
disjoint unions of subsets. No two sub-
spaces of a vector space can be disjoint,
because both contain 0. So disjoint-
ness is replaced, at least in the case
of two subspaces, with the requirement
that the intersection equal {0}.