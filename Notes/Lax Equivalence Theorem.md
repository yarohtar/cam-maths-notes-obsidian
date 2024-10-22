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
we get:
$$
\lVert A_{h} \rVert \leq 1 \text{ as } h\to 0\implies \text{the method is stable}
$$