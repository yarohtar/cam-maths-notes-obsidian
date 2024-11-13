Given a set of variables $V$ and a set of terminal symbols $\Sigma$, a parse tree is a tree $T$ with labelling $\ell$ such that:
1. if $v\in T$ is a leaf then $\ell(v)\in \Sigma$
2. if $v\in T$ is not a leaf then $\ell(v)\in V$

We always look at this tree as being rooted at the top and then having a notion of left to right