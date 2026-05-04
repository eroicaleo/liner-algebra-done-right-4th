# Chapter 4 Polynomials

## Section 4.A Polynomials

### 4A.2

Prove that if 𝑤, 𝑧 ∈ 𝐂, then ∣ |𝑤| − |𝑧| ∣ ≤ |𝑤 − 𝑧|.

**Proof**:

We can prove

$$ 
-|w-z| \leq |w| - |z| \leq |w-z|
$$

Left side

$$ 
|w| = |w-z+z| \leq |w-z| + |z|
$$

Right side

$$ 
|z| = |z-w + w| \leq |z-w| + |w| = |w-z| + |w|
$$

$\square$

### 4A.3

Suppose 𝑉 is a complex vector space and 𝜑 ∈ 𝑉′ . Define 𝜎 ∶ 𝑉 → 𝐑 by
𝜎(𝑣) = Re 𝜑(𝑣) for each 𝑣 ∈ 𝑉 . Show that

$$ 
\varphi (v) = \sigma (v) - i \sigma (iv)
$$

for all $v \in V$.

**Proof**:

Note

$$
\begin{align*}
\sigma (iv) &= \Re \varphi (iv) \\
&= \Re i \varphi (v) \\
&= - \Im \varphi (v)
\end{align*} 
$$

So

$$
\begin{align*}
\sigma (v) - i \sigma(iv)
&= \Re \varphi (v) - i(- \Im \varphi (v)) \\
&= \Re \varphi (v) + i \Im \varphi (v) \\
&= \varphi (v)
\end{align*} 
$$

$\square$

### 4A.4

Suppose $𝑚$ is a positive integer. Is the set

$$ 
\{0\} \cup \{p \in 𝒫(𝐅) : \deg p = m\}
$$

a subspace of $𝒫(𝐅)$?

**Solution**:

No. Consider $m = 2$, $p_1 = x^2 + x, p_2 = -x^2$, but $p_1+p_2 = x$.

$\square$

### 4A.5

Is the set

$$ 
U = \{0\} \cup \{p \in 𝒫(𝐅) : \deg p \text{ is even}\}
$$

a subspace of $𝒫(𝐅)$?

**Proof**:

No. Consider the same example in the previous exercise.

$\square$

### 4A.6

Suppose that 𝑚 and 𝑛 are positive integers with 𝑚 ≤ 𝑛, and suppose
$\lambda_1, …, \lambda_𝑚 ∈ 𝐅$.
Prove that there exists a polynomial $𝑝 ∈ 𝒫(𝐅)$ with
$\deg 𝑝 = 𝑛$ such that $0 = 𝑝(\lambda_1) = ⋯ = 𝑝(\lambda_𝑚)$ and such that 
$𝑝$ has no other zeros.

**Proof**:

Consider

$$ 
p(x) = (x-\lambda_1)^{n-m+1} \cdots (x-\lambda_𝑚)
$$

$\square$

### 4A.7

Suppose that $𝑚$ is a nonnegative integer,
$𝑧_1, …, 𝑧_{𝑚 + 1}$ are distinct elements
of 𝐅, and $𝑤_1, …, 𝑤_{𝑚 + 1} ∈ 𝐅$. Prove that there exists a unique 
polynomial $𝑝 ∈ 𝒫_𝑚(𝐅)$ such that

$$ 
p(z_k) = w_k
$$

for each $𝑘 = 1, …, 𝑚 + 1$.

> *This result can be proved without using linear algebra. However, try to find*
> *the clearer, shorter proof that uses some linear algebra.*

**Proof**:

Note $\mathbf{F}$ is $\mathbf{C}$ or $\mathbf{R}$.

Consider the following $m+1$ vectors in $\mathbf{F}^{m+1}$.

$$ 
v_i =
\begin{pmatrix}
z_1^i \\
z_2^i \\
\vdots \\
z_{m+1}^i \\
\end{pmatrix},
i = 0, \cdots, m
$$

If 

$$
a_0 v_0 + a_1 v_1 + \cdots + a_m v_m = 0
$$

and $a_i \neq 0$ for some $i$, that means the polynomial

$$ 
p(z) = a_0 + a_1 z + \cdots + a_{m} z^{m}
$$

has $m+1$ zeros: $z_1, \cdots, z_{m+1}$.

This is impossible, so $a_0 = \cdots = a_m = 0$.
That means $v_0, \cdots, v_m$ are linear independent.
So they are a basis of $\mathbf{F}^{m+1}$.

Then we can find 

$$ 
w = a_0 v_0 + \cdots + a_m v_m
$$

where

$$ 
w =
\begin{pmatrix}
w_1 \\
w_2 \\
\vdots \\
w_{m+1} \\
\end{pmatrix}
$$

$\square$

### 4A.8

Suppose $𝑝 ∈ 𝒫(𝐂)$ has degree $𝑚$.
Prove that $𝑝$ has $𝑚$ distinct zeros if and
only if $𝑝$ and its derivative $𝑝'$ have no zeros in common.

**Proof**:

$\Rightarrow$

Assume

$$ 
p(x) = (x-\lambda_1) \cdots (x-\lambda_m)
$$

And $\lambda_i$ are all different. We will prove $\lambda_1$ is not a zero
of $p'(x)$.

Let $g(x) = (x-\lambda_2) \cdots (x-\lambda_m)$, then $g(\lambda_1) \neq 0$.

$$
\begin{align*}
p'(x) &= g(x) + (x-\lambda_1)g'(x) \\
p'(\lambda_1) &= g(\lambda_1) + (\lambda_1-\lambda_1)g'(\lambda_1) \\
&= g(\lambda_1) \\
& \neq 0
\end{align*} 
$$

So none of $\lambda_i$ is a zero of $p'(x)$.

$\Leftarrow$

We use contradiction. Assume

$$
\begin{align*}
p(x) &= (x-\lambda)^2(x-\lambda_3)\cdots(x-\lambda_m) \\
&= (x-\lambda)^2 g(x) \\
& \Rightarrow \\
p'(x) &= 2(x-\lambda)g(x) + (x-\lambda)^2 g'(x) \\
& \Rightarrow \\
\lambda & \text{ is a zero of } p'(x)
\end{align*}
$$

Then $p, p'$ have a common zero $\lambda$.

$\square$

### 4A.9

Prove that every polynomial of odd degree with real coefficients has a real
zero.

**Proof**:

This is a immediate result from 4.16.

$\square$

### 4A.10

For $𝑝 ∈ 𝒫(𝐑)$, define $𝑇𝑝 ∶ 𝐑 → 𝐑$ by

$$ 
(Tp)(x) =
\begin{cases}
    \frac{p(x)-p(3)}{x-3} &\text{if } x \neq 3\\
    p'(3) &\text{if } x = 3\\
\end{cases} 
$$

for each $𝑥 ∈ 𝐑$. Show that $𝑇𝑝 ∈ 𝒫(𝐑)$ for every
polynomial $𝑝 ∈ 𝒫(𝐑)$ and
also show that $𝑇 ∶ 𝒫(𝐑) → 𝒫(𝐑)$ is a linear map.

**Proof**:

Assume 

$$ 
p(x)-p(3) = (x-3)g(x)
$$

We would like to show $(Tp)(x) = g(x)$.

For $x \neq 3$,

$$ 
(Tp)(x) = \frac{p(x)-p(3)}{x-3} = g(x)
$$

For $x = 3$, note $p'(x) = g(x) + (x-3)g(x)$ 

$$ 
(Tp)(x) = p'(3) = g(3) + (3-3)g(3) = g(3)
$$

So $(Tp)(x) = g(x)$. From 4.16, $g(x) \in 𝒫(𝐑)$.

Assume

$$ 
\begin{align*}
p(x) - p(3) &= (x-3)g(x) \\
q(x) - q(3) &= (x-3)h(x) \\
& \Rightarrow \\
(p+q)(x) - (p+q)(3) &= (x-3)(g+h)(x) \\
& \Rightarrow \\
T(p+q) &= g+h = Tp + Tq \\
\end{align*} 
$$

Similarly

$$ 
\begin{align*}
kp(x) - kp(3) &= (x-3)kg(x) \\
T(kp) &= kg = kTp\\
\end{align*}
$$

$\square$

### 4A.11

Suppose $𝑝 ∈ 𝒫(𝐂)$. Define $𝑞 ∶ 𝐂 → 𝐂$ by

$$ 
q(z) = p(z) \overline{p (\overline{z})}
$$

Prove that $𝑞$ is a polynomial with real coefficients.

**Proof**:

Assume

$$
\begin{align*}
p(z) &= (z - \lambda_1) \cdots (z - \lambda_m) \\
& \Rightarrow \\
\overline{p(\overline{z})} &= 
\overline{(\overline{z} - \lambda_1) \cdots (\overline{z} - \lambda_m)} \\
& \Rightarrow \\
\overline{p(\overline{z})} &=
(\overline{z} - \lambda_1) \cdots (\overline{z} - \lambda_m) \\
& \Rightarrow \\
q(z) &= (z - \lambda_1)(\overline{z} - \lambda_1)
\cdots
(z - \lambda_m)(\overline{z} - \lambda_m) \\
\end{align*} \\
$$

So $q(z) \in 𝒫(R)$

$\square$

### 4A.12

Suppose $𝑚$ is a nonnegative integer and $𝑝 ∈ 𝒫_𝑚(𝐂)$ is such that
there are distinct real numbers $𝑥_0, 𝑥_1, …, 𝑥_𝑚$ with $𝑝(𝑥_𝑘) ∈ 𝐑$ 
for each $𝑘 = 0, 1, …, 𝑚$.
Prove that all coefficients of $𝑝$ are real.

**Proof**:

We can use the same approach as 4A.7.

Consider the following $m+1$ vectors in $\mathbf{R}^{m+1}$.

$$ 
v_i =
\begin{pmatrix}
x_0^i \\
x_1^i \\
\vdots \\
x_{m}^i \\
\end{pmatrix},
i = 0, \cdots, m
$$

If 

$$
a_0 v_0 + a_1 v_1 + \cdots + a_m v_m = 0
$$

and $a_i \neq 0$ for some $i$, that means the polynomial

$$ 
p(z) = a_0 + a_1 z + \cdots + a_{m} z^{m}
$$

has $m+1$ zeros: $x_0, \cdots, x_{m}$.

This is impossible, so $a_0 = \cdots = a_m = 0$.
That means $v_0, \cdots, v_m$ are linear independent.
So they are a basis of $\mathbf{R}^{m+1}$.

Then we can find 

$$ 
w = a_0 v_0 + \cdots + a_m v_m
$$

where

$$ 
r =
\begin{pmatrix}
r_0 \\
r_1 \\
\vdots \\
r_{m} \\
\end{pmatrix}
$$

Now note that $v_0, \cdots, v_m$ are not only linear independent in
$\mathbf{R}^{m+1}$, they are also linear independent in $\mathbf{C}^{m+1}$
for the exact same reason.

So all coefficients of $𝑝$ are real.

$\square$

### 4A.13

Suppose $𝑝 ∈ 𝒫(𝐅)$ with $𝑝 ≠ 0$. Let $𝑈 = \{𝑝𝑞 ∶ 𝑞 ∈ 𝒫(𝐅)\}$.

(a) Show that $\dim 𝒫(𝐅)/𝑈 = \deg 𝑝$.

(b) Find a basis of $𝒫(𝐅)/𝑈$.

**Proof**:

Assume $\deg p = m$, and we want to show

$$ 
𝒫(𝐅)/𝑈 = 𝒫_{m-1}(𝐅)
$$

Assume $p' + U \in 𝒫(𝐅)/𝑈$, from 4.9 division algorithm for polynomials.
we can find

$$ 
p' = pq+r 
$$

where $\deg r < \deg p$, so $r \in 𝒫_{m-1}(𝐅)$.
Then $p'-r = pq \in U$. So $p'+U = r+U$.

So we established a map $T : 𝒫(𝐅)/𝑈 \rightarrow 𝒫_{m-1}(𝐅)$.

We will show this map is well defined. If $p_0 + U = p_1 + U$.

$$ 
\begin{align*}
p_0 &= pq_0 + r_0 \\
p_1 &= pq_1 + r_1 \\
& \Rightarrow \\
(p_0 - p_1) &= p(q_0 - q_1) + (r_0 - r_1) 
\end{align*} 
$$

Since $p_0 - p_1 \in U$, then $r_0 - r_1 = 0$.

It's easy to prove $T$ is an linear map.

$T$ is surjective, since if $r \in 𝒫_{m-1}(𝐅)$, $T(r+U) = r$.

If $T(p_0+U) = 0$, then $p_0 = pq + 0$ for some $q$, so $p_0 \in U$, i.e.
$p_0 + U = 0 + U$.

So $T$ is an isomorphism.

For (b), since they are isomorphic, then one basis could be

$$ 
1 + U, x + U, \cdots, x^{m-1} + U
$$

$\square$
