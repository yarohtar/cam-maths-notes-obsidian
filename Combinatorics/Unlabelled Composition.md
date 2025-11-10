Let $\mathcal{A}$ and $\mathcal{B}$ be [[Unlabelled Structure]]s.
Their unlabelled composition is defined as:
$$
\mathcal{B}(\mathcal{A}) = \sum_{k=0}^{\infty} B_{k} \times \mathcal{A}^{k}
$$
where $B_{k}=\mathcal{B}[k]$ and 
$$
\mathcal{A}^{k} = \underbrace{\mathcal{A}\times\dots \times \mathcal{A}}_{k \text{ times}}
$$
as the [[Combinatorial Product]].

### Lemma
Let $\mathcal{A}$ and $\mathcal{B}$ have [[Ordinary Generating Function]]s $f_{\mathcal{A}}$ and $f_{\mathcal{B}}$.
Then 
$$
f_{\mathcal{B}(\mathcal{A})} = f_{\mathcal{B}} \circ f_{\mathcal{A}}
$$
#### Proof
Firstly 
$$
f_{\mathcal{A}^{k}} = (f_{\mathcal{A}})^{k}
$$
as the [[Combinatorial Product]].
Now suppose 
$$
f_{\mathcal{A}^{k}} = \sum_{n} a_{n}^{(k)} x^{n}
$$
The combined weight of objects of size $n$ in $\mathcal{B}(\mathcal{A})$ is 
$$
\sum_{k} \sum_{b\in B_{k}} w(b) \cdot 
$$