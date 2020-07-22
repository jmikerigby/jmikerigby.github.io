---
layout: default
---

# Poisson-Gamma mixture is Negative Binomially Distributed

Let


$$
\begin{align*}
        X & \sim Poisson(\lambda) \\
  \lambda & \sim Gamma\left(r,\frac{p}{1-p}\right)
\end{align*}
$$

We will show that the Poisson-Gamma mixture above follows a Negative Binomial Distribution.

First, recall the gamma function:

$$ \Gamma(\alpha) = \int_{0}^{\infty} x^{\alpha-1}e^{-x}dx$$

This function, which is a generalisation of the factorial function to the complex numbers, has the property:

$$\Gamma(\alpha)=(\alpha - 1)\Gamma(\alpha - 1)\tag{$\star$}$$

This will prove useful in a moment.

## Proof

$$
\begin{align*}
P(X=x) & = \int_{0}^{\infty} \left(\frac{\lambda^{x}}{x!}e^{-\lambda}\right)\left(\frac{1}{\Gamma(r) (\frac{p}{1-p})^r} \lambda^{r- 1} e^{-\frac{\lambda}{\frac{p}{1-p}}}\right)d\lambda\\
       & = \frac{1}{\Gamma(r)x!(\frac{p}{1-p})^r}\int_{0}^{\infty} \lambda^{x+r-1}e^{-\frac{\lambda}{p}}d\lambda
       & = \frac{p^{x+r}}{\Gamma(r)x!(\frac{p}{1-p})^r}\int_{0}^{\infty} u^{x+r-1}e^{-u}du
       & = p^{x}(1-p)^r\frac{\Gamma(r+x)}{\Gamma(r)x!}
       & = {r+x-1\choose r}p^{x}(1-p)^r
\end{align*}
$$
