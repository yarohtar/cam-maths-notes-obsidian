Let $S$ be a consistent theory in a first-order language $L=L\left( \Omega,\prod \right)$. Then $S$ has a model.

#### Idea
We build a model from the language itself 
To begin with, we let $A$ be the set of closed terms of $L$, i.e. terms with no variables
We turn this into a [[Structure]] in the obvious way
$A$ is still not a model (e.g. $1+0$ and $1$ are not equal in $A$)
Define equivalence relation $\sim$ on $A$ by 
$s\sim t$ iff $T\vdash(s=t)$ where($s,t \in A$)
Replace $A$ with $A /_{\sim}$
Two issues remain
For first issue consider the t