---
title: Tossing a coin
layout: default
---

# Tossing a coin

Suppose \\(n\\) people are taking turns tossing a fair coin. The first to toss a head wins. Play proceeds sequentially 1 to \\(n\\) and round again until someone wins.

What is each player's probability of winning?

# Solution

The probability Player \\(m\\) wins is:

$$
\frac{1}{2^m}\Sum_{i=0}^{\infty}\frac{1}{2^{ni}} = \frac{1/2^m}{1-1/2^n}
$$

As a check we have

$$
\Sum_{m=1}^{n}\frac{1/2^m}{1-1/2^n}
= \frac{1}{1-1/2^n}\Sum_{m=1}^{n}\frac{1/2^m}
= \frac{1}{1-1/2^n}\frac{1/2-1/2^{n+1}}{1-1/2}
= 1
$$

# Example

For a three person game, the probability of each player winning is \\(4/7, 2/7, 1/7\\) respectively.