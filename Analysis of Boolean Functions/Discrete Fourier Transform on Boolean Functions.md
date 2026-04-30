There are multiple ways to think of this.
### Additive
For any $r\in \mathbb{F}_{2}^{n}$ define $\chi_{r}(x)=(-1)^{r.x}$ where $r.x=\sum_{i}r_{i}x_{i} \pmod{2}$ (the [[Character]]s).
Let $f:\mathbb{F}_{2}^{n}\to \mathbb{C}$ and $r\in \mathbb{F}_{2}^{n}$.
Then the [[Discrete Fourier Transform]] of $f$ is 
$$
\hat{f}(\chi_{r})=\mathop{\Large\mathbb{E}}\limits_{x}(-1)^{r.x}f(x)
$$
We will write $\hat{f}(r)$ instead of $\hat{f}(\chi_{r})$.
### Subsets
Identify each $r\in \mathbb{F}_{2}^{n}$ with $A_{r}=\{ i:r_{i}=1 \}$.
Then $r.x=\lvert A_{r}\cap A_{x} \rvert \pmod{2}$. 
Thus take the group $(\mathcal{P}([n]),\triangle)$ and the [[discr]]
### Multiplicative