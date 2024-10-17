We want to find
$$
y_{j}=(\mathcal{F}_{n}x)_{j}=\frac{1}{n}\sum_{l=0}^{n-1} \omega_{n}^{-jl}x_{l}
$$
where $j=0,\dots n-1$. 
Add zeros at the end of $x$ sequence to make $n=2^p$ and set $m=2^{p-1}$
Now denote by $E$ the set of even vertices, and by $O$ the set of odd vertices and assume we found
$$
y^E=\mathcal{F}_{m}x^E\quad \quad y^O=\mathcal{F}_{m}x^O
$$
Note that $\omega_{n}^{2k}=\omega_{2m}^{2k}=\omega_{m}^k$ and also $x^O_{l}=x_{2l+1}$ and $x^E_{l}=x_{2l}$.
We can now rewrite the original sum to get:
$$
\begin{align}
y_{l}&=\frac{1}{2m}\sum_{l=0}^{m-1}\omega_{2m}^{-2jl}x_{2l}+\frac{1}{2m}\sum_{l=0}^{m-1}\omega_{2m}^{-(2l+1)j}x_{2l+1}  \\
 & =\frac{1}{2} \frac{1}{m}\sum_{l=0}^{m-1} \omega_{m}^{-jl}x^E_{l}+\frac{1}{2} \frac{1}{m}\omega_{2m}^{-l}\sum_{l=0}^{m-1} \omega_{m}^j1x^O_{j} \\
 & =\frac{y^E_{l}+\omega_{2m}^{-l}y^O_{l}}{2}
\end{align}
$$
So we only take $O(n)$ operations to find $y$! 
Now if we do this recursively, we will only need $O(n\log n)$ operations which is much faster than the naive approach. 
## Inverse

