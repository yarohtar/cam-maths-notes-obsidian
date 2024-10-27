### Lemma (First Borel-Cantelli Lemma)
If $\sum_{n}\mu(A_{n})<\infty$, then $\mu(\lim\sup A_{n})=0$
#### Proof
As $n\to \infty$
$$
\mu(\lim\sup A_{n})\leq \mu\left( \bigcup_{m\geq n}A_{m} \right)\leq \sum_{m\geq n}\mu(A_{m})\to 0
$$
### Lemma (Second Borel-Cantelli Lemma)
Assume that the events $(A_{n})$ are [[Independence|independent]]. 
If $\sum_{n}\mathbb{P}(A_{n})=\infty$ then $\mathbb{P}(\lim\sup A_{n})=1$.