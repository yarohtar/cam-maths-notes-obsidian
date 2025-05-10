### Type 0
[[Formal Language]] $\mathcal{L}(G)$ for any [[Grammar]] $G$.
### Type 1
[[Formal Language]] $\mathcal{L}(G)$ for [[Rewrite Rule#Context-free|context free]] [[Grammar]] $G$.
### Type 2
[[Formal Language]] $\mathcal{L}(G)$ for [[Rewrite Rule]]
Fix $\Sigma,V$ and $S\in V$.
A [[Grammar]] is called respectively if all production rules satisfy a property above.
A [[Formal Language]] is called respectively if produced by a grammar of certain type.
Additionally:
Type 0: $\mathcal{L}(G)$ for any grammar $G$
Type 1: $\mathcal{L}(G)$ for noncontracting $G$
Type 2: $\mathcal{L}(G)$ for context-free $G$ 
Type 3: $\mathcal{L}(G)$ for regular $G$ 

[[Regular Formal Language]]
[[Context-Free Formal Language]]

### Example
$L=\{ 0^{n}1^{n}:n>0 \}$ is context-free, not regular.
#### Proof
##### Contextfree
$S\to 0S 1$ and $S\to 01$ produces $L$
##### Not regular
Suppose it is. Then it satisfies [[Regular Pumping Lemma]]. 
But clearly it doesn't. 
