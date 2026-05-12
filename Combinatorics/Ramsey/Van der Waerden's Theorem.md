Let $m,k\in \mathbb{N}$.
Then there is some $n\in \mathbb{N}$ such  that whenever $[n]$ is $k$-coloured,
there exists a monochromatic arithmetic progression of length $m$.
In particular, the [[Waerden's Number]] $W(m,k)$ exists.
### Proof
We proceed by induction on $m$.
The case $m=1$ is trivial. 
Suppose we have proved the claim for $m-1$.
We show the following claim:
For all $r\leq k$, there exists some $n$ such that whenever $[n]$ is $k$-coloured,
then either there is a monochromatic arithmetic progression of length $m$,
or $r$ [[Colour-Focused]] arithmetic progressions of length $m-1$
We do an induction on $r$.
For $r=1$, we can set $n=W(m-1,k)$ to find one colour-focused progression.