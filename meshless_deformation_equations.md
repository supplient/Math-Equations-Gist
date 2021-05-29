# 1. Calculate the polar decomposition $A=RS$
[](https://en.wikipedia.org/wiki/Polar_decomposition)

## 1.
Do SVD on A: 

$$ A=W\sqrt{D}V^* $$

Then:

$$ A^T=V\sqrt{D}W^* $$

So, let $S$ be:

$$ S = \sqrt{A^TA} = \sqrt{VDV^*} = V\sqrt{D}V^* $$

And let R be:

$$ 
\begin{aligned}
R = AS^{-1} 
&= W\sqrt{D}V^*(V\sqrt{D}V^*)^{-1} \\
&= W\sqrt{D}V^*V\sqrt{D}^{-1}V^* \\
&= WV^*
\end{aligned}
$$

As a result:

$$
RS = WV^*V\sqrt{D}V^* = W\sqrt{D}V^* = A
$$

And apparently, S is a symmetric matrix, and R is an orthogonal matrix. So $A=RS$ is a polar decomposition.