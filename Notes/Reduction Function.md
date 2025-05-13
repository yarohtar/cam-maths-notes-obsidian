Let $L,L'\subseteq \mathbb{B}$. 
A total [[Computable]] function $f:\mathbb{B}\to \mathbb{B}$ is a reduction from $L$ to $L'$ if for all $w\in \mathbb{B}$ we have:
$$
w \in L \iff f(w) \in L'
$$
We also say that $L$ is many-to-one reducible to $L'$.
We write $L\leq_{m} L'$
Note that $\leq_{m}$ is a [[Partial Preorder]]

### Proposition
If $L\leq_{m} L'$ and $L'$ is computable, then so is $L$.
If $L\leq$