# Chapter 1 Vector Spaces

## 1A $𝐑^𝑛$ and $𝐂^𝑛$

### 1A.1

Show that $𝛼 + 𝛽 = 𝛽 + 𝛼$ for all $𝛼, 𝛽 ∈ 𝐂$.

**Proof**:

Let

$$ 
𝛼 = a + bi, 𝛽 = c + di
$$

Then

$$ 
𝛼 + 𝛽 = (a + bi) + (c + di) =
(a + c) + (b + d)i \\
= (c+a) + (d+b)i \\
= (c + di) + (a + bi) \\
= 𝛽 + 𝛼
$$

$\square$

### 1A.2

Show that $(𝛼 + 𝛽) + 𝜆 = 𝛼 + (𝛽 + 𝜆)$ for all $𝛼, 𝛽, 𝜆 ∈ 𝐂$.

**Proof**:

$$ 
𝛼 = a + bi, 𝛽 = c + di, 𝜆 = e + fi
$$

Then

$$ 
(𝛼 + 𝛽) + 𝜆 = ((a+bi) + (c+di)) + (e + fi)\\
= ((a+c) + (b+d)i) + (e + fi)\\
= (a+c+e) + (b+d+f)i
$$

On the other hand

$$ 
𝛼 + (𝛽 + 𝜆) = (a+bi) + ((c+di) + (e+fi)) \\
= (a+bi) + ((c+e)+(d+f)i)\\
= (a+c+e)+(b+d+f)i
$$

$\square$

### 1A.3

Show that $(𝛼𝛽)𝜆 = 𝛼(𝛽𝜆)$ for all $𝛼, 𝛽, 𝜆 ∈ 𝐂$.

**Proof**:

$$ 
(𝛼𝛽)𝜆 = ((a+bi)(c+di))(e+fi) \\
= ((ac-bd) + (ad+bc)i)(e+fi) \\
= ((ac-bd)e -(ad+bc)f) + ((ac-bd)f + (ad+bc)e)i \\
= (ace - bde - adf - bcf) + (acf - bdf + ade + bce)i
$$

On the other hand

$$ 
𝛼(𝛽𝜆) = (a+bi)((c+di)(e+fi)) \\
= (a+bi)((ce-df)+(cf+de)i)\\
= (a(ce-df) - b(cf+de)) + (a(cf+de)+b(ce-df))i \\
= (ace - adf - bcf - bde) + (acf + ade + bce - bdf)i
$$

$\square$

### 1A.4

Show that $𝜆(𝛼 + 𝛽) = 𝜆𝛼 + 𝜆𝛽$ for all $𝜆, 𝛼, 𝛽 ∈ 𝐂$.

**Proof**:

$$ 
𝜆(𝛼 + 𝛽) = (e+fi)((a+bi)+(c+di)) \\
= (e+fi)((a+c)+(b+d)i)\\
= ((a+c)e - (b+d)f) + ((a+c)f + (b+d)e)i \\
$$

On the other hand

$$ 
𝜆𝛼 + 𝜆𝛽 = (e+fi)(a+bi) + (e+fi)(c+di) \\
= (ea-bf) + (eb+fa)i + (ec-fd) + (ed+fc)i \\
= (ea + ec - bf - df) + (af + cf + be + de)i
$$

$\square$

### 1A.5

Show that for every $𝛼 ∈ 𝐂$, there exists a unique $𝛽 ∈ 𝐂$ such that $𝛼 + 𝛽 = 0$.

**Proof**:

If $𝛼 = a + bi$, then let $𝛽 = (-a) + (-b)i$, we can see
$𝛼 + 𝛽 = 0$.

On the other hand, if $𝛼 + 𝛽 = 0$, then
$𝛽 = (-a) + (-b)i$.

$\square$

### 1A.6

Show that for every $𝛼 ∈ 𝐂$ with $𝛼 ≠ 0$, there exists a unique $𝛽 ∈ 𝐂$ such that $𝛼𝛽 = 1$.

**Proof**:

Let $𝛼 = a + bi$, $𝛽 = c + di$.

$$ 
𝛼𝛽 = (ac - bd) + (ad + bc)i
$$

So

$$ 
\begin{cases}
    ac - bd &= 1 \\
    ad + bc &= 0 \\
\end{cases} 
$$

Assume $a \neq 0$, then $d = -\frac{b}{a}c$

So

$$ 
ac + \frac{b^2}{a}c = 1 \\
\Rightarrow \\
c = \frac{a}{a^2 + b^2}, d = - \frac{b}{a^2 + b^2}
$$

$\square$

### 1A.7

Show that

$$ 
\frac{-1 + \sqrt[]{3} i}{2}
$$

is a cube root of 1 (meaning that its cube equals 1).

**Proof**:

let 

$$ 
r = \frac{-1 + \sqrt[]{3} i}{2}
$$

Then

$$ 
r^2 = \frac{1}{4}
((1-3) + 2 \sqrt[]{3}i) \\
= \frac{-1 - \sqrt[]{3}i}{2}
$$

Then

$$ 
r^3 = \frac{1 + 3}{4} = 1
$$

$\square$

### 1A.8

Find two distinct square roots of $𝑖$.

**Solution**:

Let $(a+bi)^2 = i$, then

$$ 
a^2 - b^2 + 2abi = i
$$

So we can have
$$ 
r_1 = \frac{\sqrt[]{2} + \sqrt[]{2}i}{2},
r_2 = \frac{-\sqrt[]{2} + -\sqrt[]{2}i}{2},
$$

$\square$

### 1A.9

Find $𝑥 ∈ 𝐑^4$ such that

$$ 
(4, −3, 1, 7) + 2𝑥 = (5, 9, −6, 8).
$$

**Solution**:

$$ 
x = (\frac{1}{2}, 6, -\frac{7}{2}, \frac{1}{2})
$$

$\square$

### 1A.10 

Explain why there does not exist $𝜆 ∈ 𝐂$ such that
$𝜆(2 − 3𝑖, 5 + 4𝑖, −6 + 7𝑖) = (12 − 5𝑖, 7 + 22𝑖, −32 − 9𝑖)$

**Proof**:

There is no $𝜆$, such that

$$ 
2𝜆 = 12 \text{ and } -3𝜆 = -5
$$

$\square$

### 1A.11

Show that $(𝑥 + 𝑦) + 𝑧 = 𝑥 + (𝑦 + 𝑧)$ for all
$𝑥, 𝑦, 𝑧 ∈ 𝐅^𝑛$.

**Proof**:

$$ 
(𝑥 + 𝑦) + 𝑧 =
(x_1 + y_1, \cdots, x_n + y_n) + z \\
= ((x_1 + y_1) + z_1, \cdots, (x_n + y_n) + z_n) \\
= (x_1 + y_1 + z_1, \cdots, x_n + y_n + z_n) \\
$$

It's same for $𝑥 + (𝑦 + 𝑧)$.

$\square$

### 1A.12

Show that $(𝑎𝑏)𝑥 = 𝑎(𝑏𝑥)$ for all $𝑥 ∈ 𝐅^𝑛$ and all
$𝑎, 𝑏 ∈ 𝐅$.

**Proof**:

$$ 
(𝑎𝑏)𝑥 = (ab)(x_1, \cdots, x_n) \\
=((ab)x_1, \cdots, (ab)x_n)
$$

$𝑎(𝑏𝑥)$ is the same.

$\square$

### 1A.13

Show that $1𝑥 = 𝑥$ for all $𝑥 ∈ 𝐅^𝑛$

**Proof**:

$$ 
1𝑥 = 1 (x_1, \cdots, x_n) \\
= (1 \cdot x_1, \cdots, 1 \cdot x_n) \\
= (x_1, \cdots, x_n) = x
$$

$\square$

### 1A.14

Show that $𝜆(𝑥 + 𝑦) = 𝜆𝑥 + 𝜆𝑦$ for all $𝜆 ∈ 𝐅$ and all 
$𝑥, 𝑦 ∈ 𝐅^𝑛$.

**Proof**:

$$ 
𝜆(𝑥 + 𝑦) = 𝜆 ((x_1, \cdots, x_n) + (y_1, \cdots, y_n)) \\
= 𝜆 (x_1+y_1, \cdots, x_n+y_n) \\
= (𝜆(x_1+y_1), \cdots, 𝜆(x_n+y_n)) \\
= (𝜆 x_1 + 𝜆 y_1, \cdots , 𝜆 x_n + 𝜆 y_n) \\
= 𝜆 (x_1, \cdots, x_n) + 𝜆 (y_1, \cdots, y_n) \\
= 𝜆 x + 𝜆 y
$$

$\square$

### 1A.15

Show that $(𝑎 + 𝑏)𝑥 = 𝑎𝑥 + 𝑏𝑥$ for all $𝑎, 𝑏 ∈ 𝐅$ and 
all $𝑥 ∈ 𝐅^𝑛$

**Proof**:

$$
\begin{split}
(𝑎 + 𝑏)𝑥 &= (a+b)(x_1, \cdots, x_n) \\
&= ((a+b)x_1, \cdots, (a+b)x_n) \\ 
&= (ax_1 + bx_1, \cdots, ax_n + bx_n) \\ 
&= (ax_1, \cdots, ax_n) + (bx_1, \cdots, bx_n) \\
&= a (x_1, \cdots, x_n) + b (x_1, \cdots, x_n) \\
&= ax + bx
\end{split}
$$

$\square$

## 1B Definition of Vector Space

### 1B.1

Prove that $−(−𝑣) = 𝑣$ for every $𝑣 ∈ 𝑉$.

**Proof**:

From $1.32$

$$ 
−(−𝑣) = (-1)(-v) \\
\Rightarrow \\
−(−𝑣) + (−𝑣) = (-1)(-v) + (1)(-v) = (-1 + 1)(-v) = 0(-v) = 0
$$

On the other hand, $v + (−𝑣) = 0$.

So both of them are the additive inverse of the $(−𝑣)$.

From $1.27$, they are the same.

$\square$

### 1B.2

Suppose $𝑎 ∈ 𝐅, 𝑣 ∈ 𝑉$ , and $𝑎𝑣 = 0$. Prove that
$𝑎 = 0$ or $𝑣 = 0$.

**Proof**:

If $a =0$, then it's valid. If $a \neq 0$, then
$a$ has a multiplicative inverse $a^{-1}$.

$a^{-1}(av) = (a^{-1}a)v = v$.

On the other hand, from 1.31, $a^{-1}0 = 0$.

So we have $v = 0$.

$\square$

### 1B.3

Suppose $𝑣, 𝑤 ∈ 𝑉$.
Explain why there exists a unique $𝑥 ∈ 𝑉$ such that
$𝑣 + 3𝑥 = 𝑤$.

**Proof**:

We add $v$'s additive inverse on both side and get

$$ 
(-v) + (𝑣 + 3𝑥) = ((-v) + v) + 3x = 0 + 3x = 3x = w - v
$$

Then we multiply the multiplicative inverse of $3$, we
got

$$ 
x = 3^{-1} (w-v)
$$

So $x$ is unique and satisfy this equation.

$\square$

### 1B.4

The empty set is not a vector space. The empty set fails to 
satisfy only one of the requirements listed in the definition of a 
vector space (1.20). Which one?

**Solution**:

It must be "additive identity":
There exists an element $0 ∈ 𝑉$ such that $𝑣 + 0 = 𝑣$ for all 
$𝑣 ∈ 𝑉$.

$\square$

### 1B.5

Show that in the definition of a vector space (1.20), the additive 
inverse condition can be replaced with the condition that

$$ 
0𝑣 = 0 \text{ for all } 𝑣 ∈ 𝑉.
$$

Here the $0$ on the left side is the number $0$, and the $0$ on 
the right side is the additive identity of $𝑉$.

**Proof**:

We just need to use this condition to prove the existence of
additive inverse.

Let $𝑣 ∈ 𝑉$, and let $w = (-1)v$, then

$$ 
w + v = (-1)v + 1v = ((-1) + 1)v = 0v = 0
$$

So $w$ is the additive inverse of $v$.

$\square$

### 1B.6

With these operations of addition and scalar multiplication, is
$𝐑 ∪ {∞, −∞}$ a vector space over $𝐑$? Explain.

**Solution**:

commutativity: yes.

associativity: no.

Let

$$ 
u = 1, v = ∞, w = -∞ \\
(u + v) + w = ∞ + (-∞) = 0 \\
u + (v+w) = 1 + (∞ + (-∞)) = 1 + 0\\
$$

So it's not a vector space over $\mathbb{R}$.

$\square$

### 1B.7

Suppose $𝑆$ is a nonempty set. Let $𝑉^𝑆$ denote the set of 
functions from $𝑆$ to $𝑉$. Define a natural addition and scalar 
multiplication on $𝑉^𝑆$ , and show that $𝑉^𝑆$
is a vector space with these definitions.

**Solution**:

Similar as 1.24, we define

* For $𝑓, 𝑔 ∈ V^𝑆$, the sum $𝑓 + 𝑔 ∈ V^𝑆$ is the function 
  defined by

$$ 
(f+g)(x) = f(x) + g(x)
$$

for all $𝑥 ∈ 𝑆$.

* For $𝜆 ∈ 𝐅$ and $𝑓 ∈ V^𝑆$, the product $𝜆 𝑓 ∈ V^𝑆$ is 
  the function defined by

$$
(𝜆𝑓)(𝑥) = 𝜆 𝑓 (𝑥)
$$

for all $𝑥 ∈ 𝑆$.

**commutativity**:

**Proof**:

$$ 
(f+g)(x) = f(x) + g(x) = g(x) + f(x) = (g+f)(x)
$$

$\square$

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

Define $0(x) = 0, \forall x \in V$.

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

### 1B.8

Suppose $𝑉$ is a real vector space.

* The complexification of $𝑉$, denoted by $𝑉^𝐂$, equals
  $𝑉×𝑉$. An element of $𝑉^𝐂$ is an ordered pair $(𝑢, 𝑣)$, where $𝑢, 𝑣 ∈ 𝑉$, but we write this as $𝑢 + 𝑖𝑣$.
* Addition on $𝑉^𝐂$ is defined by

$$ 
(𝑢_1 + 𝑖𝑣_1) + (𝑢_2 + 𝑖𝑣_2) = (𝑢_1 + 𝑢_2) + 𝑖(𝑣_1 + 𝑣_2)
$$

for all $𝑢_1, 𝑣_1, 𝑢_2, 𝑣_2 ∈ 𝑉$.

* Complex scalar multiplication on $𝑉^𝐂$ is defined by

$$ 
(𝑎 + 𝑏𝑖)(𝑢 + 𝑖𝑣) = (𝑎𝑢 − 𝑏𝑣) + 𝑖(𝑎𝑣 + 𝑏𝑢)
$$

for all $𝑎, 𝑏 ∈ 𝐑$ and all $𝑢, 𝑣 ∈ 𝑉$.

**Proof**:

**commutativity**:

$$ 
\begin{split}
(𝑢_1 + 𝑖𝑣_1) + (𝑢_2 + 𝑖𝑣_2)
&= (𝑢_1 + 𝑢_2) + 𝑖(𝑣_1 + 𝑣_2) \\
&= (𝑢_2 + 𝑢_1) + 𝑖(𝑣_2 + 𝑣_1) \\
&= (𝑢_2 + 𝑖𝑣_2) + (𝑢_1 + 𝑖𝑣_1)
\end{split}
$$

$\square$

**associativity**:

**Proof**:

$$ 
\begin{split}
((𝑢_1 + 𝑖𝑣_1) + (𝑢_2 + 𝑖𝑣_2)) + (𝑢_3 + 𝑖𝑣_3) \\
&= ((𝑢_1 + 𝑢_2) + 𝑖(𝑣_1 + 𝑣_2)) + (𝑢_3 + 𝑖𝑣_3) \\
&= ((𝑢_1 + 𝑢_2) + 𝑢_3) + 𝑖((𝑣_1 + 𝑣_2) + 𝑣_3) \\
&= (𝑢_1 + (𝑢_2 + 𝑢_3)) + 𝑖(𝑣_1 + (𝑣_2 + 𝑣_3)) \\
&= (𝑢_1 + 𝑖𝑣_1) + ((𝑢_2 + 𝑢_3) + 𝑖(𝑣_2 + 𝑣_3)) \\
&= (𝑢_1 + 𝑖𝑣_1) + ((𝑢_2 + 𝑖𝑣_2) + (𝑢_3 + 𝑖𝑣_3))
\end{split}
$$

$\square$

**additive identity**:

$$ 
(𝑢_1 + 𝑖𝑣_1) + (0 + 𝑖0) =
(𝑢_1 + 0) + 𝑖(𝑣_1 + 0) = 𝑢_1 + 𝑖𝑣_1
$$

$\square$

**additive inverse**:

$$ 
\begin{split}
(𝑢_1 + 𝑖 𝑣_1) + ((-𝑢_1) + i(-𝑣_1)) \\
&= (u_1 + (-u_1)) + i (v_1 + (-v_1)) \\
&= 0 + i 0 \\
&= 0
\end{split}
$$

$\square$

**multiplicative identity**:

$$ 
\begin{split}
(𝑢_1 + 𝑖 𝑣_1)(1 + i0) \\
&= (u_1 \cdot 1 - v_1 \cdot 0) + i (u_1 \cdot 0 + v_1 \cdot 1) \\
&= u_1 + i v_1
\end{split}
$$

**distributive properties**:

$$ 
\begin{split}
𝜆 ((𝑢_1 + 𝑖𝑣_1) + (𝑢_2 + 𝑖𝑣_2)) \\
&= 𝜆 ((𝑢_1 + 𝑢_2) + i(𝑣_1 + 𝑣_2)) \\
&= 𝜆(𝑢_1 + 𝑢_2) + i(𝜆(𝑣_1 + 𝑣_2)) \\
&= (𝜆𝑢_1 + 𝜆𝑢_2) + i((𝜆𝑣_1 + 𝜆𝑣_2)) \\
&= (𝜆𝑢_1 + 𝑖𝜆𝑣_1) + (𝜆𝑢_2 + 𝑖𝜆𝑣_2) \\
&= 𝜆 (𝑢_1 + 𝑖𝑣_1) + 𝜆 (𝑢_2 + 𝑖𝑣_2)
\end{split}
$$

$$ 
\begin{split}
(𝜆 + μ)(𝑢_1 + 𝑖𝑣_1) \\
&= (𝜆 + μ) u_1 + i ((𝜆 + μ)v_1) \\
&= (𝜆u_1 + μu_1) + i ((𝜆 v_1+ μ v_1)) \\
&= (𝜆u_1 + i 𝜆 v_1) + (μu_1 + iμ v_1) \\
&= 𝜆 (𝑢_1 + 𝑖𝑣_1) + μ (𝑢_1 + 𝑖𝑣_1)
\end{split}
$$

$\square$
