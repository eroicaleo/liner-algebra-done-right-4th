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

## 1C Subspaces

### 1C.1

For each of the following subsets of $𝐅^3$, determine whether it 
is a subspace of $𝐅^3$.

(a) $\{(𝑥_1, 𝑥_2, 𝑥_3) ∈ 𝐅^3 ∶ 𝑥_1 + 2𝑥_2 + 3𝑥_3 = 0\}$

**Solution**:

Yes. Let it be $U$.

$$ 
0 + 2 \cdot 0 + 3 \cdot 0 = 0 
$$

So $(0,0,0) \in U$.

$$ 
(x_1 + y_1) + 2(x_2 + y_2) + 3(x_3 + y_3) = \\
(𝑥_1 + 2𝑥_2 + 3𝑥_3) + (y_1 + 2y_2 + 3y_3) = 0 + 0 = 0
$$

So $U$ is closed under addition.

$$ 
a x_1 + 2 (a x_2) + 3 (a x_3) = \\
a (𝑥_1 + 2𝑥_2 + 3𝑥_3) = a 0 = 0
$$

So $U$ is closed under scalar multiplication.

$\square$

(b) $\{(𝑥_1, 𝑥_2, 𝑥_3) ∈ 𝐅^3 ∶ 𝑥_1 + 2𝑥_2 + 3𝑥_3 = 4\}$

**Solution**:

$(0,0,0) \not\in U$.

(c) $\{(𝑥_1, 𝑥_2, 𝑥_3) ∈ 𝐅^3 ∶ 𝑥_1𝑥_2𝑥_3 = 0\}$

**Solution**:

No. Consider

$$ 
u = (1, 0, 1), v = (1, 1, 0)
$$

$u + v = (1, 1, 1)$, then $u + v \not\in U$.

$\square$

(d) $\{(𝑥_1, 𝑥_2, 𝑥_3) ∈ 𝐅^3 ∶ 𝑥_1 = 5 𝑥_3\}$

**Solution**

Yes. $0 \in U$.

$x_1 + y_1 = 5 x_3 + 5 y_3 = 5 (x_3 + y_3)$.

$$ 
ax_1 = a (5 x_3) = (a5) x_3 = (5a) x_3 = 5 (a x_3)
$$

$\square$

### 1C.2

Verify all assertions about subspaces in Example 1.35.

**Proof**: See my notes.

### 1C.3

Show that the set of differentiable real-valued functions $𝑓$ on 
the interval $(−4, 4)$ such that $𝑓'(−1) = 3𝑓(2)$ is a subspace 
of $𝐑^{(−4, 4)}$.

**Proof**:

First, the $f(x) = 0 \in U$.
Because $f'(x) = 0$, so $f'(-1) = 3 f(2) = 0$.

Secondly,

$$ 
(f+g)'(-1) = f'(-1) + g'(-1) = 3 f(2) + 3 g(2) = 3(f+g) (2)
$$

Thirdly,

$$ 
(af)'(-1) = a(f'(-1)) = a(3f(2)) = 3 ((af)(2))
$$

$\square$

### 1C.4

Suppose $𝑏 ∈ 𝐑$. Show that the set of continuous real-valued 
functions $𝑓$ on the interval $[0, 1]$ such that
$\int_{0}^{1} 𝑓 = 𝑏$ is a subspace of $𝐑^{[0, 1]}$ if and only 
if $𝑏 = 0$.

**Proof**:

$\Rightarrow$

Since $U$ is a subspace, then $0 \in U$.
$\int_{0}^{1} 0 = 0$, so $b = 0$.

$\Leftarrow$

First, $0 \in U$.

Secondly,

$$ 
\int_{0}^{1} (f+g) = 
\int_{0}^{1} f + 
\int_{0}^{1} g = 0 + 0 = 0 
$$

Thirdly,

$$ 
\int_{0}^{1} (af) = a \int_{0}^{1} f = a 0 = 0
$$

$\square$

### 1C.5

Is $𝐑^2$ a subspace of the complex vector space $𝐂^2$?

**Solution**:

No. Consider $a = i, u = (1, 0)$,
then $au = (i,0) \not\in 𝐑^2$.

So addition is not closed.

$\square$

### 1C.6

(a) Is $\{(𝑎, 𝑏, 𝑐) ∈ 𝐑^3 ∶ 𝑎^3 = 𝑏^3\}$ a subspace of 
$𝐑^3$?

**Solution**:

If $a, b \in \mathbb{R}^3$, and $a^3 = b^3$, then
$a = b$.

So if

$$ 
u = (a_1, b_1, c_1) \in U,
v = (a_2, b_2, c_2) \in U,
$$

then $a_1 = b_1, a_2 = b_2$, then $a_1+b_1 = a_2+b_2$.
So $u+v \in U$.

So it's a subspace of $𝐑^3$.

(b) Is $\{(𝑎, 𝑏, 𝑐) ∈ 𝐂^3 ∶ 𝑎^3 = 𝑏^3\}$ a subspace of $𝐂^3$.

Consider

$$ 
u = (1, 1, 0),
v = (\frac{-1 + i\sqrt[]{3}}{2}, 1)
$$

Note

$$
\left( \frac{-1 + i\sqrt[]{3}}{2} \right)^2 \\
= \frac{1 - 2 i \sqrt[]{3} - 3}{4} \\
= \frac{-1 - i \sqrt[]{3}}{2}
$$

So

$$ 
\left( \frac{-1 + i\sqrt[]{3}}{2} \right)^3 = 1
$$

Now

$$ 
\left( \frac{1 + i\sqrt[]{3}}{2} \right)^2 \\
= \frac{1 + 2 i \sqrt[]{3} - 3}{4} \\
= \frac{-1 + i \sqrt[]{3}}{2}
$$

Then

$$ 
\left( \frac{1 + i\sqrt[]{3}}{2} \right)^3 = -1
$$

So $u+v \not\in U$.

$\square$

### 1C.7

Prove or give a counterexample: If $𝑈$ is a nonempty subset of 
$𝐑^2$ such that $𝑈$ is closed under addition and under taking 
additive inverses (meaning $−𝑢 ∈ 𝑈$ whenever $𝑢 ∈ 𝑈$), then
$𝑈$ is a subspace of $𝐑^2$.

**Solution**:

Counterexample: Consider

$$ 
U =
\{
(n, 0) | n \in \mathbb{Z}
\}
$$

$\square$

### 1C.8

Give an example of a nonempty subset $𝑈$ of $𝐑^2$ such that $𝑈$ 
is closed under scalar multiplication, but $𝑈$ is not a subspace 
of $𝐑^2$.

**Solution**

Consider

$$ 
U =
\{(a, 0) | a \in \mathbb{R}\}
\cup
\{(0, b) | b \in \mathbb{R}\}
$$

$\square$

### 1C.9

A function $𝑓 ∶ 𝐑 → 𝐑$ is called periodic if there exists a 
positive number $𝑝$ such that $𝑓(𝑥) = 𝑓(𝑥 + 𝑝)$ for all
$𝑥 ∈ 𝐑$. Is the set of periodic functions
from $𝐑$ to $𝐑$ a subspace of $𝐑^𝐑$ ? Explain.

**Solution**:

This example is inspired from
"Lectures on the Fourier Transform and Its Applications"
exercise 1.2.

Let

$$ 
f(t) = \begin{cases}
  1 &\text{if } t \in \mathbb{Z} \\
  0 &\text{otherwise} \\
\end{cases} 
$$

$$ 
g(t) = \begin{cases}
  1 &\text{if } t = n \sqrt[]{2}, n \in \mathbb{Z}\\
  0 &\text{otherwise} \\
\end{cases} 
$$

$f+g$ cannot be a periodic function, since
$(f+g)(t) \neq 2, t \neq 0$.

If $f(t) = g(t) = 1$, then $t = n = m \sqrt[]{2}$.
That means $n/m = \sqrt[]{2}$.

$\square$

### 1C.10

Suppose $𝑉_1$ and $𝑉_2$ are subspaces of $𝑉$.
Prove that the intersection $𝑉_1 ∩ 𝑉_2$
is a subspace of $𝑉$.

**Proof**:

$0 \in V_1, 0 \in V_2$, so $0 \in 𝑉_1 ∩ 𝑉_2$.

$a,b \in V_1, a,b \in V_2$ so $a+b \in 𝑉_1 ∩ 𝑉_2$.

$k \in F, a \in 𝑉_1 ∩ 𝑉_2$, so $k a \in 𝑉_1 ∩ 𝑉_2$.

$\square$

### 1C.11

Prove that the intersection of every collection of subspaces of 𝑉 
is a subspace of 𝑉 .

**Proof**: Very similar to the previous one.

$\square$

### 1C.12

Prove that the union of two subspaces of $𝑉$ is a subspace of 
$𝑉$ if and only if one of the subspaces is contained in the other.

**Proof**:

$\Rightarrow$

Assume $U, W, U \cup W$ are subspaces. If $a \in U, a \not\in W$.
Now assume $b \in W$, since $a+b \in U \cup W$.
If $a+b \in W$, then $(a+b) + (-b) = a \in W$, we have contradition.

So $a+b \in U$, then $(a+b) + (-a) = b \in U$, so
$W \subseteq U$.

$\Leftarrow$ is obvious.

$\square$

### 1C.13

Prove that the union of three subspaces of $𝑉$ is a subspace of $𝑉$ if and only if one of the subspaces contains the other two.

This exercise is surprisingly harder than Exercise 12, possibly because this exercise is not true if we replace $𝐅$ with a field containing only two elements.

**Proof**:

Assume $a, b, c$ are unique elements in $A, B, C$.

Now, consider $a+b$.

If $a+b \in A$, then $b \in A$, we have contradition.

If $a+b \in B$, then $a \in B$, we have contradition.

So $a+b \in C$. For the same reason, $a-b \in C$.

That means $a, b \in C$. We have contradition.

This means, one the following must be true:

$$ 
A \subseteq B \cup C \text{ or }
B \subseteq C \cup A \text{ or }
C \subseteq A \cup B
$$

In either case, this problem is reduced to 1C.12.

$\square$

### 1C.14

Suppose

$$ 
𝑈 = \{(𝑥, −𝑥, 2𝑥) ∈ 𝐅^3 ∶ 𝑥 ∈ 𝐅\}
\quad \text{and} \quad
𝑊 = \{(𝑥, 𝑥, 2𝑥) ∈ 𝐅^3 ∶ 𝑥 ∈ 𝐅\}.
$$

Describe $𝑈 + 𝑊$ using symbols, and also give a 
description of $𝑈 + 𝑊$ that uses no symbols.

**Solution**:

$$ 
U+W = \{
(x, y, 2x) \in 𝐅^3 ∶ 𝑥 ∈ 𝐅\}
$$

$\square$

### 1C.15

Suppose $𝑈$ is a subspace of $𝑉$ . What is $𝑈 + 𝑈$?

**Solution**:

It's still $U$.

$\square$

### 1C.16

Is the operation of addition on the subspaces of
$𝑉$ commutative? In other words, if $𝑈$ and $𝑊$ are 
subspaces of $𝑉$ , is $𝑈 + 𝑊 = 𝑊 + 𝑈$?

**Solution**:

Yes, this is because the vector space itself is
commutative.

$\square$

### 1C.17

Is the operation of addition on the subspaces of $𝑉$ 
associative? In other words, if
$𝑉_1, 𝑉_2, 𝑉_3$ are subspaces of $𝑉$ , is

$$ 
(V_1 + V_2) + V_3 = V_1 + (V_2 + V_3)?
$$

**Solution**:

Yes, this is because the vector space itself is
associative.

$\square$

### 1C.18

Does the operation of addition on the subspaces of $𝑉$ 
have an additive identity? Which subspaces have additive 
inverses?

**Solution**:

Yes. The subspace contains only $0$. Only itself has
additive inverse, which is itself.

$\square$

### 1C.19

Prove or give a counterexample: If $𝑉_1, 𝑉_2, 𝑈$ are 
subspaces of $𝑉$ such that

$$ 
V_1 + U = V_2 + U
$$

then $𝑉_1 = 𝑉_2$.

**Solution**:

Counterexample, consider

$$ 
V_1 = \{(x, 0, 0) \in F^3\} \\
V_2 = \{(0, y, 0) \in F^3\} \\
U = \{(x, y, 0) \in F^3\} \\
$$

Then $V_1 + U = U = V_2 + U$, but $V_1 \neq V_2$.

$\square$

### 1C.20

Suppose

$$ 
𝑈 = \{(𝑥, 𝑥, 𝑦, 𝑦) ∈ 𝐅^4 ∶ 𝑥, 𝑦 ∈ 𝐅\}.
$$

Find a subspace $𝑊$ of $𝐅^4$ such that $𝐅^4 = 𝑈 ⊕ 𝑊$.

**Solution**:

Consider

$$ 
W = \{(𝑥, -𝑥, 𝑦, -𝑦) ∈ 𝐅^4 ∶ 𝑥, 𝑦 ∈ 𝐅\}.
$$

Then $U \cap W = 0$.

$\square$

### 1C.21

Suppose

$𝑈 = \{(𝑥, 𝑦, 𝑥 + 𝑦, 𝑥 − 𝑦, 2𝑥) ∈ 𝐅^5 ∶ 𝑥, 𝑦 ∈ 𝐅\}.$

Find a subspace $𝑊$ of $𝐅^5$ such that $𝐅^5 = 𝑈 ⊕ 𝑊$.

**Solution**

Consider

$$ 
W = \{(0, 0, a, b, c) ∈ 𝐅^5 ∶ a, b, c ∈ 𝐅 \}.
$$

$\square$

### 1C.22

Suppose

$𝑈 = \{(𝑥, 𝑦, 𝑥 + 𝑦, 𝑥 − 𝑦, 2𝑥) ∈ 𝐅^5 ∶ 𝑥, 𝑦 ∈ 𝐅\}.$

Find a subspace $𝑊_1, W_2, W_3$ of $𝐅^5$ such that $𝐅^5 = 𝑈 ⊕ 𝑊_1 ⊕ 𝑊_2 ⊕ 𝑊_3$.

**Solution**:

Consider

$$ 
W_1 = \{(0, 0, x_1, 0, 0) ∈ 𝐅^5 ∶ w_1, x_1, y_1, z_1 ∈ 𝐅 \} \\
W_2 = \{(0, 0, 0, y_2, 0) ∈ 𝐅^5 ∶ y_2, z_2 ∈ 𝐅 \} \\
W_3 = \{(0, 0, 0, 0, z_3) ∈ 𝐅^5 ∶ z_3 ∈ 𝐅 \} \\
$$

So if $u + w_1 + w_2 + w_3 = 0$, then we must have

$$
\begin{cases}
  x + 0 + 0 + 0 = 0 &\text{}\\
  y + 0 + 0 + 0 = 0 &\text{}\\
  (x + y) + x_1 + 0 + 0 = 0 &\text{}\\
  (x - y) + 0 + y_2 + 0 = 0 &\text{}\\
  2x + 0 + 0 + z_3 = 0 &\text{}\\
\end{cases}
$$

then we must have

$$ 
x = y = x_1 = y_2 = z_3 = 0 \\
\Rightarrow \\
u = w_1 = w_2 = w_3 = 0
$$

So $𝐅^5 = 𝑈 ⊕ 𝑊_1 ⊕ 𝑊_2 ⊕ 𝑊_3$.

$\square$

### 1C.23

Prove or give a counterexample: If $𝑉_1, 𝑉_2, 𝑈$ are subspaces of $𝑉$ such that

$$ 
𝑉 = 𝑉_1 ⊕ 𝑈
\quad \text{and} \quad
𝑉 = 𝑉_2 ⊕ 𝑈,
$$

then $𝑉_1 = 𝑉_2$.

Hint: When trying to discover whether a conjecture in 
linear algebra is true or false, it is often useful to 
start by experimenting in $𝐅^2$.

**Solution**:

Counterexample:

As hinted, let $F = \mathbb{R}$.

$$ 
U = (x, 0) \\
V_1 = (0, y) \\
V_2 = (z, z) \\
$$

So

$$ 
𝑉_1 ⊕ 𝑈 = \mathbb{R}^2 = 𝑉_2 ⊕ 𝑈
$$

But $V_1 \neq V_2$.

$\square$

### 1C.24

A function $𝑓 ∶ 𝐑 → 𝐑$ is called even if

$$ 
f(-x) = f(x)
$$

for all $𝑥 ∈ 𝐑$. A function $𝑓 ∶ 𝐑 → 𝐑$ is called odd if

$$ 
f(-x) = -f(x)
$$

for all $𝑥 ∈ 𝐑$. Let $𝑉_e$ denote the set of 
real-valued even functions on $𝐑$
and let $𝑉_o$ denote the set of real-valued odd 
functions on $𝐑$. Show that
$𝐑^𝐑 = 𝑉_e ⊕ 𝑉_o$.

**Solution**:

We have seen this again in the book of 
"Lectures on the Fourier Transform and Its Applications"
Appendix B.

Let

$$ 
f_e(x) = \frac{f(x) + f(-x)}{2} \\
f_o(x) = \frac{f(x) - f(-x)}{2} \\
$$

Then $f_e$ is even, and $f_o$ is odd.
Furthermore, $f = f_e + f_o$.
This proves $𝐑^𝐑 = 𝑉_e + 𝑉_o$.

Now if $f \in 𝑉_e \cap 𝑉_o$, then $f(x) = f(-x) = -f(x)$
so $f(x) = 0$, i.e. $𝑉_e \cap 𝑉_o = 0$.

So $𝐑^𝐑 = 𝑉_e ⊕ 𝑉_o$.

$\square$
