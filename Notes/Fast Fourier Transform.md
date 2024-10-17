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
Note that $\omega_{n}^{2j}=\omega_{2m}^{2j}=\omega_{m}^j$ and also $x^O_{j}=x_{2j+1}$ and $x^E_{j}=x_{2j}$.
We can now rewrite the original sum to get:
$$
\begin{align}
y_{l}&=\frac{1}{2m}\sum_{j=0}^{n-1}\omega_{2m}^{-2jl}x_{2j}+\frac{1}{2m}\sum_{j=0}^{n-1}\omega_{2m}^{-(2j+1)l}x_{2j+1}  \\
 & =\frac{1}{2} \frac{1}{m}\sum_{j=0}^{n-1} \omega_{m}^{-jl}x^E_{j}+\frac{1}{2}
\end{align}
$$
