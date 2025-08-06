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
