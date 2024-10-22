Assume $\Omega=\Sigma \cup V$ and $\Sigma\cap V=\emptyset$, $\Sigma \neq \emptyset \neq V$
$\Sigma$ is the set of alphabet letters
$V$ is the set of variables

$\mathbb{W}=\Sigma ^{*}$ is the set of words
$L\subset \mathbb{W}$ is a formal language.
### Definition
$G=(\Sigma,V,S,P)$ is a grammar if $(\Sigma\cup V,P)$ is a [[Rewrite Systems|RWS]].
$S\in V$ is the start symbol

### Definition
$\mathcal{D}(G,\alpha)$ is the set of derivable strings (ie all string that we can obtain by applying a finite number of rewrite rules)
$\mathcal{L}(G)=\mathcal{D}(G,S)\cap \mathbb{W}$ is a language derived by $G$.

### Proposition
Isomorphic grammars are equivalent. (??)

### Definition
$\mathcal{G}(\Sigma,V)$ is the set of all grammars with $\Sigma,V$. This is countable.

### Lemma
Every grammar is equivalent to a variable-based grammar