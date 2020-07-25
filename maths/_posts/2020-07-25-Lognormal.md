---
title: Lognormal Distibution
layout: default
---

# Lognormal Distribution

Let \\(X\dist Lognormal(\mu, \sigma^2)\\)

Then \\(log(X)\dist Normal(\mu, \sigma^2)\\)

Let \\(m\\) and \\(s\\) denote the mean and standard deviation of X. Let \\(c=s/m\\) denote the CoV.

We have

$$
\begin{align*}
        m & = e^{\mu + \sigma^2/2} \\
        s^2 & = m^2\left(e^{\sigma^2}-1\right)
\end{align*}
$$

Therefore if you started with \\(m\\) and \\(s\\) you could calculate the underlying normal parameters thus

$$ \sigma^2 = 1+2log(s/m) = 1+2log(c) $$

$$ \mu = log(m)-\sigma^2/2 = log(m/c) - 1/2$$