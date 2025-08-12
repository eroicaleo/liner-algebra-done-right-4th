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
