---
layout: default
---

# Puzzle - Tossing a coin

Suppose \\(n\\) people are taking turns tossing a fair coin. The first to toss a head wins. Play proceeds sequentially 1 to \\(n\\) and round again until someone wins.

What is each player's probability of winning?

# Solution 1

The probability Player \\(m\\) wins is:

$$
\begin{align*}
\frac{1}{2^m}\sum_{i=0}^{\infty}\frac{1}{2^{ni}} &= \frac{1/2^m}{1-1/2^n} \\
&= \frac{2^{n-m}}{2^n-1}
\end{align*}
$$

**NB** The next player, \\((m+1)\\), has \\(\frac{1}{2}\\) the chances of winning as the previous player.

As a check, everything is as it should be, the chances someone wins is:

$$
\begin(align*)
\sum_{m=1}^{n}\frac{1/2^m}{1-1/2^n}
&= \frac{1}{1-1/2^n}\sum_{m=1}^{n}{1/2^m} \\
&= \frac{1}{1-1/2^n}\frac{1/2-1/2^{n+1}}{1-1/2} \\
&= 1
\begin(align*)
$$

# Solution 2

Another way of doing this is to recognise that each subsequent player has half the chances of winning as the previous player, as noted above, and someone will win eventually. 

Therefore:

$$
1 = p\sum_{m=0}^{n-1}\frac{1}{2^m}= p(2-1/2^{n-1})
$$

where \\(p\\) is the probability player 1 wins.

So:

$$
p = \frac{2^{n-1}}{2^n - 1}
$$


# Example

For a three person game, the probability of each player winning is \\(4/7, 2/7, 1/7\\) respectively.