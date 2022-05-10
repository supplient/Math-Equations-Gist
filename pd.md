# From (4) to (5)

We have

$$
\begin{aligned}
\tilde{E}_i(x,z)&=||G_ix-z||^2_F \\
\tilde{g}(x,p)&=\frac{1}{2h^2}tr((x-y)^TM(x-y))+\sum_iw_i\tilde{E}_i(x,S_ip) \\
\end{aligned}
$$


Start from $\tilde{E}_i$:

$$
\begin{aligned}
\tilde{E}_i(x,p)&=||G_ix-p||^2_F \\
&=(G_ix-p)^T(G_ix-p) \\
&=(G_ix)^T(G_ix)-p^TG_ix-(G_ix)^Tp+p^Tp \\
&=(G_ix)^T(G_ix)-2(G_ix)^Tp+p^Tp \\
\end{aligned}
$$

So, after extracting a factor $\frac{1}{2}$ and notate the constant as $C$, we have:

$$
\frac{1}{2}\tilde{E}_i(x,p)
=\frac{1}{2}(G_ix)^T(G_ix)-(G_ix)^Tp+C
$$

Then,

$$
\begin{aligned}
tr(x^TLx) 
&= x^TLx \quad \text{[$x^TLx$ is a real number]}\\
&= \sum x^TG_i^TG_ix \\
&= \sum (G_ix)^T(G_ix) \\

tr(x^TJx) 
&= x^TJx \quad \text{[$x^TJx$ is a real number]}\\
&= \sum x^TG_i^TS_ip \\
&= \sum (G_ix)^T(S_ip)
\end{aligned}
$$

So,

$$
\begin{aligned}
\sum\frac{1}{2}\tilde{E}_i(x,p)
&=\sum\frac{1}{2}(G_ix)^T(G_ix)-\sum(G_ix)^Tp+C \\
&=\frac{1}{2}(x^TLx)-x^TJp+C \\
\end{aligned}
$$