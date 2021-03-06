---
layout: default
---

# Cholesky decomposition

## Statement

Let \\(A\\) be a positive definite matrix. Then there exists a unique lower triangular matrix $L$ such that $A = LL^*$.

There is a constructive proof of this fact which we shall go through but first it should be noted that there is a non-constructive proof that this result can be extended to positive *semi*-definite matrices, although then $L$ is not necessarily unique.

### Positive semi-definite matrices

Let $A$ be a positive semi-definite matrix. Define the family of operators $A_k = A + \frac{1}{k}I$. By the spectral mapping theorem, from the polynomial functional calculus, we have $\sigma(A_k)=\sigma(A)+1/k\subseteq[1/k,\infty)$ and therefore $\{A_k\}$ is a family of positive definite matrices. Therefore each $A_k$ has a Cholesky decomposition, i.e. there exists a unique lower triangular matrix $L_k$ such that $A_k = L_kL_k^*$.

Now $\|A-A_k\| = \frac{1}{k}\|I\| = \frac{1}{k}\to 0$ as $n\to\infty$ shows that $A_k$ converges to $A$ in operator norm.

Let $\mathfrak{B}(\mathbb{C}^n)$, with the operator norm, denote the Banach space of linear operators from $\mathbb{C}^n$ into $\mathbb{C}^n$. Let $\epsilon > 0$ and $N = \lceil\frac{1}{\epsilon}\rceil$, then for any $m,n>N$ we have

$$\left\|L_m - L_n\right\| = \left |\frac{1}{m} - \frac{1}{n}\right|<\frac{1}{N}<\epsilon$$

Therefore $(L_k)_k$ is a Cauchy sequence and has a limit $L\in\mathfrak{B}(\mathbb{C}^n)$ by completeness. As the underlying vector space is finite dimensional all topologies are equivalent. Therefore, as well as convergence in operator norm, we also have convergence elementwise, which ensures $L$ is also lower triangular.

Finally, $\langle Ax,y\rangle = \lim_{k\to\infty}\langle A_k,y\rangle = \lim_{k\to\infty}\langle L_kL_k^*x,y\rangle = \langle LL^*x,y\rangle$ for any $x,y\in\mathbb{C}^n$, which implies $A = LL^*$ as required.