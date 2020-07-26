---
layout: default
---

# Puzzle - Guess the polynomial

I am thinking of a polynomial with positive coefficients:

$$p(x)=a_n x^n+\ldots + a_1 x + a_0$$

where \\(a_0, \ldots, a_n \gt 0\\)

If you give me an \\(x\\) I will tell you the evaluation \\(p(x)\\). After that you can have one more evaluation (*Hint:* you know the previous evaluation before your second go!).

Now tell me the full form of \\(p(x)\\)?

# Solution

Choose \\(x=1\\) for the first evaluation, so we know \\(p(1)\\), which is the sum of all the coefficients. As all the coefficients are positive this means each is less than \\(p(1)\\). Therefore, if our second evaluation is \\(p(p(1))\\), we know that by expanding this in base \\(p(1)\\) we will recover the coefficients.

# Example

Suppose the unknown polynomial is:

$$p(x)=x^3+2x^2+x+5$$

We are told \\(p(1)=9\\) and \\(p(p(1))=905\\). Expanding 905 out in base 9 reveals the coefficients:

$$
905 \text{(base 10)} = 1215 \text{(base 9)}
$$

Therefore:

$$p(x)=x^3+2x^2+x+5$$

Of course, if we wanted the questioner to do more of the work, we could instead ask for \\(p(\alpha)\\) for our second evaluation, where \\(\alpha=\text{min}_{m \in \mathbb{N}}\\{ 10^m\enspace|\enspace 10^m \gt p(1)\\}\\). This will leave the coefficients more easily visible and won't require expanding in another base.

In this example, we would be told

$$p(10)=1215$$