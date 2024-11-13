Let $L\subseteq \mathbb{W}$ be a [[Formal Language]]
We say $L$ satisfies the context free pumping lemma with pumping number $n$ if for every word $w\in L$ with $\lvert w \rvert\geq n$ there are words $x,u,y,v,z$ such that $w=xuyvz$, $\lvert uv \rvert>0$ and $\lvert uyv \rvert\leq n$ and for all $k\in \mathbb{N}_{0}$ we have $xu^kyv^kz\in L$.

### Theorem
For every [[Context-Free Formal Language]] $L$ there is a number $n$ such that $L$ satisfies the context free pumping lemma with pumping number $n$.
#### Proof
WLOG $G$ generating $L$ is in [[Chomsky Normal Form]].
Let $m=\lvert V \rvert$ and $n=2^m+1$. We claim $n$ is the pumping number of $G$.
