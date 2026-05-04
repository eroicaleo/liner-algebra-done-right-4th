# Chapter 4 Polynomials

## Section 4.A Polynomials

### 4.12 fundamental theorem of algebra, first version

Every nonconstant polynomial with complex coefficients has a zero in 𝐂.

**Proof**:

Note, this is just a summary of proof, and I added some steps that are
not very clear to me.

We will need the De Moivre’s theorem

$$ 
(\cos \theta + 𝑖 \sin \theta)^𝑘 = \cos 𝑘\theta + 𝑖 \sin 𝑘\theta.
$$

We will need another fact: a continuous real-valued function on a
closed disk in $𝐑^2$ attains a minimum value.

Assume we have 

$$ 
p(z) = c_0 + c_1 z + \cdots + c_m z^m
$$

Consider the function $|p(z)|$ when $|z| \rightarrow +\infty$.

$$ 
\begin{align*}
|c_m z^m + c_{m-1} z^{m-1} + \cdots + c_1 z^1 + c_0|
&=
|z^m| | c_m + c_{m-1} z^{-1} + \cdots + c_1 z^{-(m-1)} + c_0 z^{-m}| \\
\end{align*}
$$

Note that from we have triangle inequality

$$
\begin{align*}
&|c_{m-1} z^{-1} + \cdots + c_1 z^{-(m-1)} + z^{-m}| \\
& \leq
\frac{|c_{m-1}|}{|z|} + \cdots \frac{|c_1|}{|z^{m-1}|} +
\cdots \frac{|c_0|}{|z^{m}|} \\
& \leq |c_m/2| \text{ when |z| is big enough }
\end{align*} 
$$

So when $|z|$ is big enough

$$ 
\begin{align*}
& | c_m + c_{m-1} z^{-1} + \cdots + c_1 z^{-(m-1)} + c_0 z^{-m}| \\
& \geq |c_m| - | c_{m-1} z^{-1} + \cdots + c_1 z^{-(m-1)} + z^{-m} | \\
& \geq |c_m| - |c_m / 2| \\
& = |c_m/2|
\end{align*} 
$$

So when $|z| > r$, $|p(z)| \geq |c_m/2||z^m| > |c_m/2| r^m$.
Then $|p(z)|$ achieves its minimum in $B(0, r)$.

Normalize $p(z)$ to $q(z) = 1 + a_k z^k + \cdots + a_m z^m$, where
$|q(z)|$ achieves its minimum $1$ at $z = 0$.

Let $\beta^k = -1/a_k$, let $t \in (0,1)$ such that $|\beta t| < 1$, then
check the value when $z = \beta t$,

$$ 
\begin{align*}
& |q(z)| = 1 + a_k z^k + \cdots + a_m z^m \\
& \leq | 1 + a_k z^k| + |a_{k+1} z^{k+1}| + \cdots + |a_m z^m| \\
& \leq | 1 - t^k| + |a_{k+1} z^{k+1}| + \cdots + |a_m z^m| \\
& \leq (1 - t^k) + |a_{k+1} \beta^{k+1}| t^{k+1} + \cdots + |a_m \beta^m|t^m \\
& \leq (1 - t^k) + c t^{k+1} \\
& = 1 - t^k(1 - ct) \\
\end{align*} 
$$

So if $t < \min \{1/c, 1/|\beta |\}$, where
$c = |a_{k+1} \beta^{k+1}| + \cdots + |a_m \beta^m|$,
$|q(z)| < 1$.

Then we achive a contradiction, so $\min |p(z)| = 0$.

$\square$

### 4.13 fundamental theorem of algebra, second version

If $𝑝 ∈ 𝒫(𝐂)$ is a nonconstant polynomial, then $𝑝$ has a unique 
factorization (except for the order of the factors) of the form

$$ 
p(z) = c (z-\lambda_1) \cdots (z-\lambda_m),
$$

where $c, \lambda_1, \cdots, \lambda_m \in C$.

**Proof**:

The existence part can be derived from induction, 4.6 and 4.12.

The uniqueness is as follows:

Assume

$$ 
(z-\lambda_1) \cdots (z-\lambda_m) = (z-\tau_1) \cdots (z-\tau_m)
$$

Since $\lambda_1$ is a zero, then we can find $\tau_i = \lambda_1$.
Let $\tau_1 = \lambda_1$.

For all $z \neq \lambda_1$, we have

$$ 
(z-\lambda_2) \cdots (z-\lambda_m) = (z-\tau_2) \cdots (z-\tau_m)
$$

If when $z = \lambda_1$, the left and the right side is not equal, then
assume

$$ 
\begin{align*}
p_1(z) &= (z-\lambda_2) \cdots (z-\lambda_m) \\
p_2(z) &= (z-\tau_2) \cdots (z-\tau_m) \\
\end{align*} 
$$

$p_1(z) - p_2(z)$ has infinite zeros. This contradicts with 4.8.
So $p_1(z) = p_2(z)$ for all $z \in C$.

Then we can continue with induction.

$\square$

### 4.16 factorization of a polynomial over 𝐑

Suppose $𝑝 ∈ 𝒫(𝐑)$ is a nonconstant polynomial. Then $𝑝$ has a unique 
factorization (except for the order of the factors) of the form

$$ 
𝑝(𝑥) = 𝑐(𝑥 − \lambda_1)⋯(𝑥 − \lambda_𝑚)
(𝑥^2 + 𝑏_1𝑥 + 𝑐_1)⋯(𝑥^2 + 𝑏_𝑀𝑥 + 𝑐_𝑀),
$$

**Proof summary**:

If $\lambda$ is a zero then $\bar{\lambda}$ is also a root,
assume $(x - \lambda)(x - \bar{\lambda}) = x^2 + bx + c$, then $b, c \in \mathbb{R}$.

Let $p(x) = (x^2 + bx + c) q(x)$, so $q(x) = \frac{p(x)}{(x^2 + bx + c)}$.

For any $x \in \mathbb{R}$, $q(x) \in \mathbb{R}$.

Let

$$ 
q(x) = a_0 + a_1 x + \cdots + a_{m} x^{m}
$$

Then

$$ 
0 = \Im q(x) = \Im a_0 + \Im a_1 x + \cdots + \Im a_{m} x^{m}
$$

have infinite zeros. So $\Im a_0 = \Im a_1 = \cdots = \Im a_{m} = 0$

$\square$
