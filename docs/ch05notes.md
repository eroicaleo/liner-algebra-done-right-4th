# Chapter 5 Eigenvalues and Eigenvectors

## Section 5A Invariant Subspaces

### 5.1 definition: operator

A linear map from a vector space to itself is called an operator.

> The reason we want to study invariant subspaces is because we want to
express the original space $V$ by the direct sum of some
smaller subspace. But we also want to each smaller subspace $V_k$ maps to
it self under $T$.

### 5.2 definition: invariant subspace

Suppose $𝑇 ∈ ℒ(𝑉$). A subspace $𝑈$ of $𝑉$ is called invariant
under $𝑇$ if $𝑇𝑢 ∈ 𝑈$ for every $𝑢 ∈ 𝑈$.

### 5.4 Examples

$\{0\}, V, \text{range } T, \text{null } T$ are all invariant under $T$.

> We investigate the simplest possible nontrivial invariant
> subspaces—invariant subspaces of dimension one.

### 5.5 definition: eigenvalue

Suppose $𝑇 ∈ ℒ(𝑉)$. A number $𝜆 ∈ 𝐅$ is called an eigenvalue of $𝑇$
if there exists $𝑣 ∈ 𝑉$ such that $𝑣 ≠ 0$ and $𝑇𝑣 = 𝜆𝑣$.

### 5.7 equivalent conditions to be an eigenvalue

Suppose $𝑉$ is finite-dimensional, $𝑇 ∈ ℒ(𝑉)$, and $𝜆 ∈ 𝐅$.
Then the following are equivalent.

(a) $𝜆$ is an eigenvalue of $𝑇$.

(b) $𝑇 − 𝜆𝐼$ is not injective.

(c) $𝑇 − 𝜆𝐼$ is not surjective.

(d) $𝑇 − 𝜆𝐼$ is not invertible.

**Proof**:

If $\lambda$ is an eigenvalue of $𝑇$, then we can find $u \neq 0$ such that
$T u = \lambda u$, then $(T - \lambda I) (u) = 0$ so
$\text{null } (𝑇 − \lambda 𝐼)$ is not $\{0\}$, so $𝑇 − \lambda 𝐼$ is not 
injective.

Conditions (b), (c), and (d) are equivalent by 3.65.

$\square$

### 5.8 definition: eigenvector

Suppose $𝑇 ∈ ℒ(𝑉)$ and $𝜆 ∈ 𝐅$ is an eigenvalue of $𝑇$.
A vector $𝑣 ∈ 𝑉$ is called
an eigenvector of $𝑇$ corresponding to $𝜆$ if $𝑣 ≠ 0$ and $𝑇𝑣 = 𝜆𝑣$.

> a vector $𝑣 ∈ 𝑉$ with $𝑣 ≠ 0$ is an eigenvector of $𝑇$ corresponding
to $𝜆$ if and only if $𝑣 ∈ \text{null } (𝑇 − \lambda 𝐼)$.

