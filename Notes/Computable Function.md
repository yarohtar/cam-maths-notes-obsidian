Given a register machine $M$ and $k>0$, we can define a [[Partial Function]] $f_{M,k}:\mathbb{B}^{k}\dashrightarrow \mathbb{B}$ by:
1. $f_{M,k}(\vec{w})\uparrow$ iff $M$ does not halt on $\vec{w}$
2. $f_{M,k}(\vec{w})=v_{0}$ iff $M$ halts on $\vec{w}$ with register content $\vec{v}$

A partial function $f:\mathbb{B}^{k}\dashrightarrow \mathbb{B}$ is called computable if there is a register machine $M$ such that $f=f_{M,k}$. 
[[Domain of a Computable Function]]