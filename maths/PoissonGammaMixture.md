---
layout: default
---

# Poisson-Gamma mixture is Negative Binomially Distributed

Let


$$
\begin{align*}
        X & \sim Poisson(\lambda) \\
  \lambda & \sim Gamma(r,\frac{p}{1-p})
\end{align*}
$$

We will show that the Poisson-Gamma mixture above follows a Negative Binomial Distribution.

First, recall the gamma function:

$$ \Gamma(\alpha) = int_{0}^{\infty} x^{\alpha-1}e^{-\alpha}dx$$