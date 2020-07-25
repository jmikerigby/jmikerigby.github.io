---
title: Lognormal Distibution
layout: default
---

# Lognormal Distribution

Let \\(X\sim Lognormal(\mu, \sigma^2)\\)

Then \\(log(X)\sim Normal(\mu, \sigma^2)\\)

Let \\(m\\) and \\(s\\) denote the mean and standard deviation of X. Let \\(c=s/m\\) denote the CoV.

We have

$$
\begin{align*}
        m & = e^{\mu + \sigma^2/2} \\
        s^2 & = m^2\left(e^{\sigma^2}-1\right)
\end{align*}
$$

Therefore if you started with \\(m\\) and \\(s\\) you could calculate the underlying normal parameters thus

$$ \sigma^2 = 1+2log(s/m) = log(1+c^2) $$

$$ \mu = log(m)-\sigma^2/2 = log\left(\frac{m}{\sqrt{1+c^2}}\right) $$