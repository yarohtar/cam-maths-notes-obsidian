Suppose that a numerical method for a PDE of evolution can be written in the form 
$$
u^{n+1}=A_{h}u^{n}
$$
with zero boundary conditions

Fix a norm $\lVert  \rVert$ (any norm) and $\lVert A_{h} \rVert=\sup \frac{\lVert  A_{h}x\rVert}{\lVert x \rVert}$ 
Then since:
$$
\lVert u^n \rVert \leq \lVert A_{h}^n u^0 \rVert \leq \lVert A_{h} \rVert ^n\lVert u^0 \rVert
$$
we get that the method is [[Stability of Numerical Methods|stable]] if
$$
\lVert A_{h} \rVert \leq 1 \text{ as } h\to 0
$$
Suppose the method is also [[Consistency of Numerical Methods|consistent]]. Then, assuming $\lVert e^{0} \rVert=0$ we have $\lVert e^{n} \rVert\leq \lVert \eta^{n-1} \rVert+\dots+\lVert \eta^{0} \rVert\leq nck^{2}$ for some constant $c>0$.
Since $n\leq \frac{T}{k}$, we get $\lVert e^{n} \rVert\leq cTk$, which shows convergence. 

### Theorem (Lax equivalence)
[[Consistency of Numerical Methods]] + [[Stability of Numerical Methods]] = Convergence
#### Proof
Above we proved the implication $\implies$.

yea... thats enough.
